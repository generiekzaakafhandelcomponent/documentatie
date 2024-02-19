# Introductie GZAC Valtimo

### Waar staat ‘GZAC’ in GZAC Valtimo voor?&#x20;

GZAC is de afkorting van Generiek Zaakafhandelcomponent. Volgens GEMMA (GEMeentelijke Model Architectuur): “GZAC is e_en generiek component dat medewerkers ondersteunt bij het afhandelen van verschillende soorten zaken. Belangrijk is dat de Generieke Zaakafhandelcomponent geschikt is om zaken van alle typen af te handelen. Dus niet beperkt tot zaken van één domein._" Zie de website van [Gemma](https://www.gemmaonline.nl/index.php/GEMMA2/0.9/id-f2dfbd0b-9d36-405c-bdbe-827f3296de29) voor meer gedetaileerde informatie.&#x20;

### Hoe is GZAC ontstaan?&#x20;

In 2017 heeft de taskforce “Samen Organiseren” besloten om Common Ground uit te werken. De eerste twee jaren die volgden waren gefocussed op de <mark style="background-color:orange;">datalagen 1 t/m 3.</mark> Dit resulteerde in 2019 tot de eerste versie van OpenZaak – als referentie-implementatie en bewijs dat het model zou gaan werken.&#x20;

Daarmee kwam de vervolgvraag: hoe gaan we zaakafhandeling aansturen? Het antwoord werd gevonden in open source Business Process Model and Notation (BPMN) – de ISO standaard voor procesautomatisering. In dat jaar zijn er een tiental proof of concepts uitgevoerd door diverse gemeenten en samenwerkende organisaties, zoals de gemeente Groningen, Haarlem, Den Haag, Rotterdam, Dimpact en Wigo4it. Er is getest met diverse oplossingsrichtingen, waaronder Camunda en Valtimo – dat al enkele jaren in gebruik was bij de gemeente Breda. Dat resulteerde in de GZAC-editie van Valtimo, toegespitst op het gebruik op de Common Ground Zaakgericht Werken API’s.&#x20;

### Hoe verhoudt GZAC zich tot Valtimo?&#x20;

GZAC is een superset van Valtimo. Het zijn extra functies die alleen toepasbaar zijn in het Common Ground Zaakgericht Werken-landschap.&#x20;

### Het is open source?&#x20;

Klopt. De licentie die wij hanteren is [EUPL 1.2](https://eupl.eu/1.2/nl/), een licentie ontwikkeld door de Europese Unie. EUPL1.2 is het formaat dat in de Common Ground de voorkeur geniet. Open Source levert voordelen op:

* Controleerbaar: iedereen kan zien wat de kwaliteit van het product is
* Alles wat een keer geschreven is, kunnen anderen ook weer gebruiken&#x20;

### Hoe is de uitbouw en het onderhoud georganiseerd?

Er werkt een vast team vanuit Ritense aan het bouwen en onderhouden van Valtimo. Dit omvat het bouwen van nieuwe functionaliteiten, het schrijven van documentatie, het ondersteunen van gebruikers, het fixen van bugs, het onderhouden van de honderden (!) dependencies om het product veilig te houden, het draaien van security scans, het beheren van de CI-pipenline en nog veel meer. Dit alles wordt deels gefinancierd vanuit abonnementen die de afnemers garanties geven op kwaliteit, veiligheid en ondersteuning. Daarnaast zijn er bijdrages in de vorm van code en kennis van projecten. Daar wordt soms de afweging gemaakt om functies toe te voegen aan het product, wat significant meer werk kost dan een procesimplementatie oplossing. Echter helpt het toevoegen van functies aan het product uiteindelijk andere projecten weer te versnellen, wat op de lange termijn zijn vruchten afwerpt.&#x20;

### Kan ik bijdragen?&#x20;

Graag! Zoals eerder benoemd is, wordt er constant aan Valtimo GZAC gewerkt en alle bijdragen worden gewaardeerd. Start direct met [https://docs.valtimo.nl/readme/contributing ](https://docs.valtimo.nl/readme/contributing)

### GZAC Goverance – wie stuurt de ontwikkeling?&#x20;

Het beleid voor GZAC wordt gemaakt door de gemeentes die gebruik maken van GZAC. Vanuit dit beleid worden vaak ook bijdragen met code of kennis gecreëerd . De betrokken gemeentes komen eens per kwartaal bijeen. De roadmap is [hier](https://ritense.airfocus.com/share/7e310d940ab2cea996c52ba1d22da03b) te vinden. Ritense heeft de verantwoordelijkheid voor de bewaking van de architectuur en code kwaliteit.
