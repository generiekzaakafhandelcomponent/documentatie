# Integratiepatronen

Bijzonder aan een zaakafhandelcomponent is dat ze een spin in het web vormt. Er wordt gekoppeld aan een groot aantal omliggende componenten. Er zijn twee patronen die veel worden toegepast, het synchroon en a-synchroon communiceren.

Synchrone communicatie is een communicatiestijl waarbij de vragende service wacht tot er een antwoord is van de antwoordende service. Er is direct contact tussen twee services. Het is een veelgebruikte aanpak - en ook de meest eenvoudige.

Synchrone communicatie zijn praktisch vaak calls naar een REST API - maar dat hoeft niet.

<figure><img src="../../.gitbook/assets/Screenshot 2023-05-28 at 18.56.21.png" alt="" width="375"><figcaption></figcaption></figure>

Voordelen:

* Eenvoudig / goedkoop.
* Meest ondersteund. De meeste componenten bieden standaard een REST API aan.

Nadelen:

* Service A wordt afhankelijk van service B. Omdat de vragende service wacht op het antwoord van de leverende service, beinvloedt de snelheid van B die van A. Als voorbeeld, als GZAC synchroon aan service B vraagt een PDF te genereren en dit duurt 5 seconden, stopt het proces en wacht tot de PDF klaar is. Het systeem doet in de tussentijd geen andere dingen. Bij een systeem A dat intensief door vele gebruikers wordt gebruikt kan dit problemen opleveren.
* Het vervangen van services wordt is mogelijk lastiger. Immers, systeem A is verbonden met systeem B - ze kennen elkaar. Systeem A authenticeert zich bij B zoals B dat wenst en vraagt de gegevens van systeem B volgens de specificaties van systeem B. Systeem B kan niet zomaar vervangen worden door een gelijksoortige dienst.
* Het opschalen is lastig. Systeem A vraagt expliciet een systeem B iets te doen. Als er een systeem B' wordt ingezet om werklast op te vangen, werkt dit niet 'uit de doos'.

#### A-synchrone communicatie

A-synchrone communicatie is een stijl waarbij de vragende service niet wacht op een antwoord van een andere service. Er is geen direct contact tussen de twee services, sterker: de services kennen elkaar niet.

Het principe is gestoeld op voorvallen - 'events'. Een service meldt dat er 'iets' is voorgevallen, zonder daarbij te weten dat daarop iets moet gebeuren. Andere service abonneren zich op deze 'events'. In het geval er een event voorvalt waarop zij moeten handelen, dan doen ze dat.

Als voorbeeld, service A meldt dat er een betaling is geslaagd (het event). Daarop abonneert service B zich, die daarop een factuur genereert. Service C abonneert zich ook op events van het type betaling, en schrijft in een logfile dat er een betaling heeft plaatsgevonden. Service A abonneert zich op events van het type 'factuur beschikbaar gekomen'. Indien dit voorvalt, informeert ze de betalende partij.

<figure><img src="../../.gitbook/assets/Screenshot 2023-05-28 at 18.58.35.png" alt="" width="375"><figcaption></figcaption></figure>

Uit dit voorbeeld blijkt dat services samenwerken zonder dat ze elkaar opdrachten geven, zonder dat ze op elkaar wachten en zonder dat ze elkaar uberhaupt kennen.

Meer weten? Het a-synchrone integratiepatroon was de basis van het project [VNG Notificaties Services](https://vng.nl/projecten/notificatie-services). Meer is ook te vinden op [Github](https://vng-realisatie.github.io/gemma-zaken/themas/achtergronddocumentatie/notificaties).

Binnen het ZGW-landschap wordt als standaard gebruik gemaakt van de [Notificaties API](https://vng-realisatie.github.io/gemma-zaken/standaard/notificaties/).

#### Informatiearm, a-synchrone communicatie

Binnen de groep koplopers Common Ground is gekozen voor het informatiearm a-synchroon communiceren. Dit betekent dat de informatie ('payload') van het bericht niet in de notificatie wordt vastgelegd maar in een separaat bericht. Vanuit de notificatie wordt verwezen naar dit bericht.

<figure><img src="../../.gitbook/assets/Screenshot 2023-05-28 at 19.06.39.png" alt="" width="375"><figcaption></figcaption></figure>

1. Vanuit een component - bijvoorbeeld portaal wordt een verzoek in de vorm van een object in de [Objects API](https://objects-and-objecttypes-api.readthedocs.io/en/latest/) geplaatst.
2. De objects API notificeert het [notificatie component](https://open-notificaties.readthedocs.io/en/latest/).
3. GZAC is geabonneerd op notificaties van een bepaald type en wordt op de hoogte gebracht van het feit dat er een nieuw bericht is.
4. GZAC vraagt het verzoek op uit de objects API.
