# Modelleren met het Zaakdetailobject

Het zaakdetailobject is het belangrijkste object in GZAC Zaakdossiers. Het is object is het hart van de Zaak. Het object is technisch niet anders dan andere objecten, het is een JSON-object. Er is maximaal 1 Zaakobject per Zaakdossier. Het Zaakdetailobject wordt primair opgeslagen in de GZAC database, en (indien ingesteld) bij elke wijziging gesynchroniseerd naar een Objects API.&#x20;

De gegevens in het Zaakdetailobject zijn (voor zover rechten zijn verstrekt) toegankelijk voor elke applicatie in het ZGW-landschap.&#x20;

#### Welke data hoort niet thuis in het Zaakobject?

* Gegegevens uit [basisregistraties](https://www.digitaleoverheid.nl/overzicht-van-alle-onderwerpen/stelsel-van-basisregistraties/10-basisregistraties/). Het principe is dat deze gegevens zo min mogelijk worden gedupliceerd. Ze worden realtime opgehaald zodra ze nodig zijn. Uitzonderingen op deze regel:&#x20;
  * Als er de wens is een 'foto' te maken van de situatie in tijd, de situatie vast te leggen zoals deze op een bepaald moment is. Praktisch voorbeeld is het woonadres ten tijde van een aanvraag. In dit geval worden de gegevens gekopieerd naar het zaakdetailobject.&#x20;
  * Als de wens te filteren op gegevens of ze in de lijstschermen te tonen. Als voorbeeld, als de Achternaam van een aanvrager moet worden getoond in het lijstscherm, wordt dit gegeven opgenomen in het zaakdetailobject.&#x20;
* Gegevens uit andere registraties.&#x20;
* Technische ofwel 'stuurinformatie'. Daarvoor zijn process variables beschikbaar. Als voorbeeld de ID van een printopdracht.&#x20;

#### Best practise / goede gewoontes

* Maak altijd een JSON schema. Een JSON schema dwingt een bepaalde kwaliteit van elk document af. De ervaring leert dat voor productiewaardige systemen een JSON schema nodig is.&#x20;
* Zorg voor een stabiel ontwerp en wijzig het model zo min mogelijk. Bespreek de impact van wijzigingen goed voor ze door te voeren. Als voorbeeld, als in een v2 van het schema een atribuut verplicht wordt gesteld dat in v1 nog niet verplicht was, moeten de formulieren die deze gegevens leveren ook worden aangepast.&#x20;
* &#x20;Het Zaakdetail moet bruikbaar zijn voor Formio formulieren. Complexiteiten zoals arrays in arrays kan de bouwer van formulieren frustreren. Tip: neem niet klakkeloos een JSON schema over van een bron.&#x20;
