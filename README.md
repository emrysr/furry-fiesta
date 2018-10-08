# JS MQTT Client 
Uses [paho-mqtt](https://www.eclipse.org/paho/clients/js/) to create a connection
with a MQTT server via WebSockets.

Open index.html and view the on-screen instructions to connect
and subscribe to topics on the connected server

You'll have to use your own mqtt server.


# TL;DR

## install localhost mqtt server
```
$ node install mqtt -g
```

## pub/sub with locally installed mqtt server
```
$ mqtt sub -t topic
```
```
$ mqtt pub -t topic -m message
```

## testing mqtt server
you can test your mqtt connections using mosquitto's servers:
> [https://test.mosquitto.org/](https://test.mosquitto.org/)

## ports and connection types:
| port | protocol                                     |
|------|----------------------------------------------|
| 1883 | MQTT, unencrypted                            |
| 8883 | MQTT, encrypted                              |
| 8884 | MQTT, encrypted, client certificate required |
| 8080 | MQTT over WebSockets, unencrypted            |
| 8081 | MQTT over WebSockets, encrypted              |
