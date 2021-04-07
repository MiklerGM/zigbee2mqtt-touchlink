# zigbee2mqtt-assistant

This setup was born while I was looking how to reset my Philips Hue Play Bar (or any Philips Bulb) without use of a dimmer.

I found that it was possible to reset a Zigbee bulb using [touchlink](https://www.zigbee2mqtt.io/information/touchlink.html) feature [(original ticket)](https://github.com/Koenkk/zigbee2mqtt/issues/2396).

I was lucky enough and I had a TI CC2531 USB Zigbee Stick at hand, so I was able to proceed.

This docker-compose file will set up zigbee2mqtt with ui
- [zigbee2mqtt](https://www.zigbee2mqtt.io)
- [mosquito](https://mosquitto.org/)
- [zigbee2mqttAssistant](https://github.com/yllibed/Zigbee2MqttAssistant)

*Huge thanks to authors of this software*

## How to Use
Configure device in docker-compose.yml and configuration.yaml files

Run
```
docker-compose up
```
Open http://localhost:8880/ and navigate to status

![zigbee2mqtt UI](https://raw.githubusercontent.com/MiklerGM/zigbee2mqtt-touchlink/main/zigbee2mqttAssistant.png "Assistant UI and Touchlink button")


## Articles and documentation

https://www.zigbee2mqtt.io/information/docker.html

https://thesmarthomejourney.com/2020/05/11/guide-zigbee2mqtt/

https://thesmarthomejourney.com/2021/01/13/zigbee2mqttassistant/

https://medium.com/swlh/using-docker-compose-to-build-zigbee-infrastructure-336983a6ad67