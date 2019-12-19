# ansible role to install mqtt-tempo

## How to run it

create a playbook and setup on your inventory variables:

| ansible variable | environment variable | default |
|------------------|----------------------|---------|
| tempo_url | TEMPO_URL | https://particulier.edf.fr/bin/edf_rc/servlets/ejptemponew?Date_a_remonter=%s&TypeAlerte=TEMPO |
| tempo_mqtt_url | TEMPO_MQTT_URL | tcp://localhost:1883 |
| tempo_mqtt_login| TEMPO_MQTT_LOGIN | "" |
| tempo_mqtt_password | TEMPO_MQTT_PASSWORD | "" |

they will be replaced by the corresponding environment variable thanks to the systemctl service.

For more details about the variable, check https://bitbucket.org/mbee/go-mqtt-tempo
