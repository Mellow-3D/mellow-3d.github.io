---
title: Fly Gemini V3 Pins
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly Gemini V3 Pin map"
sidebar: mydoc_sidebar
permalink: fly-gemini_v3_pins.html
folder: mydoc
comments: false
toc: true
datatable: true
---
## Fly-Gemini-V3 Pinout Diagram

<a href="https://raw.githubusercontent.com/Mellow-3D/Fly-Gemini-V3/main/Hardware/Gemini_v3_pinout.svg"><img src="https://raw.githubusercontent.com/Mellow-3D/Fly-Gemini-V3/main/Hardware/Gemini_v3_pinout.svg?sanitize=true" /></a>


## Fly-Gemini-V3 Driver Pins in Firmware

Driver pin numbers. They are separated into driver number.

<div class="datatable-begin"></div>

|Pin Type|0 (X)|X Alias|1 (Y)|Y Alias|2 (Z)|Z Alias|3 (E0)|EXT Alias|
| :------------- |:-------------|:-------------|:-------------|:-------------|:-------------|:-------------|:-------------
|Enable Pins|PA3|X_EN|PD2|Y_EN|PC12|Z_EN|PC11|EXT_EN|
|Step Pins|PC13|X_STEP|PC14|Y_STEP|PC15|Z_STEP|PC3|EXT_STEP|
|Direction Pins|PC1|X_DIR|PC4|Y_DIR|PC5|Z_DIRPC12|PC8|EXT_DIR|
|UART Pins|PB11|X_UART|PC10|Y_UART|PB7|Z_UART|PB6|EXT_UART|

<div class="datatable-end"></div>

## Fly-Gemini-V3 Other Pins in Firmware 


<div class="datatable-begin"></div>

|Pin Number|Pin Name 1|Pin Name 2|Alias|
| :------------- |:-------------|:-------------|:-------------|
|PA0|e0heat|he0|HE0|
|PA1|probe||PROBE_1|
|PA10|LCD_RS|RX1|EXP1_4|
|PA13|LCD_EN||EXP1_3|
|PA14|LCD_BTN_EN2||EXP2_5|
|PA15|LCD_BTN_EN1||EXP2_3|
|PA2|bed|hbed|HE1|
|PA7|LCD_CD||EXP2_7|
|PA8|LCD_D5||EXP1_6|
|PA9|LCD_D4|TX1|EXP1_5|
|PB0|servo0|||
|PA4|xstop||LIMIT0|
|PA5|ystop||LIMIT1|
|PA6|zstop||LIMIT2|
|PB1|estop||LIMIT3|
|PB10|LCD_ENC_SW||EXP1_2|
|PB12|LCD_SS||EXP2_4|
|PB13|LCD_SCK||EXP2_2|
|PB14|LCD_MISO||EXP2_1|
|PB15|LCD_MOSI||EXP2_6|
|PC0|e0temp|t0|TH0|
|PC2|bedtemp|tb|TH1|
|PC6|fan0|fan|FAN0|
|PC7|fan1||FAN1||
|PC9|LCD_BEEP||EXP1_1|
|\<NC> |LCD_D6||EXP1_7|
|\<NC> |LCD_D7||EXP1_8|
|\<GND>|LCD_GND||EXP1_9|
|\<5V> |LCD_VCC||EXP1_10|
|\<RST>|LCD_RST||EXP2_8|
|\<GND>|LCD_GND||EXP2_9|
|\<NC> |LCD_KILL||EXP2_10|

<div class="datatable-end"></div>

## ZH TFT Headers

{% include custom/sbc/zh_sockets_datatablev3.html %}