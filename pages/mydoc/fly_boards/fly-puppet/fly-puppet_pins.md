---
title: Fly-Puppet Pin Names
tags: []
keywords: 
last_updated: 18/05/2022
summary: "The pin names of the Fly-Puppet"
sidebar: mydoc_sidebar
permalink: fly-puppet_pins.html
folder: mydoc
comments: false
toc: false
datatable: true
---

## Fly-Puppet Pinout Diagram

{% include image.html 
file="fly-puppet/fly-puppet_pins.webp" 
url="./images/fly-puppet/fly-puppet_pins.webp" alt="Fly-Puppet" 
caption="Fly-Puppet Pinout" %}

<a href="https://github.com/Mellow-3D/Fly-Puppet/blob/main/Hardware/fly_puppet_pinout.svg"><img src="https://raw.githubusercontent.com/Mellow-3D/Fly-Puppet/main/Hardware/fly_puppet_pinout.svg?sanitize=true"></a>

## Fly-Puppet Driver Pins in Firmware

Driver pin numbers. They are separated by driver number.

<div class="datatable-begin"></div>

|Pin Type|0 (X)|1 (Y)|2 (Z)|3 (E0)|4 (E1)|
| :------------- |:-------------|:-------------|:-------------|:-------------|:-------------|
|Enable Pins|gpio18|gpio14|gpio10|gpio6|gpio2|
|Step Pins|gpio20|gpio16|gpio12|gpio8|gpio4|
|Direction Pins|gpio19|gpio15|gpio11|gpio7|gpio13|
|UART Pins|gpio21|gpio17|gpio13|gpio9|gpio5|

<div class="datatable-end"></div>

## Fly-Puppet Other Pins in Firmware 

<div class="datatable-begin"></div>

|Pin Number|Pin Name 1|Pin Name 2|Alias|
| :------------- |:-------------|:-------------|:-------------|
|gpio26|bed|hbed|BED_OUT|
|gpio22|xmin|xstop|X_STOP|
|gpio29|bedtemp|tb|BED_TEMP|
|gpio28|e0temp|t0|HEAT_TEMP|
|gpio27|e0heat|he0|HEAT|
|host:gpio21|fan1||FAN1|
|host:gpio20|fan2||FAN2|
|gpio25|fan0|fan|FAN0|
|host:gpio16|servo0||SERVO|
|gpio23|ymin|ystop|Y_STOP|
|host:gpio19|neopixel|RGB|LED|
|host:gpio20|fan2||FAN2|
|gpio24|zmin|zstop|Z_STOP|
|gpio24|probe||PROBE|

<div class="datatable-end"></div>