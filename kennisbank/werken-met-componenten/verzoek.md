---
description: De start van een Zaakdossier
---

# Verzoek

Een zaakdossier start naar aanleiding van  'iets wat gebeurt', in BPMN 2.0 termen een '[event](https://www.bpmnquickguide.com/view-bpmn-quick-guide/)'. In de Haagse referentiearchitectuur van het ZGW-landschap wordt het event op basis waarvan een zaakdossier kan worden gestart een 'verzoek' genoemd.&#x20;

Het verzoek is zelf geen onderdeel van een zaakdossier, er is immers nog geen zaakdossier op het moment dat het event plaatsvindt. Het verzoek kan wel worden toegevoegd aan het zaakdossier, zodat de oorsprong van het zaakdossier herleidbaar is.&#x20;

{% hint style="info" %}
Het Verzoek wordt ook wel ProductAanvraag genoemd. Deze term is de oorspronkelijke naam in de Haagse referentiearchitectuur. We hanteren bijvoorkeur de term 'verzoek', omdat een Zaakdossier niet altijd tot een Product leidt.&#x20;
{% endhint %}

### Wie doet een Verzoek?

Het verzoek wordt gedaan door een klant, voor het leveren van een product of dienst in de breedste zin van het woord. Het kan een vraag zijn of een verzoek iets te leveren, zoals een parkeervergunning of rijbewijs. Ketenpartners doen geen verzoeken, ze dragen bij aan de uitvoering van een verzoek. Een organisatie die ketenpartner is kan in de rol van klant een verzoek doen.

### Van Verzoek tot Zaakdossier

In het ZGW-landschap wordt bijvoorkeur gebruik gemaakt van informatie-arm notificeren, zoals beschreven in de [informatiearchitectuurprincipes van de VNG](https://componentencatalogus.commonground.nl/20190130\_-\_Common\_Ground\_-\_Informatiearchitectuurprincipes.pdf). Het werken met notificaties zorgt voor het ontkoppelen van systemen, in dit geval veelal een [formulierencomponent](https://www.gemmaonline.nl/index.php/GEMMA2/0.9/id-5c9f683b-4454-4e3e-b93c-da50dfd6934a) en GZAC. Dit principe staat uitgelegd op de pagina [Integratiepatronen](https://gzac.gitbook.io/product-docs/kennisbank/werken-met-componenten/integratiepatronen).&#x20;

Meerdere componenten kunnen verzoeken kunnen aanmaken. Dat ondersteunt de volgende scenario's:&#x20;

* meerdere soorten formulierencomponenten van verschillende leveranciers maken verzoeken aan, bijvoorbeeld in een 'nieuw-naast-oud' situatie;&#x20;
* een zaakafhandelcomponentent verzoekt een ander zaakafhandelcomponent een subzaak uit te voeren;
* een chatbot of een scanstraat maakt een verzoek aan.&#x20;

### **Formattering van een verzoek**

Uitgangspunt is dat het verzoek in JSON-formaat wordt gemaakt. De waardes uit het verzoek worden via een mapping geplaatst op de juiste locatie in GZAC, in praktijk het vooral het zaakdetailobject. Er kan ook gekozen worden het gehele verzoek op te nemen in het zaakdetailobject.&#x20;

<figure><img src="../../.gitbook/assets/Screenshot 2023-06-16 at 14.37.06.png" alt=""><figcaption><p>mapping van waardes uit het verzoek naar het zaakdetailobject</p></figcaption></figure>

### Het verzoek toevoegen aan het Zaakdossier

Om na te gaan wat de aanleiding van een Zaakdossier was, kan het verzoek worden toegevoegd aan het zaakdossier. Er zijn meerdere mogelijkheden dit te doen.&#x20;

1. Sommige formulierencomponenten zijn in staat het verzoek in PDF mee te leveren. Het veel toegepaste OpenFormulieren plaatst het verzoek in PDF-formaat in de Documenten API en levert de link naar dit document mee. Deze link wordt door GZAC verwerkt, zodat het document een zaakinformatieobject wordt in de Zaak - praktisch veelal OpenZaak. Het document is dan inzichtelijk in GZAC onder de documententab.&#x20;

<figure><img src="../../.gitbook/assets/Screenshot 2023-06-16 at 14.46.50.png" alt=""><figcaption><p>het verzoek in PDF vanuit het formulierencomponent OpenFormulieren, in de Documenten API, binnen een Zaakdossier</p></figcaption></figure>

2. De informatie vanuit het verzoek kan in zijn geheel worden opgenomen in het zaakdetailobject.
3. Het verzoek wordt geplaatst in de Objects API en na verwerking verwijderd. Dit is het principe achter informatie-arm notificeren, nadat het bericht succesvol is overgebracht wordt het vernietigd, waarmee dataduplicatie wordt voorkomen (immers, alle inhoud van het verzoek is verwerkt in het zaakdossier). Het is ook mogelijk om het bericht te bewaren, en te linken als zaakobject in OpenZaak. Dit wordt gedaan in het systeemproces dat de verzoekenplugin gebruikt. Dit wordt weergegeven in de laatste stap van het systeemproces, deze kan worden verwijderd of aangepast.&#x20;

<figure><img src="../../.gitbook/assets/Screenshot 2023-06-16 at 14.53.22.png" alt=""><figcaption><p>systeemproces dat onder de verzoekenplugin draait</p></figcaption></figure>

