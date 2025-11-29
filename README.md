### How to run code on Pi + Chromium kiosk mode

## Start PI in desktop mode

```shell
sudo rasp-config

```
`System Options` -> `Boot` -> `Desktop Desktop GUI`


## Install `snap`

```shell
sudo apt install snapd

```

## Install `chromium`

```shell
sudo snap install chromium

```

## Run chromium in kiosk mode

chromium --kiosk --disable-infobars "https://skeckulous.github.io/TVSTudio-Map/maptest-prototype.html"

CTRL-W to exit kiosk mode

## How to communicate with node-red via mosquitto websockets interface

### Create a mosquitto websockets endpoint.

Below a minimal mosquitto.conf file

```
listener 1883
protocol mqtt
allow_anonymous true

listener 9001
protocol websockets
allow_anonymous true

```

### Connect the Web frontend to mosquitto

We use a library called [paho](https://github.com/eclipse-paho/paho.mqtt.javascript) that enables web applications to connect to the mosquitto MQTT broker using WebSockets

You can find an example in:

https://stackoverflow.com/questions/70128563/mosquitto-and-simple-paho-js-client



