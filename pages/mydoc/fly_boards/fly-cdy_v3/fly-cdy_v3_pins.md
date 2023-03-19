---
title: Fly-CDY V3 Pin Names
tags: []
keywords: 
last_updated: 18/05/2022
summary: "The pin names of the Fly-CDY V3"
sidebar: mydoc_sidebar
permalink: fly-cdy_v3_pins.html
folder: mydoc
comments: false
toc: false
datatable: true
---

## Fly-CDY V3 Pinout Diagram

<a href="https://github.com/Mellow-3D/Fly-CDYv3/blob/main/Hardware/pins.svg"><img src="https://raw.githubusercontent.com/Mellow-3D/Fly-CDYv3/d02f482a1c9e2bf6f6ddf2493f6be83915802c45/Hardware/pins.svg?sanitize=true"></a>


## Fly-CDY V3 Driver Pins in Firmware

Driver pin numbers. They are separated by driver number.

<div class="datatable-begin"></div>

|Pin Type|0 (X)|1 (Y)|2 (Z)|3 (E0)|4 (E1)|5 (E2)|
|:------------- |:-------------|:-------------|:-------------|:-------------|:-------------|:-------------|
|Step Pins|PE5 |PE4|PE3 |PE2|PE1|PD0|
|Direction Pins|PC0|PC13|PB7|PD6|PD3|PA15|
|Enable Pins|PC1|PC14|PB8 |PD7|PD4 |PD0|
|UART Pins|PC15|PE8|PB6 |PD5|PD1|PE9|

<div class="datatable-end"></div>

## Fly-CDY V3 Other Pins in Firmware 

<div class="datatable-begin"></div>

|Pin Number|Pin Name 1|Pin Name 2|Alias
| :------------- |:-------------|:-------------|:-------------|
|PB0|bed|hbed|BED_OUT|
|PB1|bedtemp|tb|BED_TEMP|
|PC7|x-min|xstop|X_STOP|
|PD11|y-min|ystop|Y_STOP|
|PB10|z-min|zstop|Z_STOP|
|PC6|x-max|e0stop|E_STOP|
|PD10|y-max|e1stop|E1_STOP|
|PB11|z-max|e2stop|E2_STOP|
|PA3|e0temp|t0|HEAT_TEMP|
|PC4|e1temp|t1|HEAT1_TEMP|
|PC5|e2temp|t2|HEAT2_TEMP|
|PD12|e0heat|he0|HEAT|
|PD13|e1heat|he1|HEAT1|
|PD14|e2heat|he2|HEAT2|
|PA0|fan0|fan|FAN0|
|PA1|fan1||FAN1|
|PA2|fan2||FAN2|
|PB9|laser|||
|PD15|neopixel|||
|PC2|probe||PROBE|
|PE6|servo0||SERVO|
|\<NC>|LCD_BEEP||EXP1_1|
|PA9|LCD_BTN_ENC|ENC_SW|EXP1_2|
|PB2|LCD_EN||EXP1_3|
|PA10 |LCD_RS||EXP1_4|
|PE15|LCD_D4||EXP1_5|
|PE14|LCD_D5||EXP1_6|
|PA13|LCD_D6||EXP1_7|
|PA14|LCD_D7||EXP1_8|
|\<GND>|GND||EXP1_9|
|\<5V>|VCC||EXP1_10|	 
|PA6|LCD_MISO||EXP2_1|
|PA5|LCD_SCK||EXP2_2|
|PD8|LCD_BTN_EN1|RX1|EXP2_3|
|PA4|LCD_SS||EXP2_4|
|PD9|LCD_BTN_EN2|TX1|EXP2_5|
|PA7|LCD_MOSI||EXP2_6|
|PE13|LCD_CD||EXP2_7|
|\<RST>|RST||EXP2_8|
|\<GND>|GND||EXP2_9|
|\<NC>|KILL||EXP2_10|


<div class="datatable-end"></div>