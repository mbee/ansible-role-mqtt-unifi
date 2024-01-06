# ansible role to install mqtt-tempo

## How to run it

create a playbook and setup on your inventory variables:

| ansible variable    | environment variable | default              | comment                        |
| ------------------- | -------------------- | -------------------- | ------------------------------ |
| unifi_mqtt_url      | MQTT_URL             | tcp://localhost:1883 | mqtt url to connect to         |
| unifi_mqtt_login    | MQTT_LOGIN           | ""                   | mqtt login                     |
| unifi_mqtt_password | MQTT_PASSWORD        | ""                   | mqtt password                  |
| unifi_mqtt_name     | MQTT_NAME            | mqtt_unifi_v103      | mqtt client name               |
| unifi_host          | UNIFI_HOST           | localhost            | unifi server url to connect to |
| unifi_user          | UNIFI_USER           |                      | unifi user                     |
| unifi_pass          | UNIFI_PASS           |                      | unifi password                 |
| unifi_version       | UNIFI_VERSION        |                      | unifi version                  |
| unifi_port          | UNIFI_PORT           |                      | unifi port                     |
| unifi_site_id       | UNIFI_SITE_ID        |                      | unifi site id                  |
| unifi_delay         | UNIFI_DELAY          |                      | unifi delay                    |

they will be replaced by the corresponding environment variable thanks to the systemctl service.

For more details about the variable, check https://github.com/mbee/mqtt-unifi
