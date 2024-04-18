# Releases

### GZAC Valtimo v12.0 - coming soon!

In deze release komt de takenlijst filter feature uit, waarbij je zelf kan kiezen op welke eigenschappen je de taken wilt filteren. Ook kan je de takenlijst filteren op het type dossier.&#x20;

### GZAC Valtimo v11.2

5 april 2023: release 11.2.0 is uit. In deze nieuwe release zijn een aantal nieuwe features beschikbaar, waaronder het kunnen importeren en exporteren van dossier definities vanuit een ZIP archief. Verder worden nu ook Keycloak groepsrollen ondersteund in de Access control feature, importeren van een geëxporteerde document definitie én zie je nu ook de versie van het proces op de 'progress' tab van een dossier. Zie voor de volledige lijst [hier](https://docs.valtimo.nl/release-notes/11.x.x/11.2.0/valtimo-backend-libraries) en [hier](https://docs.valtimo.nl/release-notes/11.x.x/11.2.0/valtimo-frontend-libraries).&#x20;

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

30 januari 2023_._ Release 10.2 is beschikbaar! Nieuw in deze tweede release van 2023:

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
