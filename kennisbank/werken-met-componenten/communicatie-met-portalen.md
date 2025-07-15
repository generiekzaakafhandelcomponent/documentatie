# Communicatie met portalen

Op deze pagina wordt uitgelegd hoe portalen communiceren met GZAC. Het patroon is universeel, het kan ook worden toegepast voor communicatie tussen andere componenten.

### Wat is een portaal?

Een portaal kan worden ingezet bij processen waar klanten of ketenpartners betrokken zijn. De klant is een inwoner of ondernemer die contact heeft met de gemeente. De ketenpartner is een organisatie die bijdraagt aan het proces van levering van een dienst aan de klant.

<figure><img src="../../.gitbook/assets/Screenshot 2023-05-28 at 17.58.02.png" alt="" width="375"><figcaption></figcaption></figure>

De communicatie met klanten en ketenpartners kan via diverse kanalen verlopen, bijvoorbeeld email, telefoon, chatbot, brieven, de app, fysiek of een portaal. Het portaal (ofwel de 'mijn omgeving') heeft als voordeel boven de andere kanalen dat de communicatie digitaal en gestructureerd verloopt.

### Communicatiepatronen

Er bestaan vier communicatiepatronen tussen GZAC en Portalen.

#### Verzoek (ProductAanvraag)

Het verzoek van een klant voor het leveren van een product of dienst in de breedste zin van het woord. Het kan een vraag zijn of een verzoek iets te leveren, zoals een parkeervergunning of rijbewijs. Ketenpartners doen geen verzoeken, ze dragen bij aan de uitvoering van een verzoek. Een organisatie die ketenpartner is kan in de rol van klant een verzoek doen. In de Haagse referentie architectuur werd ook wel gesproken over ProductAanvraag.

<figure><img src="../../.gitbook/assets/Screenshot 2023-05-28 at 14.34.43.png" alt=""><figcaption></figcaption></figure>

> Voorbeeld: een klant doet een verzoek voor het organiseren van een evenement.

#### Bericht

Het bericht is informatie vanuit de gemeente naar de klant of ketenpartner. Binnen de scope van dit document is dat een bericht vanuit een afhandelcomponent naar een portaal - buiten de scope van dit document wordt een bericht breder gebruikt. Het bericht wordt getoond in een beveiligde omgeving en mag vertrouwelijke informatie bevatten.\
Let op: een email, SMS of Whatapp is in deze context geen bericht. Binnen de context van dit document wordt het sturen van informatie via deze kanalen een notificatie genoemd. Een notificatie mag geen vertrouwelijke informatie bevatten. Een notificatie kan wel melden dat er een bericht beschikbaar is.

<figure><img src="../../.gitbook/assets/Screenshot 2023-05-28 at 14.42.45.png" alt=""><figcaption></figcaption></figure>

> Voorbeeld klantcommuicatie: de gemeente bevestigt de klant dat de aanvraag voor de evenementenvergunning in goede orde is ontvangen.
>
> Voorbeeld ketenpartnercommunicatie: de gemeente verstrekt de notaris aanvullende informatie voor het passeren van een erfpachtcontract.

#### Externe Taak

De externe taak is informatie vanuit de gemeente naar de klant of ketenpartner, met het verzoek een taak uit te voeren. De taak is tweeweg communicatie.

> _\* in de voorlopige API voor Klantinteracties hanteert de VNG de term klanttaak. Dit domein voorziet in taken voor ketenpartners waardoor gewerkt wordt met de bredere term 'externe taak'._ \\

<figure><img src="../../.gitbook/assets/Screenshot 2023-05-28 at 14.57.38.png" alt=""><figcaption></figcaption></figure>

> Voorbeeld klantcommunicatie: de gemeente vraag de klant om een document te uploaden met de kaart van het evenemententerrein.
>
> Voorbeeld ketenpartnercommunicatie: de gemeente vraagt de ketenpartner schade aan straatmeubilair te herstellen en terugmelding te geven na uitvoering.

#### ZaakVerzoek

Het ZaakVerzoek is een verzoek of voorval vanuit de klant of ketenpartner richting de gemeente, binnen de context van een bestaande zaak. Dit scenario komt voor bij langlopende, complexe aanvragen.

<figure><img src="../../.gitbook/assets/Screenshot 2023-05-28 at 15.00.32.png" alt=""><figcaption></figcaption></figure>

> Voorbeeld klantcommunicatie: de klant heeft de behoefte het evenement groter op te zetten, en wil weten of dit kan middels een aanpassing binnen de lopende aanvraag.
>
> Voorbeeld ketenpartnercommunicatie: de partij die trainingen geeft aan minder draagkrachtige inwoners in opdracht van de gemeente, meldt dat een deelnemer drie keer niet is verschenen.
