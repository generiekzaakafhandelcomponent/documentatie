# Data in zaakdossiers

Bij het lezen van deze pagina's ben je waarschijnlijk vooral op zoek naar informatie over processen. De structurering van data in je zaakdossier is echter minstens zo belangrijk als het ontwerp van de processen.

### Wat is een Zaakdossier?

Beginnend bij de basis, wat is een zaakdossier? Volgens NORA "_een digitale bundeling van alle bij een zaak horende informatie_".

<div align="left"><figure><img src="../.gitbook/assets/Screenshot 2023-06-09 at 10.18.47.png" alt="" width="563"><figcaption><p><a href="https://www.noraonline.nl/wiki/Het_vullen_en_archiveren_van_een_zaakdossier">https://www.noraonline.nl/wiki/Het_vullen_en_archiveren_van_een_zaakdossier</a></p></figcaption></figure></div>

De informatie in een zaakdossier kan verschillende vormen aannemen. Denk aan gestructureerde, door computer leesbare formaten zoals XML of JSON maar ook aan formaten die gericht zijn op de verwerking door mensen zoals PDF, Word en Excel.

Data hoeft niet 'fysiek' in het dossier te zitten, het kan ook een verwijzing zijn naar data die ergens anders is opgeslagen.

### Een zaak is data in beweging

Een zaakdossier is niet zomaar data - het is data in beweging. Het creëren van een zaakdossier heeft een aanleiding, er is behoefte aan iets. En, een zaakdossier heeft in veel gevallen ook een resultaat.

Een concreet voorbeeld is de behoefte aan een vergunning voor het organiseren van een evenement. Nadat een aanvraag voor een vergunning is gedaan (de aanleiding is altijd iets wat gebeurd is - een voltooid deelwoord) wordt er een zaakdossier aangemaakt. En bij goed verloop vanuit het perspectief van de aanvrager levert dat 'iets' op: in dit geval een vergunning.

<figure><img src="../.gitbook/assets/Screenshot 2023-06-09 at 10.37.14.png" alt=""><figcaption></figcaption></figure>

Een zaakdossier is tijdelijk. De afhandeling kan 3 minuten duren als het geheel geautomatiseerd gebeurt, het kan drie weken duren en soms zelf maanden, maar een zaakdossier is nooit permanent. Er is geen harde definitie van de maximale duur voor het afhandelen van een zaakdossier. Als vuistregel kan je aanhouden dat 3 tot 6 maanden lang is. Als je een zaakdossier ontwerpt dat langer dan een jaar gaat bestaan, vraag jezelf dan af of er wel sprake is van een zaakdossier.

<div align="center"><figure><img src="../.gitbook/assets/Screenshot 2023-06-09 at 10.50.02.png" alt=""><figcaption><p>Hoewel ook deze objecten niet eeuwig zullen bestaan en in die zin 'tijdelijk' zijn, zijn het geen zaakdossiers.</p></figcaption></figure></div>

### Soorten data

De **zaakdata** is de gegevensset die specifiek is voor een zaakdossier-type. Deze bestaat binnen GZAC uit:

* **zaak meta-data**. Deze is generiek: voor elk type zaakdossier worden dezelfde gegevens vastgelegd. Denk daarbij een zaaknummer, het zaakdossiertype, de registratiedatum en vertrouwelijkheidsaanduiding.
* het **zaakdetailobject**. Dit is de data die het hart van het zaakdossier vormt.
* **gerelateerd zaakobjecten**. Dit is _machine-readable_ data (bijvoorbeeld in JSON-formaat) die een rol heeft binnen het zaakdossier, en alleen benodigd voor het afhandelen van de zaak. Een voorbeeld is een gespreksverslag.
* **zelfstandig zaakobjecten .** Dit is _machine-readable_ data (bijvoorbeeld in JSON-formaat) die een rol heeft binnen het zaakdossier, maar ook buiten de context van een zaakdossier bestaansrecht heeft. Een voorbeeld is een lantaarnpaal binnen een MOR-melding.
* **zaakinformatieobjecten**. Dit is _niet-machine-readable_ data (bijvoorbeeld in PDF-formaat) die een rol heeft binnen het zaakdossier. In het spraakgebruik zijn dit documenten.
* **procesvariabelen**. Dit is stuurinformatie nodig voor de besturing van het zaakdossier, maar inhoudelijk niet relevant voor gebruikers in alle vormen. Een voorbeeld, aan de hand van een beslistabel wordt tijdelijk in het proces opgeslagen welk template-nummer gebruikt gaat worden voor het genereren van een brief. Na het generen is dit nummer niet relevant meer.

Het onderscheid tussen zelfstandig- en gerelateerd zaakobject wordt in de Gemma niet gemaakt maar is wel relevant voor archivering. Informatie die deel uitmaakt van de zaak moet worden gearchiveerd met de zaak, data die op zichzelf bestaansrecht heeft, niet. Concreet: als een zaakdossier voor de aanvraag van een uitkering wordt vernietigd, moeten de gespreksverslagen ook worden vernietigd, maar als een melding openbare ruimte (MOR)-zaakdossier wordt gearchiveerd moet de digitale informatie van de lantaarnpaal waar de melding over ging niet mee worden gearchiveerd.

Hoewel procesvariabelen data zijn die van invloed zijn op het verloop van het zaakdossier, kan worden betwist of processen onderdeel uitmaken van het zaakdossier. Om een goed overzicht te houden van alle mogelijkheden zijn ze hier wel vernoemd.

### Data binnen en buiten de context van het zaakdossier

Zoals al bleek uit de definitie van de verschillende soorten data, bevindt data zich niet per se _in_ het zaakdossier. Het zaakdossier is een conceptueel model, een digitale bundeling van alle informatie. Informatie kan op allerhande plekken staan.

Als een zaak gevisualiseerd zou worden als een hangmap, dan is de zaakmeta de informatie over het zaakdossier dat op het geeltje aan de buitenzijde staat. Het zaakdetail, gerelateerd zaakobjecten en de zaakinformatieobjecten zitten _in_ het zaakdossier. De zelfstandig zaakobjecten bevinden zich _buiten_ het zaakdossier, er wordt naar verwezen.\
\
Er kan ook worden verwezen naar andere informatie buiten de context van zaakdossiers. Binnen de gemeentelijke- en overheidscontext wordt gesproken over _registraties_. Voorbeelden zijn de Basisregistratie personen of het Handelsregister, maar ook interne registraties zoals die van alle binnenkomende Verzoeken. Buiten het gemeentelijk domein wordt bij data die zich buiten het zaakdossier bevindt ook wel gesproken over _master data._

<figure><img src="../.gitbook/assets/Screenshot 2023-06-09 at 14.21.55.png" alt=""><figcaption></figcaption></figure>

Voor de gebruiker is dat onderscheid niet altijd zichtbaar - informatie kan prima in de userinterface als één geheel worden getoond.

Voor de volledigheid:

* het product van een zaakdossier kan ook weer een object zijn - maar behoort feitelijk niet meer tot de zaak. Er kan gekozen worden om de link naar het product op te nemen, dit wordt dan een zelfstandig zaakobject.
* de aanleiding voor de zaak maakt formeel geen deel uit van het zaakdossier. De aanleiding wordt ProductAanvraag of Verzoek genoemd. Wel kan besloten worden om na het aanmaken van het zaakdossier de ProductAanvraag of Verzoek toe te voegen.
* de opdeling zoals geschetst is conceptueel, niet technisch. Data die zich conceptueel binnen het zaakdossier bevindt, bevindt zich niet per se binnen (de database van) het component GZAC.

### GZAC in het Commom ground 5 lagenmodel

Zoals in de introductie aangegeven is het zaakdossier een conceptuele bundeling van informatie. Als een Verzoek (ofwel ProductAanvraag) in GZAC binnenkomt, maakt het systeem een dossierrecord in de database (een 'case'), waarna een BPMN-proces wordt gestart. Vervolgens wordt gestart met het verwerken van binnengekomen informatie.

Een voorbeeld van een service architectuur is hier weergegeven:

<figure><img src="../.gitbook/assets/Screenshot 2023-06-09 at 16.04.47.png" alt=""><figcaption><p>Micro service architectuur, volgens Haags model</p></figcaption></figure>

* Een kleine set aan metadata wordt vastgelegd in GZAC, de ZGW-specifieke meta-data in OpenZaak.
* Het Zaakdetail ligt gedurende de afhandeling primair vast in GZAC, het zaakdetail' wordt direct gekopieerd naar de Objects API.
* De meta-data van documenten en de documenten liggen vast in de Documenten API. De fysieke locatie van de documenten is instelbaar, bijvoorbeeld een DMS of schijf ('persistant volume').
* Zelfstandig- en gerelateerd zaakobjecten liggen vast in de Objects API.

### Praktische tips

* Het zoeken over gegevens uit meerdere bronnen (JOIN's over REST API's) duurt lang. Voorbeeld 'zoek voor alle bedrijven groter dan 100 medewerkers in de plaats Den Haag in de KVK API alle bijbehorende Zaken in de Zaken API met de status 'in behandeling'. Zorg voor dat alle data waarop gezocht wordt, wordt opgenomen in het Zaakdetail - en accepteer dataduplicatie. In teams met procoders kan overwoging om een cachinglaag in te zetten.

<figure><img src="../.gitbook/assets/Screenshot 2023-09-15 at 15.01.51.png" alt=""><figcaption></figcaption></figure>

* Zorg dat het de JSON structuur van het Zaakdetail Object zodanig eenvoudig is, dat deze werkbaar is voor low-code formio formulieren. Grote document definities zijn geen probleem, complexe structuren wel.
* Dupliceer geen data waarop niet gezocht wordt, maar haal deze op bij de bron. Zorg dat de user interface deze '[lazy loadt](https://en.wikipedia.org/wiki/Lazy_loading)', zodat de gebruiker wel toegang heeft tot data die snel beschikbaar is.
* Gebruik voor stuurinformatie procesvariabelen. Implementatieteams vinden het werken met het Zaakdetail vaak fijn, neigen stuurdata daar te plaatsen.
* GZAC biedt geen mogelijkheid om binnen het zaakdetail object rechten toe te kennen op attribuutniveau. Indien rechten op delen het zaakdossier aan bepaalde medewerkers wordt verleend, maak gebruik van losse (zaak)objecten.
* Gebruik JSON Objecten niet als relationeel model. De Objects API biedt geen referentiële integriteit. Referentiële integriteit in een relationele database is het uitgangspunt dat de interne consistentie tussen de verschillende tabellen binnen die database wordt gewaarborgd.
* Start met een grondig uitgewerkt datamode. GZAC v12 voorziet niet in datamigratie. Het aanpassen van JSON schema's na het configureren van formulier-definities kan aanpassingen nodig maken in de formulieren. GZAC voorziet (nog) niet in een mechanisme voor versiebeheer van formulieren.
* Zorg dat data zoveel als mogelijk _machine readable_ wordt opgeslagen. Deze zijn kleiner, de gegevens zijn te doorzoeken/filteren en te verwerken in output. Als voorbeeld, teams zijn geneigd om een besluit met motivatie in PDF in een Zaakdossier vast te leggen. Overweeg JSON, de PDF kan altijd worden gegeneerd op basis van de informatie in JSON.\
