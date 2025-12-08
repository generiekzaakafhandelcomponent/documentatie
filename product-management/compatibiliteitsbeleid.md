# Compatibiliteitsbeleid

## Compatibiliteitsbeleid

Deze policy beschrijft hoe GZAC omgaat met backward compatibility en welke onderdelen van het product stabiele contracten vormen. Het doel is om ontwikkelaars, implementatiepartners en beheerders te beschermen tegen onverwachte breuken bij upgrades, terwijl we ruimte houden voor gecontroleerde innovatie.

***

### Doel

Dit beleid heeft drie doelen:

1. **Voorspelbaarheid:** Gebruikers kunnen veilig upgraden zonder dat bestaande implementaties breken.
2. **Transparantie:** Eventuele breaking changes worden vooraf aangekondigd en gedocumenteerd.
3. **Beheersbaarheid:** Alleen expliciet gemarkeerde stabiele interfaces vallen onder deze garantie.

***

### Stabiele onderdelen

De volgende onderdelen worden als **stabiel** beschouwd. Breaking changes in deze onderdelen worden **niet zonder major release** geïntroduceerd:

#### 1. REST API

* De REST API’s van GZAC volgen semantische versiebeheer.
* Nieuwe velden kunnen worden toegevoegd (backward compatible).
* Bestaande endpoints, velden of response formats worden niet gewijzigd of verwijderd binnen een minor release.
* Wijzigingen aan endpoints kunnen in een minor release worden geïntroduceerd met behulp van API versioning. Bijvoorbeeld: `/api/v2/endpoint/path`&#x20;

#### 2. Configuratiebestanden

* JSON-configuraties (zoals dossier definities en formulieren) behouden hun structuur.
* Nieuwe configuratie-opties (velden kunnen worden toegevoegd.
* Bestaande keys of semantiek worden alleen gewijzigd bij een major release.

#### 3. Outbox Events (CloudEvents)

* De Outbox-eventstructuur en de bijbehorende CloudEvent-velden blijven stabiel.
* Nieuwe eventtypes of attributen kunnen worden toegevoegd.

#### 4. Custom Frontend Widgets & Tabs

* Het mechanisme voor het registreren en gebruiken van custom widgets en tabs in de frontend is stabiel.
* Breaking changes in Angular of build tooling worden alleen doorgevoerd bij een major release.

#### 5. Applicatieconfiguratie

* Environment variabelen en `application.yaml` properties blijven stabiel.
* Sleutels worden niet hernoemd of verwijderd zonder migratiepad.
* Nieuwe configuratie-opties kunnen worden toegevoegd zonder impact op bestaande omgevingen.

***

### Niet-stabiele onderdelen

De volgende onderdelen vallen **niet** onder de breaking change garantie:

* Interne API’s, zoals service classes
* Feature-flags, previews of experimenten
* Interne database-tabellen en queries
* Niet-gedocumenteerde configuratie-opties
* UI-styling en CSS selectors

***

### Breaking Changes

Wanneer een breaking change noodzakelijk is:

* Wordt deze aangekondigd in de release notes.
* Wordt er, waar mogelijk, een migratiepad of fallback aangeboden.
* Wordt het versienummer verhoogd volgens semver (major).
