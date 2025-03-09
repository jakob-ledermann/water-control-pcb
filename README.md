# Introduction

This is my first PCB Design.
It is intended to use an ESP32-H2-mini-1 to measure the humidity of the soil with capacitive sensors `DEBO CAP SENS` and control the power to a watering pump.
The pump used is from the [Gardena Holiday set](https://www.gardena.com/de/produkte/bewaesserung/urlaubsbewaesserung/urlaubsbewaesserung-set/970548801.html) and operating at
14V DC using 30VA according to the labels on the pump.

Power for the ESP32 is obtained from the 15V DC Power for the pump so you only need to connect a 15V DC Powersupply to run the whole thing.

The ESP32-H2 is used as it supports Zigbee and Matter more or less of the shelf.

The USB-Port is provided so the ESP32-H2 can be flashed directly.
All GPIOs of the ESP32-H2 are exposed to headers so it is possible to expand the usages.

## Design process

During the design process I basically selected core components and slapped the recommended support components on there.
There is no ESD Protection on the Power input.
The sensors I ordered for this project require 5V DC to Power themselves.

The design is created using [EasyEDA 6.5.46](https://easyeda.com/page/download)