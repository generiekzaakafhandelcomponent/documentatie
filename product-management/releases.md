# Releases

### GZAC Valtimo v13.14.0

4 februari 2026 - nieuwe minor release met onder andere nieuwe functionaliteiten, verbeteringen en bug-fixes:

* De plugin “Link document to zaak” ondersteunt nu twee nieuwe properties: ‘vernietigingsdatum’ en ‘status’. Deze worden toegevoegd aan het zaakinformatieobject tijdens het koppelen van een document aan een zaak.
* Bij het verwijderen van een zaak worden gekoppelde documenten nu alleen verwijderd uit de Documenten API als ze niet aan andere zaken zijn gekoppeld. Documenten die aan meerdere zaken zijn gekoppeld blijven beschikbaar; alleen de relatie tussen de zaak en het document wordt verwijderd.
* Bouwblokken kunnen nu worden aangeroepen vanuit onafhankelijke processen die niet aan een zaak zijn gekoppeld.
* Wat is opgelost in deze release: een nieuw aangemaakte zaak binnen de Zaken API plugin  is nu correct aangekoppeld aan de case wanneer deze wordt gebruikt in een bouwblok, het contextmenu in het case-detail toont de actie 'Ontkoppelen' nu alleen wanneer de gebruiker beschikt over de juiste toewijzingsrechten, de uploadmodals voor casedefinities en bouwblokken zijn consistenter vormgegeven en andere kleinere fixes

###

### GZAC Valtimo v13.13.0

28 januari 2026 - minor release met super belangrijke functionaliteiten waaronder:

* Bouwblokken - Met Bouwblokken kunnen veelgebruikte processtappen eenvoudig opnieuw ingezet worden in meerdere zaken. Dit zorgt ervoor dat gedeelde onderdelen van processen overal hetzelfde blijven en makkelijker te beheren zijn. Bouwblokken kunnen ook eenvoudig worden meegenomen naar andere omgevingen.
* Integratie met IKO-server - de GZAC-gebruikers kunnen nu een actueel en compleet overzicht  krijgen van klant- en objectinformatie. Hierdoor kunnen burgers, bedrijven en instellingen sneller en duidelijker worden geholpen.
* Widget-configuratie is nu beschikbaar gemaakt voor custom components&#x20;
* Verplichte velden zijn aangepast voor "_Employee_", "_Organisational unit_" en "_Branch_" in Zaken API&#x20;
* Het is nu mogelijk om te wisselen tussen de stappen van de configuratie binnen de proceslink-modal.
* Een paar bugfixes, o.a. taken worden niet langer automatisch afgesloten wanneer een andere gebruiker de taaktoewijzing wijzigt, de LockProvider-configuratie ondersteunt nu het instellen van de tijdzone via configuratie-eigenschappen en gebruikt standaard UTC als er niets is opgegeven.



### GZAC Valtimo v13.12.0

21 januari 2026 - deze release bevat:

* Duidelijkere versieregels voor casedefinities: bij het aanmaken van een casedefinitie wordt nu duidelijk aangegeven dat het versienummer een standaard formaat moet volgen (bijvoorbeeld: 1.0.0).
* Betere zichtbaarheid wanneer een proces een probleem ondervindt - het is nu mogelijk om automatisch een foutmelding vast te leggen wanneer een Operaton-proces in een incidentstatus terechtkomt. Dit helpt teams om problemen sneller te signaleren en indien nodig meldingen (alerts) in te stellen. Meer informatie hierover vind je in de documentatie over incident error logging.
* Wat is opgelost in deze release: We hebben een probleem opgelost waarbij de applicatie `logging_event`-fouten kon tonen bij het opstarten met een lege database

###

### GZAC Valtimo v13.11.0

14 januari 2026 - nieuwe minor release met onder andere nieuwe functionaliteiten, verbeteringen en bug-fixes:

* Er is een nieuwe functionaliteit toegevoegd aan de Documenten API: het is nu mogelijk om bestandstypen te beperken in de uploader FormIO-component. De bestandsextensie van het geüploade bestand weerspiegelt nu altijd het daadwerkelijke bestandstype, ook wanneer we de bestandsnaam programmatisch instellen vanuit de Documenten API-uploadercomponent.
* Om de gebruikerservaring te verbeteren en de systeemprestaties te verhogen, hebben we lazy loading geïntroduceerd voor de case widgets.
* Wat is opgelost in deze release: paginering op de keuzeveld-pagina, een fout bij het ophalen van gebruikers uit Keycloak (versie 26.3.0 of nieuwer), de documenttype-dropdown van de Documenten API.



### GZAC Valtimo v13.10.0

7 januari 2026 – De eerste release van 2026 bevat een aantal kleine verbeteringen:

* De lijst met zaakdefinities in het menu is nu alfabetisch gesorteerd.
* Er is een nieuwe actie toegevoegd aan de Zaken API-plugin voor het bijwerken van de startdatum van een zaak.
* Diverse kleine maar belangrijke bugfixes, waaronder: de lijst met dossiers is weer zichtbaar op het JsonSchemaDocument, een migratieprobleem bij een groot aantal zaken is opgelost en everige kleine fixes

### GZAC Valtimo v13.9.0 / 13.9.1

24 december 2025 - een klein release met een belangrijke feature en bug-fix:

* Er is nieuwe functionaliteit toegevoegd: wanneer dit is ingeschakeld, worden bestanden die zijn geüpload naar de Documenten API of die zijn opgeslagen in tijdelijke bestandsopslag gescand op virussen.
* Opgelost: bij het uploaden van een ZIP-bestand worden de bestaande gegevens niet langer overschreven.

### GZAC Valtimo v13.8.0

17 december 2025 – nieuwe minor release met onder andere nieuwe functionaliteiten, verbeteringen en bug-fixes:

* De case properties kunnen nu direct vanuit Form.io worden aangepast. Ondersteunde TargetKeys-waarden:
  * `case:assigneeId` — past de case-verantwoordelijke aan
  * `case:internalStatus` — past de interne status van de case aan
  * `case:caseTags` — voegt een tag toe aan de case
* Key en value kunnen nu worden geconfigureerd in de custom component widgets.
* Documenttypes in de Documenten API zijn alfabetisch geordend en doorzoekbaar.
* De Zaken API-plugin is uitgebreid met een nieuwe actie om een zaaknotitie te creëren en aan de zaak te koppelen.
* Deze release bevat ook enkele bug-fixes, waaronder process-links zijn nu gefixt met de juiste versie; vertalingen in de Catalogi API zijn gecorrigeerd.

### GZAC Valtimo v13.7.0

10 december 2025 - een klein release met paar nieuwe features en bug-fixes:

* Er zijn drie nieuwe _retry cycle_-opties beschikbaar voor Tasks, Call Activities, Subprocesses en Events: **DEFAULT**, **QUICK** en **CRITICAL**, die aangepast en gedefinieerd kunnen worden.
* Alle widgets hebben nu ook een compacte modus. Dit kan worden ingesteld tijdens de widgetconfiguratie

<figure><img src="../.gitbook/assets/Screenshot 2025-12-10 at 15.54.29.png" alt=""><figcaption></figcaption></figure>

* Kleine bugfixes zijn ook doorgevoerd, waaronder verbeteringen aan plugin, en gedraag van Auto Key input component.

### GZAC Valtimo v13.6.0

27 november 2025 - nieuwe minor release met o.a nieuwe functionaliteiten en diverse bug-fixes:

* Zaken API-plugin heeft enkele veranderingen: een datum voor een zaakstatus kan nu worden ingesteld en zaakbesluiten kunnen nu worden opgehaald
* De Besluiten API plugin is uitgebreid met een plugin action waarmee de vervaldatum en vervalreden op een eerder vastgelegd besluit aangepast kan worden
* Een nieuwe widget — de kaart-widget — is toegevoegd&#x20;
* Een actieknop kan nu bij bijna alle widgets worden toegevoegd tijdens de configuratie. Deze knop kan worden gebruikt om een zaak te starten of de gebruiker naar een externe link te brengen
* Er zijn meerdere bugfixes en UI-verbeteringen doorgevoerd. Zo worden radioknoppen nu naast elkaar getoond, gaat de applicatie beter om met tijdzone-informatie, is de verwerking bij het ophalen van gebruikers sneller, kunnen icoontjes nu worden toegevoegd tijdens de widget-configuratie en meer.

### GZAC Valtimo v13.5.0

05 november 2025 - nieuwe minor release met o.a nieuwe functionaliteiten, verbeteringen en bug-fixes:

* OpenZaak-plugin is bijgewerkt met een nieuwe actie waarmee een Zaak-rolen kunnen worden verwijderd zodra deze niet langer beschikbaar zijn.
* Meerdere beveiligingsverbeteringen aan de applicatie zijn doorgevoerd.
* Prestatieverbeteringen bij het ophalen van taken en zaken zijn nu uitgerold.
*   Meerdere bug-fixes, onder anderen koppelingen tussen processen en formulieren worden nu altijd correct meegenomen, zaaktags en header-widgets worden nu goed overgenomen in nieuwe conceptversies, bij het uploaden van een document wordt het veld met document typen automatisch ingevuld (indien beschikbaar), bij het aanmaken van een nieuwe zaak-widget worden voorwaarden van eerder geopende widgets niet langer vooraf ingevuld, de titels van FormIO- en aangepaste widgets worden nu correct weergegeven, widgets UI correcties en meer.



### GZAC Valtimo v13.4.0

21 oktober 2025 – Deze release bevat:

* Snelle zoekfunctie toegevoegd aan de case lijst
* Kolommen in de case lijst kunnen nu worden verborgen of weergegeven, zodat relevante informatie gemakkelijker te zien is
* Widgets kunnen nu worden gegroepeerd
* En last but not least in dit pakket: de Case Header Widget, waarmee belangrijke case-informatie duidelijk bovenaan de detailpagina wordt weergegeven.
* Kleine bugfixes zijn ook doorgevoerd, waaronder verbeteringen aan vertalingen, de knop-UI, plugin configuraties en meer.

### GZAC Valtimo v13.3.0

8 oktober 2025: nieuwe minor release met o.a nieuwe functionaliteiten:

* Gebruikers kunnen nu case-objecten toevoegen aan een case
* Bij het aanmaken van een nieuwe case in Open Zaak is het nu mogelijk om meer case-details toe te voegen
* Condities kunnen nu worden gedefinieerd en ingesteld voor de weergave van case-widgets
* Diverse bugfixes, zoals verbeterde prestaties van widget pagina’s, algemene performance verbeteringen, kleine UI-correcties en verbeterd gedrag van de verzoek-plugin.

### GZAC Valtimo v13.2.0

16 september 2025: verdere uitbreidingen van v13, waaronder:

* Case-widgets hebben nu een klikbare link waarmee case-informatie in een nieuw tabblad kan worden geopend.
* Het is nu mogelijk om direct van een taak naar een case over te schakelen.
* Case-informatie kan nu worden geëxporteerd.
* Beveiliging van toegangsrechten is verder verbeterd.
* Een snelle zoekfunctie is toegevoegd.
* De documentdefinitie naam wordt nu automatisch ingevuld op basis van de huidige case.
* Diverse bug-fixes met betrekking tot de migratie van V12 naar V13, vertalingen en processen.

### GZAC Valtimo v13.1.0&#x20;

20 augustus 2025: Beta - release met uitbreidingen is beschikbaar - dit zit erin:

* Case Definition-controle maakt het nu mogelijk voor gebruikers om details te bekijken op basis van hun toegewezen rol
* Gebruikers kunnen nu kolommen en zoekvelden zelf configureren&#x20;
* Widgets kunnen nu ook worden ingesteld
* Verbeteringen aan de Notificaties API zijn doorgevoerd voor meer betrouwbaarheid en betere prestaties
* Een nieuwe aanpak voor Form.io-formuliervertalingen is geïmplementeerd
* Diverse systeemverbeteringen met betrekking tot deployments, toegangsbeheer en algemene stabiliteit.

### GZAC Valtimo v13.0 Beta release

22 mei 2025: de Beta release van Valtimo 13 is uit, met daarin:

* Alles gerelateerd aan een dossier on 1 plek: een duidelijk overzicht wat bij elkaar hoort
* Alles geversioneerd: maak sneller een nieuwe iteratie zonder zorgen over backwards compatibility
* Concept dossier definities: laat de gebruikers werken de processen testen i.p.v WIP
* Betere performance, verbeterde veiligheid
* SSE: realtime updates!
* And meer.. stay tuned!

Wil je deze Beta versie uitproberen? Stuur hier dan je [verzoek](https://request.demo.k8s.ritense.com/).&#x20;

### GZAC Valtimo v12.14 coming soon...

29 mei 2025: ‼️Breaking change: versie 12.13.0 introduceert de implementatie van toegevoegde rolpermissie controles. Deze versie lost kwetsbaarheid (CVE 8,6) op in de Objecten-API plugin, [hier](https://github.com/advisories/GHSA-965r-9cg9-g42p) verder uitgelegd.

### GZAC Valtimo v12.13 (alleen back-end)

### GZAC Valtimo v12.12

9 mei 2025, een kleine release met één nieuwe functionaliteit en 2 bugfixes:

*   Mogelijkheid om einddatum van een taak aan te passen vanuit de taken modal (voor een gebruiker met de juiste rechten hiervoor)

    <figure><img src="../.gitbook/assets/Screenshot 2025-06-16 at 14.51.14.png" alt=""><figcaption><p>Aanpassen einddatum in taak</p></figcaption></figure>
* Bugfix rondom procesvariabele type Map

### GZAC Valtimo v12.11

10 april 2025:

* Dossiertags kunnen nu worden toegevoegd aan een dossier om extra informatie mee te geven aan het dossier. Tags kunnen getoond worden in de dossierlijst, op het dossierdetailpagina en kunnen gebruikt worden bij het zoeken van een dossier uit de dossierlijst.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2025-06-16 at 14.27.16.png" alt=""><figcaption><p>Dossiertags</p></figcaption></figure>

* Externe startformulieren kunnen geconfigureerd worden voor een dossiertype. Wanneer dit is geconfigureerd, wanneer je klikt op het aanmaken van een nieuw dossier, opent dit de geconfigureerde URL in een nieuwe browser tab.
* Meer components zijn omgezet naar het Carbon design systeem
* Verschillende bugfixes, zoals die gerelateerd aan het afhandelen van formulieren en het Form.io valuta component

### GZAC Valtimo v12.10

3 april 2025: nieuwe minor release met o.a.:&#x20;

* Optie tot het verbergen van taken die niet tot de afhandelrechten behoren van betreffende gebruiker
* Verscheidene bugfixes

### GZAC Valtimo v12.9

26 maart 2025:

* De overzichtelijkheid van de loggingdetails is verbeterd. Belangrijke regels in de stacktrace zijn nu gemarkeerd zodat ze beter leesbaar zijn en zodat er sneller 'gedebugged' kan worden.
* Verscheidene bugfixes, bv. bugs gerelateerd aan geüploade bestanden en Carbon tags

### GZAC Valtimo v12.8

4 maart 2025:

* Proceslinkconfiguraties kunnen nu herbruikt worden. Je kan nu een configuratie importeren van een andere proceslink vanuit dezelfde plugin.&#x20;

<figure><img src="../.gitbook/assets/image (1).png" alt="" width="375"><figcaption><p>Importeer configuratie</p></figcaption></figure>

* Verbergen van lege dossierwidgetvelden
* Rollen en rechten voor Documenten API documenten.  Toegang o.b.v. gebruiker kan ingeregel worden om documenten te bekijken, creeëren, beerkend en verwijderen
* Verscheidene bugfixes

### GZAC Valtimo v12.7

21 januari 2025:&#x20;

* Taakinformatie beschikbaar op het dashboard

<figure><img src="../.gitbook/assets/Screenshot 2025-06-10 at 14.37.12.png" alt=""><figcaption><p>Taakinformatie op het dashboard</p></figcaption></figure>

* Knoppen op de dossierwidgets om een ad-hoc/supporting proces te starten
* De optie om dossierwidgets and dashboardwidgets te dupliceren
* Value path selectoren, voor
  * Dashboard widgets
  * Verzoek, Portaaltaak en SmartDocuments plugin
* Ondersteuning voor custom UI componenten om taken te beheren
* Verschillende bugfixes

### GZAC Valtimo v12.6

20 december 2024: In deze laatste release van het jaar:

* Ondertitels voor taken om meer context te geven aan de zaakbehandelaar

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Ondertitel voor een taak (configuratiescherm)</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (2).png" alt="" width="375"><figcaption><p>Ondertitel voor een taak</p></figcaption></figure>

* De mogelijkheid om een ​​zaak te verwijderen gelijk vanaf de zaakdetailpagina (gebruiker moet hier wel rechten tot hebben)
* Een enorme prestatieverbetering in PBAC door het cachen van de gebruikersgegevens
* Toegangscontrole op gegevens in de startformulieren van ondersteunende processen
* Ondersteuning voor nieuwe regels in zaaknotities
* Niet langer verwijderen en opnieuw aanmaken van Notificatie API-abonnementen bij het opstarten
* Zaakdetails-object automatisch koppelen aan de Zaak
* Dashboard:
  * Persoonlijke dashboardwidgets. Je kan bijvoorbeeld op het dashboard het 'aantal aan mij toegewezen zaken' zien)
  * Klikbare dashboardwidgets naar een configureerbare URL. Bv. een widget die het aantal dossiers laat zien o.b.v. specifieke criteria kan doorlinken naar de dossierlijstpagina met hetzelfde toegapaste filter
  * Zaakwidgets die langere teksten op meerdere regels kunnen weergeven
* Configureerbare uploadvelden voor Documenten API, zodat zaakbehandelaars niet telkens elk veld hoeven in te vullen

<figure><img src="../.gitbook/assets/image (3).png" alt="" width="375"><figcaption><p>Configureerbare Documenten API metadata</p></figcaption></figure>

* Een handige, niet-toegankelijke zaakdetailpagina wanneer u geen rechten hebt om te bekijken
* Een oplossing voor de terugknop op de zaakdetailpagina
* Diverse andere kleinere dingen en bugfixes

### GZAC Valtimo v12.5

22 november 2024: Deze release bevat:

* Logging - bekijken en filteren/zoeken van logs in admin UI (na 21 dagen worden de logs automatisch verwijderd voor het voorkomen van een alsmaar groter wordende database).&#x20;

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption><p>Overzicht in Admin > Logs</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption><p>Filteren van de logs</p></figcaption></figure>

* Uploaden ZGW documenten in gedeeltes (zodat grote files toch nog toegevoegd kunnen worden).
* Gebruiken omgevingsvariabelen voor proceslink autodeployment
* Bugfixes

### GZAC Valtimo v12.4

25 oktober 2024: :warning: Deze release bevat een potentiële breaking change, nl. de vervanging van WebClient door RestClient, wat de stabiliteit verbetert.  Verder in deze release:

* De taken panel: bewerkstelligt gebruikers te navigeren tussen dossiertabs tegelijkertijd tijdens het invullen van het takenformulier. Admins kunnen instellen of het formulier in de modal of in de takenpanel getoond moet worden.

<figure><img src="../.gitbook/assets/Screenshot 2025-05-26 at 16.09.22.png" alt="" width="563"><figcaption></figcaption></figure>

* Veel Formulieren Flow verbeteringen
* Een nieuwe manier om formulieren te configureren is beschikbaar, nl. via een URL. Bij het gebruiken van deze feature kunnen externe formulieren worden gebruikt om een proces te starten of een gebruikerstaak te submitten.
* Bij het selecteren van een informstieobjecttype, bv. bij het uploaden van een document, de lijst van resultaten is nu gefilterd en ducmenttypes zijn alleen zichtbaar als:
  * ze definitief zijn/gepubliceerd
  * ze een valide startdatum hebben dat in het verleden ligt
  * ze geen einddatum hebben die al is gepasseerd
* De documentenlijst ondersteunt nu het tonen van resultaten op verschilende pagina's, oftewel 'pagination'
* Wanneer audit events zijn geïnitieerd bij het systeem is de auteur nu 'systeem' i.p.v. 'anoniem'.
* O.a bugfixes

### GZAC Valtimo v12.3

20 september 2024: In deze release:

* \[Documenten API] Geüploade documenten URLs worden nu lokaal opgeslagen in GZAC en opgevraagd door een REST API. Dat opent de deur naar het maken van een document-download form.io component, zowel als het uploaden van een document zonder het te hoeven selecteren voor het aanmaken van het besluit.&#x20;
* De taken panel feature, achter een feature toggle (enableTaskPanel)
* Het eerste gedeelte van technische logging verbeteringen
* Verschillende bugfixes

### GZAC Valtimo v12.2

19 augustus. In GZAC Valtimo 12.2 is het mogelijk om de dossierpagina samen te stellen met behulp van de nieuwe **widgets**. Data uit meerdere **bronnen** kan eenvoudig worden getoond in een widget. Naast standaard datavelden zijn er meerdere vormen beschikbaar, zoals een tabel.

<figure><img src="../.gitbook/assets/Screenshot 2024-09-19 at 13.56.01.png" alt="" width="563"><figcaption></figcaption></figure>

In GZAC Valtimo 12.2 biedt de beheeromgeving ondersteuning voor het selecteren van data, in plaats van het handmatig opgeven van een pad (JsonPath of JsonPointer). Dit maakt het configureren van bijvoorbeeld zoekvelden of kolommen eenvoudiger, sneller en minder foutgevoelig.

### GZAC Valtimo v12.1

25 juli. In GZAC Valtimo 12.1 zijn er een aantal verbeteringen doorgevoerd aan de Documenten tab. De getoonde kolommen in de Documenten lijst zijn nu configureerbaar door de beheerder, die daarmee per dossier-type kan bepalen welke informatie relevant is. Daarnaast kan de beheerder nu trefwoorden instellen die gebruikt kunnen worden om aan de Documenten te koppelen, en deze daarmee te filteren.

{% embed url="https://player.vimeo.com/video/993513068" %}

Ook is het in v12.1 mogelijk om taken te filteren op basis van dossierdata. De beheerder kan de zoekvelden in het taakscherm configureren per dossiertype.

### GZAC Valtimo v12.0

27 juni. In deze release zit o.a. de mogelijkheid **takenlijst** te filteren op het type dossier, en data uit de (zaak)dossier te te tonen in kolommen. Zo krijgen de taken de noodzakelijke contextuele informatie om zonder de taak te open te kunnen besluiten deze te behandelen.

{% embed url="https://vimeo.com/936317640?share=copy" %}
Takenlijst filter
{% endembed %}

Er is een **dark mode** toegevoegd, na feedback over de 'witte' schermen bij intensief gebruik. Elke gebruiker kan deze instelling maken onder de persoonlijke settings.

<figure><img src="../.gitbook/assets/Screenshot 2024-04-18 at 15.43.40 (1).png" alt=""><figcaption><p>GZAC Dark mode</p></figcaption></figure>

Met behulp van **FormFlow** kunnen formulieren worden gebouwd die uit meerdere stappen bestaan, waarbij tussen de stappen backend code aangeroepen kan worden of condities kunnen worden uitgevoerd.

<figure><img src="../.gitbook/assets/Screenshot 2024-06-27 at 10.58.27.png" alt=""><figcaption></figcaption></figure>

Er is een nieuwe editor ingebouwd, de open source **Microsoft Monaco editor** . Deze biedt de mogelijkheid om via de user interface JSON bestanden te beheren.

Het **beheren van formulieren** is verbeterd, met onder meer de meer de mogelijkheid om direct via de admin in de JSON te werken. Daarnaast wordt er een preview getoond van het formulier dat gebouwd wordt, zodat je direct kan testen met data.

<figure><img src="../.gitbook/assets/Screenshot 2024-06-27 at 11.00.24.png" alt=""><figcaption></figcaption></figure>

Dossiers kunnen in GZAC 12.0 standaard voorzien worden van een **status**, in te stellen door de beheerder. De dossierstatus wordt getoond op de dossierpagina en in de dossierlijst. Dossiers filteren op basis van de status is standaard mogelijk, evenals het aangeven dat dossiers met bepaalde statussen niet standaard in de lijst getoond moeten worden.

### GZAC Valtimo v11.3

Op 2 mei is GZAC Valtimo 11.3.0 gereleased. In deze nieuwe release wordt 'termijnbewaking' geintroduceerd, waarmee de einddatum van een Zaak kan worden aangepast in geval van een hersteltermijn. Op die manier kunnen inwoners geinformeerd worden over de verwachte doorlooptijd van hun verzoek. Daarnaast biedt de Zaak plugin nu ondersteuning voor Zaakeigenschappen.

### GZAC Valtimo v11.2

5 april 2023: release 11.2.0 is uit. In deze nieuwe release zijn een aantal nieuwe features beschikbaar, waaronder het kunnen importeren en exporteren van documentdefinities vanuit een ZIP archief. Verder worden nu ook Keycloak groepsrollen ondersteund in de Access control feature en zie je nu ook de versie van het proces op de 'progress' tab van een dossier. Zie voor de volledige lijst [hier](https://docs.valtimo.nl/release-notes/11.x.x/11.2.0/valtimo-backend-libraries) en [hier](https://docs.valtimo.nl/release-notes/11.x.x/11.2.0/valtimo-frontend-libraries).

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

1 december 2023, release 10.8 is beschikbaar en de laatste patch release voor deze minor (10.8.3 is gereleased op 19 februari). In deze versie zijn er eigenschappen (verloopdatum en zaak) toegevoegd aan de portaaltaak, wanneer een portaaltaak is aangemaakt via de portaaltaak plugin.

Daarnaast is de performance is verbeterd en verschillende bug fixes zijn doorgevoerd, zie voor meer gedetailleerde informatie [hier](https://docs.valtimo.nl/release-notes/10.x.x/10.8.0/valtimo-backend-libraries).

### GZAC Valtimo v10.7

4 oktober 2023, release 10.7 is beschikbaar voor download. Nieuw in deze release:

**Dashboards**

{% embed url="https://player.vimeo.com/video/871027565" %}

**Kleine uitbreidingen**

* Notities kunnen nu worden bewerkt en verwijderd.

<figure><img src="../.gitbook/assets/Screenshot 2023-10-04 at 14.24.32.png" alt=""><figcaption></figcaption></figure>

* Taken kunnen nu automatisch met het zaakdossier verhuizen naar een andere behandelaar.
* Het kruimelpad en de paginatitel zijn omgezet naar het Carbon Design System. Er zijn in de hele applicatie nieuwe kruimelpaden en paginatitels geïntroduceerd om een consistente gebruikerservaring met Carbon-componenten te bieden.
* Menu-items kunnen in een nieuwe tab worden geopend door met de rechtermuisknop op een item te klikken.

### GZAC Valtimo v10.3

24 februari 2023, release 10.3 is beschikbaar voor download. Nieuw in deze release:

**Zoekopdrachten delen met collega's**

Zoekopdrachten kunnen nu worden gebookmarkt en worden doorgestuurd naar collega's, indien ze de juiste rechten hebben tot het Zaakdossier.

**Ondersteuning voor selectielijsten in zoek**

In de configuratie van zoekvelden is nu de mogelijkheid om keuzelijsten te maken.

{% embed url="https://vimeo.com/801879653" %}

**De lijst van bug-fixes, beveilingsverbeteringen en kleinere features** is te vinden op [https://docs.valtimo.nl/release-notes/10.x.x/10.3.0-rc/valtimo-backend-libraries](https://docs.valtimo.nl/release-notes/10.x.x/10.3.0-rc/valtimo-backend-libraries) .

### GZAC Valtimo v10.2

30 januari 202&#x33;_._ Release 10.2 is beschikbaar! Nieuw in deze tweede release van 2023:

**Notities**

De release heeft een eerste eenvoudige opzet van notities. Medewerkers kunnen aantekeningen bij een Zaakdossier maken. Dit maakt het mogelijk om naast de gestructureerde zaak-data ook wat informelere informatie bij te houden over een zaak. De informatie wordt in laag 4 opgeslagen - in de loop van dit jaar wordt ondersteuning voor de [Contactmomenten API](https://vng-realisatie.github.io/gemma-zaken/standaard/contactmomenten/) verwacht.

{% embed url="https://vimeo.com/794406845" %}

**Plugins voor de** [**VNG Realisatie Notificaties API** ](https://vng-realisatie.github.io/gemma-zaken/standaard/notificaties/index)**standaard en de** [**OpenNotificaties**](https://github.com/open-zaak/open-notificaties) **implementatie**

Er zijn twee nieuwe plugins! De Notificaties API plugin maakt het mogelijk om vanuit GZAC notificaties uit te wisselen met alle software die de VNG Realisatie standaard ondersteunt. De tweede plugin levert authenticatie voor de OpenNotificaties implementatie die is ontwikkeld door Maykin onder regie van Dimpact. Het is nu mogelijk om zonder code notificaties te sturen en te ontvangen vanuit een procesmodel.

**Beheren van kolommen in een Zaakdossierlijst**

Voor beheerders is het nu mogelijk om via de admin-schermen de kolommen van een zaakdossier in te stellen. Dit kon voorheen alleen in een configuratie-file. De beheerder kan de lijst samenstellen uit alle eigenschappen die in het Zaakdetail Object zijn opgenomen, aangevuld met enkele altijd beschikbare eigenschappen zoals de startdatum.

{% embed url="https://vimeo.com/794552794" %}

**Plant-een-boom-knop**

Vanuit een persoonlijk initiatief, onder de log-uitknop is een knop toegevoegd waarmee je een verzoek kan sturen een boom te planten om de CO2 uitstoot voor de installatie te compenseren. Eén per persoon :-).

**GZAC editie standaard plugins**

Vanaf deze release komt een selectie aan plugins standaard mee met de GZAC editie, steeds in hun laatste versie, waarbij de compatibiliteit wordt bewaakt. Zo hoef je niet zelf plugins toe te voegen - en zijn ze ook zonder bouwen beschikbaar.

**En een lijst van bug-fixes, beveilingsverbeteringen en kleinere features.** De complete lijst staat op [https://docs.valtimo.nl/release-notes/10.x.x/10.2.0/valtimo-frontend-libraries](https://docs.valtimo.nl/release-notes/10.x.x/10.2.0/valtimo-frontend-libraries) en [https://docs.valtimo.nl/release-notes/10.x.x/10.2.0/valtimo-backend-libraries](https://docs.valtimo.nl/release-notes/10.x.x/10.2.0/valtimo-backend-libraries)

### GZAC Valtimo v10.1

15 januari 2023. Release 10.1 is beschikbaar! Deze sprint is er ook nog een laatste release van Major 9 vrijgegeven (9.26.0), wat direct de laatste is in die reeks. Vanaf nu zullen er alleen security- en bugfixes worden vrijgegeven met hotfixes.

#### FormFlow

Deze release brengt uitbreidingen in FormFlow. FormFlow maakt het mogelijk om binnen een gebruikerstaak formulieren te bouwen die uit stappen bestaan – zoals de belastingdienstformulieren. Het is nu mogelijk om ‘server side’ conditionele volgende stappen te definiëren. Bijvoorbeeld, op basis van een bedrag dat de invuller aangeeft kan worden bepaald of de aanvrager in aanmerking komt voor een subsidie. Indien de aanvrager niet in aanmerking komt, wordt de aanvraag niet ingediend – en wordt dus op voorhand voorkomen dat er een Zaak wordt aangemaakt die tot afwijzing leidt – met besparing van het werk dat daarbij komt kijken.

{% embed url="https://player.vimeo.com/video/790805033" %}

Verder zijn er verbeteringen die het implementeren sneller maken, en is er feedback van gebruikers verwerkt, zoals het opslaan van gegevens als er een stap terug wordt gezet. Alle details staan in de [documentatie](https://docs.valtimo.nl/release-notes/10.x.x/10.1.0/valtimo-backend-libraries).

#### Basisprocessen

Het eerste Basisproces staat op Github. Basisprocessen helpen gemeentes om snel een bedrijfsproces op te zetten aan de hand van een voorbeeld. Een beetje van jezelf en een beetje van Maggi. Een Basisproces wordt geïmporteerd in GZAC en waar nodig aangepast aan lokale wensen en eisen. Een email-template zal bijvoorbeeld lokaal anders zijn, en een rechtenstructuur ook. Er is op dit moment een eerste voorbeeld beschikbaar. Wil je aan de slag, zorg dat je een implementatie kan builden hebt en start bij de [documentatie](https://github.com/generiekzaakafhandelcomponent/Basisprocessen).

<figure><img src="../.gitbook/assets/Screenshot 2023-01-18 at 15.25.55.png" alt=""><figcaption></figcaption></figure>
