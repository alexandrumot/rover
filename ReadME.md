# Rover
## General Section
![General Section](./img/General-Section.png)
### IsAlive Watchdog
Waits for hello message from ESP32 and updates state accordingly.
### Reset Button
Sends a reset signal when pressed.

## Motors Section
![Motors Section](./img/Motors-Section.png)
Both DC motors are controlled individually with 2 sliders. After I configured the speed control I added a mirror and stop option.

## GPS Section
![GPS Section](./img/GPS-Section.png)
With the help of web-worldmap lib I was able to display the current location using my coordinates as input.

## Logs Section
![Logs Section](./img/Logs-Section.png)
Almost every log I got on the ESP32 I tried to replicate on the Node-Red end. This is crucial in case something in the rover breaks.

## Status Section
![Status Section](./img/Status-Section.png)
On/Off status on sensors and battery.

## InfluxDB Section
![InfluxDB Section](./img/InfluxDB-Section.png)
This section routes sensor logs to InfluxDB server. All data analysis will happen there.

## Libraries Used
- node-red-dashboard
- node-red-contrib-influxdb
- node-red-contrib-web-worldmap