---
title: Fly-E3-Pro-v3 Pin Names
tags: []
keywords: 
last_updated: 18/05/2022
summary: "The pin names of the Fly-E3-Pro-v3"
sidebar: mydoc_sidebar
permalink: fly-e3_pro_v3_pins.html
folder: mydoc
comments: false
toc: false
datatable: true
---

## Fly-E3-Pro-v3 Pinout Diagram

{% include image.html 
file="fly-e3_pro_v3/fly_e3_prov3_pins.svg" 
url="https://raw.githubusercontent.com/Mellow-3D/Fly-E3-Pro-v3/main/Hardware/fly_e3_prov3_pins.svg" alt="Fly-E3-Pro-v3" 
caption="Fly-E3-Pro-v3 Pinout" %}

## Fly-E3-Pro-v3 Driver Pins in Firmware

Driver pin numbers. They are separated by driver number.

<div class="datatable-begin"></div>

|Pin Type|0 (X)|1 (Y)|2 (Z)|3 (E0)|4 (E1)|
| :------------- |:-------------|:-------------|:-------------|:-------------|:-------------|
|Enable Pins|PE5|PE1|PC2|PD6|PC15|
|Step Pins|PE3|PB9|PA15|PD4|PC13|
|Direction Pins|PE2|PB8|PD7|PD3|PC0|
|UART Pins|PE4|PE0|PA8|PD5|PC14|

<div class="datatable-end"></div>

## Fly-E3-Pro-v3 Other Pins in Firmware 

<div class="datatable-begin"></div>

|Pin Number|Pin Name 1|Pin Name 2|
| :------------- |:-------------|:-------------|
|PA0|bed|hbed|
|PA1|e1temp|t1|
|PA10|RX1|BTN_EN1|
|PA13|LCD_CD||
|PA14|LCD_EN||
|PA2|xmin|xstop|
|PA3|bedtemp|tb|
|PA4|e0temp|t0|
|PA5|e0heat|he0|
|PA6|fan1||
|PA7|fan0|fan|
|PA9|TX1|BTN_EN2|
|PB0|servo0||
|PB1|laser||
|PB10|ymin|ystop|
|PB11|neopixel||
|PB2|LCD_SS||
|PB3|LCD_SCK||
|PB4|LCD_MISO||
|PB5|LCD_MOSI||
|PB6|fan2||
|PB7|fan3||
|PC1|boardtemp|tboard|
|PC4|zmin|zstop|
|PC5|probe||
|PC6|e1heat|he1|
|PD0|e0min|e0stop|
|PD1|e1min|e1stop|
|PD10|pwr|PWRDET|
|PD11|PSON||
|PE10|LCD_D5||
|PE11|BEEP||
|PE12|BTN_ENC||
|PE6|LCD_RS||
|PE7|LCD_D6||
|PE8|LCD_D7||
|PE9|LCD_D4||


<div class="datatable-end"></div>