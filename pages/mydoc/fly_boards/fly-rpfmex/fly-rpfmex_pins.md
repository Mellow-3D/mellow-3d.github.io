---
title: Fly-RPFMEX Pin Names
tags: []
keywords: 
last_updated: 18/05/2022
summary: "The pin names of the Fly-RPFMEX"
sidebar: mydoc_sidebar
permalink: fly-rpfmex_pins.html
folder: mydoc
comments: false
toc: true
datatable: true
---

## Fly-RPFMEX Pinout Diagram

{% include image.html 
file="fly-rpfmex/fly-rpfmex_pins.webp" 
url="./images/fly-rpfmex/fly-rpfmex_pins.webp" alt="Fly-rpfmex" 
caption="Fly-rpfmex Pinout" %}

## Fly-RPFMEX Driver Pins in Firmware

Driver pin numbers. They are separated by driver number.

<div class="datatable-begin"></div>

|Pin Type|0 (X)|1 (Y)|2 (Z)|3 (E0)|
| :------------- |:-------------|:-------------|:-------------|:-------------|
|Enable Pins|GPIO9|GPIO4|GPIO25|GPIO20|
|Step Pins|GPIO6|GPIO1|GPIO22|GPIO17|
|Direction Pins|GPIO5|GPIO0|GPIO21|GPIO16|
|UART Pins|GPIO7|GPIO2|GPIO23|GPIO18|
|Diag Pins|GPIO8|GPIO3|GPIO24|GPIO19|

<div class="datatable-end"></div>

## Fly-rpfmex Other Pins in Firmware 

<div class="datatable-begin"></div>

|Pin Number|Pin Name 1|Pin Name 2|Alias|
|Pin Number|Pin Name 1|Pin Name 2|Alias|
| :------------- |:-------------|:-------------|
|GPIO27|xmin|xstop|X_STOP|
|GPIO12|fan1|fan1|FAN1|
|GPIO11|fan0|fan|FAN|
|GPIO28|ymin|ystop|Y_STOP|
|GPIO10|neopixel|LED|
|GPIO29|zmin|zstop|Z_STOP|


<div class="datatable-end"></div>