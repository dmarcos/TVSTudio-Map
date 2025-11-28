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

https://stackoverflow.com/questions/70128563/mosquitto-and-simple-paho-js-client

