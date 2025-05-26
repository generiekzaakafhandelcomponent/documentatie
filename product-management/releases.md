# Releases

### GZAC Valtimo v13.0.0 Beta release

22 mei 2025: de Beta release van Valtimo 13 is uit, met daarin:

* Alles gerelateerd aan een dossier on 1 plek: een duidelijk overzicht wat bij elkaar hoort
* Alles geversioneerd: maak sneller een nieuwe iteratie zonder zorgen over backwards compatibility
* Concept dossier definities: laat de gebruikers werkende processen testen i.p.v WIP
* Betere performance, verbeterde veiligheid
* SSE: realtime updates!
* And meer.. stay tuned!

Wil je deze Beta versie uitproberen? Stuur hier dan je [verzoek](https://request.demo.k8s.ritense.com/).&#x20;

### GZAC Valtimo v12.12

### GZAC Valtimo v12.11

### GZAC Valtimo v12.10

### GZAC Valtimo v12.9

### GZAC Valtimo v12.8

### GZAC Valtimo v12.7

### GZAC Valtimo v12.6

### GZAC Valtimo v12.5

### GZAC Valtimo v12.4

### GZAC Valtimo v12.3

### GZAC Valtimo v12.2

19 augustus. In GZAC Valtimo 12.2 is het mogelijk om de dossierpagina samen te stellen met behulp van de nieuwe **widgets**. Data uit meerdere **bronnen** kan eenvoudig worden getoond in een widget. Naast standaard datavelden zijn er meerdere vormen beschikbaar, zoals een tabel.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2024-09-19 at 13.56.01.png" alt="" width="563"><figcaption></figcaption></figure>

In GZAC Valtimo 12.2 biedt de beheeromgeving ondersteuning voor het selecteren van data, in plaats van het handmatig opgeven van een pad (JsonPath of JsonPointer). Dit maakt het configureren van bijvoorbeeld zoekvelden of kolommen eenvoudiger, sneller en minder foutgevoelig.

### GZAC Valtimo v12.1

25 juli. In GZAC Valtimo 12.1 zijn er een aantal verbeteringen doorgevoerd aan de Documenten tab. De getoonde kolommen in de Documenten lijst zijn nu configureerbaar door de beheerder, die daarmee per dossier-type kan bepalen welke informatie relevant is. Daarnaast kan de beheerder nu trefwoorden instellen die gebruikt kunnen worden om aan de Documenten te koppelen, en deze daarmee te filteren.&#x20;

{% embed url="https://player.vimeo.com/video/993513068" %}

Ook is het in v12.1 mogelijk om taken te filteren op basis van dossierdata. De beheerder kan de zoekvelden in het taakscherm configureren per dossiertype.

### GZAC Valtimo v12.0

27 juni. In deze release zit o.a. de mogelijkheid **takenlijst** te filteren op het type dossier, en data uit de (zaak)dossier te te tonen in kolommen. Zo krijgen de taken de noodzakelijke contextuele informatie om zonder de taak te open te kunnen besluiten deze te behandelen.&#x20;

{% embed url="https://vimeo.com/936317640?share=copy" %}
Takenlijst filter
{% endembed %}

Er is een **dark mode** toegevoegd, na feedback over de 'witte' schermen bij intensief gebruik. Elke gebruiker kan deze instelling maken onder de persoonlijke settings.

<figure><img src="../.gitbook/assets/Screenshot 2024-04-18 at 15.43.40 (1).png" alt=""><figcaption><p>GZAC Dark mode</p></figcaption></figure>

Met behulp van **FormFlow** kunnen formulieren worden gebouwd die uit meerdere stappen bestaan, waarbij tussen de stappen backend code aangeroepen kan worden of condities kunnen worden uitgevoerd.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2024-06-27 at 10.58.27.png" alt=""><figcaption></figcaption></figure>

Er is een nieuwe editor ingebouwd, de open source **Microsoft Monaco editor** . Deze biedt de mogelijkheid om via de user interface JSON bestanden te beheren.&#x20;

Het **beheren van formulieren** is verbeterd, met onder meer de meer de mogelijkheid om direct via de admin in de JSON te werken. Daarnaast wordt er een preview getoond van het formulier dat gebouwd wordt, zodat je direct kan testen met data.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2024-06-27 at 11.00.24.png" alt=""><figcaption></figcaption></figure>

Dossiers kunnen in GZAC 12.0 standaard voorzien worden van een **status**, in te stellen door de beheerder. De dossierstatus wordt getoond op de dossierpagina en in de dossierlijst. Dossiers filteren op basis van de status is standaard mogelijk, evenals het aangeven dat dossiers met bepaalde statussen niet standaard in de lijst getoond moeten worden.

### GZAC Valtimo v11.3

Op 2 mei is GZAC Valtimo 11.3.0 gereleased. In deze nieuwe release wordt 'termijnbewaking' geintroduceerd, waarmee de einddatum van een Zaak kan worden aangepast in geval van een hersteltermijn. Op die manier kunnen inwoners geinformeerd worden over de verwachte doorlooptijd van hun verzoek. Daarnaast biedt de Zaak plugin nu ondersteuning voor Zaakeigenschappen.

### GZAC Valtimo v11.2

5 april 2023: release 11.2.0 is uit. In deze nieuwe release zijn een aantal nieuwe features beschikbaar, waaronder het kunnen importeren en exporteren van documentdefinities vanuit een ZIP archief. Verder worden nu ook Keycloak groepsrollen ondersteund in de Access control feature en zie je nu ook de versie van het proces op de 'progress' tab van een dossier. Zie voor de volledige lijst [hier](https://docs.valtimo.nl/release-notes/11.x.x/11.2.0/valtimo-backend-libraries) en [hier](https://docs.valtimo.nl/release-notes/11.x.x/11.2.0/valtimo-frontend-libraries).&#x20;

{% embed url="https://vimeo.com/936309895?share=copy" %}
Export en import van documentdefinitie
{% endembed %}

### GZAC Valtimo v11.1

22 december 2023: release 11.1 is uit. In deze versie introduceren we 'tab management'. Met deze feature kunnen beheerders configureren welke tabbladen er getoond worden op de dossier-pagina. We ondersteunen standaard tabs, tabs met formulieren of custom frontend-componenten. De laatste patch op deze minor versie is 11.1.5, zie voor meer info [hier](https://docs.valtimo.nl/release-notes/11.x.x/11.1.5/valtimo-frontend-libraries).

{% embed url="https://vimeo.com/936232003?share=copy" %}
Tab management
{% endembed %}

### GZAC Valtimo v11.0

14 december 2023: release 11.0 is beschikbaar. In deze versie wordt Access control geïntroduceerd: een framework om fijnmazig toegangsrechten te beheren. De beheerder kan de permissies configureren met behulp van de JSON-editor in de beheeromgeving.

Versie 11.0 bevat diverse security- en performance verbeteringen. Ook is verouderde code opgeschoond.

{% embed url="https://vimeo.com/936229717?share=copy" %}
Access control
{% endembed %}

### GZAC Valtimo v10.8

1 december 2023, release 10.8 is beschikbaar en de laatste patch release voor deze minor (10.8.3 is gereleased op 19 februari). In deze versie zijn er eigenschappen (verloopdatum en zaak) toegevoegd aan de portaaltaak, wanneer een portaaltaak is aangemaakt via de portaaltaak plugin.&#x20;

Daarnaast is de performance is verbeterd en verschillende bug fixes zijn doorgevoerd, zie voor meer gedetailleerde informatie [hier](https://docs.valtimo.nl/release-notes/10.x.x/10.8.0/valtimo-backend-libraries).&#x20;

### GZAC Valtimo v10.7

4 oktober 2023, release 10.7 is beschikbaar voor download. Nieuw in deze release:&#x20;

**Dashboards**

{% embed url="https://player.vimeo.com/video/871027565" %}

**Kleine uitbreidingen**

* Notities kunnen nu worden bewerkt en verwijderd.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2023-10-04 at 14.24.32.png" alt=""><figcaption></figcaption></figure>

* Taken kunnen nu automatisch met het zaakdossier verhuizen naar een andere behandelaar.&#x20;
* Het kruimelpad en de paginatitel zijn omgezet naar het Carbon Design System. Er zijn in de hele applicatie nieuwe kruimelpaden en paginatitels geïntroduceerd om een consistente gebruikerservaring met Carbon-componenten te bieden.&#x20;
* Menu-items kunnen in een nieuwe tab worden geopend door met de rechtermuisknop op een item te klikken.&#x20;

### GZAC Valtimo v10.3

24 februari 2023, release 10.3 is beschikbaar voor download. Nieuw in deze release:&#x20;

**Zoekopdrachten delen met collega's**

Zoekopdrachten kunnen nu worden gebookmarkt en worden doorgestuurd naar collega's, indien ze de juiste rechten hebben tot het Zaakdossier.&#x20;

**Ondersteuning voor selectielijsten in zoek**

In de configuratie van zoekvelden is nu de mogelijkheid om keuzelijsten te maken.&#x20;

{% embed url="https://vimeo.com/801879653" %}

**De lijst van bug-fixes, beveilingsverbeteringen en kleinere features** is te vinden op [https://docs.valtimo.nl/release-notes/10.x.x/10.3.0-rc/valtimo-backend-libraries](https://docs.valtimo.nl/release-notes/10.x.x/10.3.0-rc/valtimo-backend-libraries) .&#x20;

### GZAC Valtimo v10.2

30 januari 202&#x33;_._ Release 10.2 is beschikbaar! Nieuw in deze tweede release van 2023:

**Notities**

De release heeft een eerste eenvoudige opzet van notities. Medewerkers kunnen aantekeningen bij een Zaakdossier maken. Dit maakt het mogelijk om naast de gestructureerde zaak-data ook wat informelere informatie bij te houden over een zaak. De informatie wordt in laag 4 opgeslagen - in de loop van dit jaar wordt ondersteuning voor de [Contactmomenten API](https://vng-realisatie.github.io/gemma-zaken/standaard/contactmomenten/) verwacht.&#x20;

{% embed url="https://vimeo.com/794406845" %}

**Plugins voor de** [**VNG Realisatie Notificaties API** ](https://vng-realisatie.github.io/gemma-zaken/standaard/notificaties/index)**standaard en de** [**OpenNotificaties**](https://github.com/open-zaak/open-notificaties) **implementatie**&#x20;

Er zijn twee nieuwe plugins! De Notificaties API plugin maakt het mogelijk om vanuit GZAC notificaties uit te wisselen met alle software die de VNG Realisatie standaard ondersteunt. De tweede plugin levert authenticatie voor de OpenNotificaties implementatie die is ontwikkeld door Maykin onder regie van Dimpact. Het is nu mogelijk om zonder code notificaties te sturen en te ontvangen vanuit een procesmodel.&#x20;

**Beheren van kolommen in een Zaakdossierlijst**

Voor beheerders is het nu mogelijk om via de admin-schermen de kolommen van een zaakdossier in te stellen. Dit kon voorheen alleen in een configuratie-file. De beheerder kan de lijst samenstellen uit alle eigenschappen die in het Zaakdetail Object zijn opgenomen, aangevuld met enkele altijd beschikbare eigenschappen zoals de startdatum.&#x20;

{% embed url="https://vimeo.com/794552794" %}

**Plant-een-boom-knop**

Vanuit een persoonlijk initiatief, onder de log-uitknop is een knop toegevoegd waarmee je een verzoek kan sturen een boom te planten om de CO2 uitstoot voor de installatie te compenseren. Eén per persoon :-).&#x20;

**GZAC editie standaard plugins**

Vanaf deze release komt een selectie aan plugins standaard mee met de GZAC editie, steeds in hun laatste versie, waarbij de compatibiliteit wordt bewaakt. Zo hoef je niet zelf plugins toe te voegen - en zijn ze ook zonder bouwen beschikbaar.

**En een lijst van bug-fixes, beveilingsverbeteringen en kleinere features.** De complete lijst staat op [https://docs.valtimo.nl/release-notes/10.x.x/10.2.0/valtimo-frontend-libraries](https://docs.valtimo.nl/release-notes/10.x.x/10.2.0/valtimo-frontend-libraries) en [https://docs.valtimo.nl/release-notes/10.x.x/10.2.0/valtimo-backend-libraries](https://docs.valtimo.nl/release-notes/10.x.x/10.2.0/valtimo-backend-libraries)&#x20;

### GZAC Valtimo v10.1&#x20;

15 januari 2023. Release 10.1 is beschikbaar! Deze sprint is er ook nog een laatste release van Major 9 vrijgegeven (9.26.0), wat direct de laatste is in die reeks. Vanaf nu zullen er alleen security- en bugfixes worden vrijgegeven met hotfixes. &#x20;

#### FormFlow

Deze release brengt uitbreidingen in FormFlow. FormFlow maakt het mogelijk om binnen een gebruikerstaak formulieren te bouwen die uit stappen bestaan – zoals de belastingdienstformulieren. Het is nu mogelijk om ‘server side’ conditionele volgende stappen te definiëren. Bijvoorbeeld, op basis van een bedrag dat de invuller aangeeft kan worden bepaald of de aanvrager in aanmerking komt voor een subsidie. Indien de aanvrager niet in aanmerking komt, wordt de aanvraag niet ingediend – en wordt dus op voorhand voorkomen dat er een Zaak wordt aangemaakt die tot afwijzing leidt – met besparing van het werk dat daarbij komt kijken.&#x20;

{% embed url="https://player.vimeo.com/video/790805033" %}

Verder zijn er verbeteringen die het implementeren sneller maken, en is er feedback van gebruikers verwerkt, zoals het opslaan van gegevens als er een stap terug wordt gezet. Alle details staan in de [documentatie](https://docs.valtimo.nl/release-notes/10.x.x/10.1.0/valtimo-backend-libraries).&#x20;

#### Basisprocessen

Het eerste Basisproces staat op Github. Basisprocessen helpen gemeentes om snel een bedrijfsproces op te zetten aan de hand van een voorbeeld. Een beetje van jezelf en een beetje van Maggi. Een Basisproces wordt geïmporteerd in GZAC en waar nodig aangepast aan lokale wensen en eisen. Een email-template zal bijvoorbeeld lokaal anders zijn, en een rechtenstructuur ook. Er is op dit moment een eerste voorbeeld beschikbaar. Wil je aan de slag, zorg dat je een implementatie kan builden hebt en start bij de [documentatie](https://github.com/generiekzaakafhandelcomponent/Basisprocessen).

<figure><img src="../.gitbook/assets/Screenshot 2023-01-18 at 15.25.55.png" alt=""><figcaption></figcaption></figure>
