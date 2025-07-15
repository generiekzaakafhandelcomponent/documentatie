# Werken met componenten

Een Common Ground architectuur is opgebouwd uit componenten. Het idee is gebaseerd op de [microservice architectuur](https://microservices.io/). Elk component is verantwoordelijk voor een domein, bijvoorbeeld 'facturatie', 'authenticatie' of natuurlijk 'zaakafhandeling'. Voordelen van deze architectuur zijn:

1. De componenten zijn individueel vervangbaar. Er kan worden gewisseld van oplossing A naar B, zonder dat omliggende componenten vervangen hoeven worden. Dat vermindert de lockin op een oplossing.
2. Vrijheid in keuze. Een component kan in elke taal en technologie gemaakt zijn. Er is geen noodzaak om alle componenten van één platform, taal, techniek of leverancier te kiezen.
3. Centralisatie en deduplicatie van functies. Het maken van brieven kan bijvoorbeeld worden belegd bij één component, in plaats van in elke individuele softwareoplossing - wat er voor zorgt dat taal- en huisstijlgebruik centraal wordt geborgd.
4. Schaalbaarheid en betrouwbaarheid. Als één component niet goed fungeert, hoeft dat geen invloed te hebben op de andere componenten. Als voorbeeld, klanten kunnen blijven communiceren via het portaal als de brievengenerator niet beschikbaar is.

De microservice architectuur heeft ook nadelen, de voornaamste is dat ze complexer is dan de monolitische architectuur. Naast dat de componenten zelfstandig goed moeten fungeren is de uitdaging ze als geheel goed te laten werken.

### GZAC als component in het ZGW-landschap

Het zaakafhandelcomponent is één van de componenten in het ZGW-landschap. Er kunnen er meerdere bestaan in een landschap, bijvoorbeeld taakspecifieke en generieke componenten, of meerdere installaties van een generiek component.

Het zaakafhandelcomponent communiceert met andere componenten, zoals bijvoorbeeld portalen, systemen voor gebruikersauthenticatie, financiele systemen, email services, BRK, BRP en vele anderen.

De koppeling tussen GZAC en andere componenten wordt gelegd via [Plugins](broken-reference/).

###
