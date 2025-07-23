# Downloads

## <sup>GZAC met demo proces</sup>

Dit is de volledige instructie voor het lokaal downloaden en installeren van GZAC met het demo proces “Aanvraag Evenementenvergunning”. Het duurt ongeveer 15 minuten. Je kunt daarbij gebruik maken van vier begeleidende video’s voor elke stap.

### Wat je nodig hebt

* Een computer met macOS 11 of hoger, of Windows 10 of hoger
* Een internetverbinding
* Minstens 3 GB vrije schijfruimte
* Vereiste software:
  * macOS: Homebrew, Git, Docker Desktop
  * Windows: Git, Docker Desktop

{% stepper %}
{% step %}
### **GIT Downloaden en installeren**

{% embed url="https://vimeo.com/1087659555?share=copy#t=0" %}
{% endstep %}

{% step %}
### Docker Desktop Downloaden en Installeren

{% embed url="https://vimeo.com/1087670700?share=copy#t=0" %}
{% endstep %}

{% step %}
### GIT Version controle en start Docker Desktop

{% embed url="https://vimeo.com/1087669744?share=copy#t=0" %}
{% endstep %}

{% step %}
### Download en installeer GZAC met demo proces

* Git clone commando:

{% code overflow="wrap" %}
```
git clone https://github.com/generiekzaakafhandelcomponent/gzac-docker-compose.git
```
{% endcode %}

* CD commando

```
cd gzac-docker-compose
```

* Docker compose download en start commando

```
docker compose --profile zgw --profile demo up -d
```

{% embed url="https://vimeo.com/1087671443?share=copy#t=0" %}
{% endstep %}
{% endstepper %}
