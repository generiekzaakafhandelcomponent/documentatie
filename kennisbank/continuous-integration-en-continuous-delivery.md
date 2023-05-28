# Continuous Integration en Continuous Delivery

GZAC is gebouwd rondom het concept 'configuratie waar het kan, code waar het moet'-concept. Afhankelijk van de complexiteit kan een proces wordt er in het geheel geen code gebruikt tot scenario's waarin procode teams een oplossing bouwen op het platform. Zie ook de pagina [adopteren vs bouwen](adopteren-vs-bouwen.md).&#x20;

Voor het productiewaardig draaien van processen is een Continuous Integration en Continuous Delivery-omgeving nodig. In 2021 heeft de [Software Improvement Group](https://www.softwareimprovementgroup.com/) in een onderzoek naar OpenZaak en GZAC Valtimo geadviseerd:&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2023-05-28 at 19.46.19.png" alt=""><figcaption></figcaption></figure>

### CI & CD

Het doel van **Continuous Integration** is om een geautomatiseerde manier te creëren voor het ontwerpen en testen van processen. Het versiebeheer, eventuele conflicten in versies en het testen wordt geautomatiseerd gedaan, waardoor de kwaliteit wordt verhoogd.&#x20;

**Continuous delivery** begint waar Continuous Integration eindigt. CD zorgt dat nieuwe versies van processen op de verschillende omgevingen worden uitgerold. In de meeste gevallen wordt gewerkt met acceptatie-, productie- en testomgevingen die elk weer een eigen configuratie hebben. CD zorgt ervoor dat er een geautomatiseerde manier is om codewijzigingen door te voeren naar deze verschillende omgevingen.

CD zorgt er ook voor dat de ontwerpers van processen geen toegang hebben tot de productieomgeving - scheiding van verantwoordelijkheden. Daarnaast wordt gelogd wie en wanneer welke verandering maakt, waarmee het risico op fraude wordt verkleind.&#x20;

<figure><img src="https://lh6.googleusercontent.com/9ogfClsI7xbKYJ25UXcDKXTwJDOLZGwXYGjKxGi50xaWXI_brByEwc-KsPQ96rh9hACs6k3WpwTteYvu-xcuEKyuaB-IJ0HnomouzFCwtyj3MIVGkiFbDpa9IRwZWtt9THvNwpKzLralWlByN6tLEoQSVfZAbK3prMGDKw6fseq47gJa74i2sn63mp3FmA" alt=""><figcaption><p>Alle rechten van <a href="https://silicon-mind.com/what-is-ci-cd-in-devops-continuous/">https://silicon-mind.com/what-is-ci-cd-in-devops-continuous/</a></p></figcaption></figure>

###

