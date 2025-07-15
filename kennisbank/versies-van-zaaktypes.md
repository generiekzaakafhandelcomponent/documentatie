---
description: Hoe om te gaan met versies van Zaaktypes?
---

# Versies van Zaaktypes

Een Dossier in GZAC is gekoppeld aan één versie van een Zaaktype in OpenZaak, zoals hieronder weergegeven:

<figure><img src="../.gitbook/assets/Screenshot 2023-11-09 at 16.28.45.png" alt="GZAC versie 11.1"><figcaption><p>gzac versie 11.1</p></figcaption></figure>

Zaaktypes met dezelfde indentificatie kunnen naast elkaar bestaan indien de data niet overlappen. GZAC is (v11.1) gekoppeld aan een specifieke versie.

<figure><img src="../.gitbook/assets/Screenshot 2023-11-09 at 16.33.58.png" alt=""><figcaption></figcaption></figure>

Hoewel het dossier gekoppeld kan worden aan een nieuwe (versie van) een Zaaktype, betekent dat lopende procesinstancies

Per versie 11.1 biedt GZAC nog geen ondersteuning voor het koppelen van meerdere zaaktype(versies) aan 1 dossier. OpenZaak biedt ook geen ondersteuning voor automatische migratie. Indien de wens bestaat om over te gaan naar een nieuw Zaaktype, kan de leverancier van OpenZaak middels scripts de migratie verzorgen. Punt van aandacht is dat de taken in lopende proces instanties verwijzen naar het oude zaaktype. Deze moeten ofwel worden gemigreerd in BPMN ofwel in OpenZaak dezelfde UUID behouden middels een migratie in OpenZaak.
