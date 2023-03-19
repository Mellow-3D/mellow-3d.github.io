---
title: Fly Gemini V2 Pins
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly Gemini V2 Pin map"
sidebar: mydoc_sidebar
permalink: fly-gemini_v2_pins.html
folder: mydoc
comments: false
toc: true
datatable: true
---
## Fly-Gemini-V2 Pinout Diagram

{% 
include image.html 
file="fly-gemini-v2/gemini_v2_pins.png" 
url="images/fly-gemini-v2/gemini_v2_pins.png" 
alt="Fly-Gemini-V2 pins" 
caption="Fly-Gemini-V2 Pinout" 
%}


{% 
include image.html 
file="fly-gemini-v2/PCB_Geminiv2_2022-11-23.svg" 
url="images/fly-gemini-v2/PCB_Geminiv2_2022-11-23.svg" 
alt="Fly-Gemini-V2 pins" 
caption="Fly-Gemini-V2 Pins" 
%}


## Fly-Gemini-V2 Driver Pins in Firmware

Driver pin numbers. They are separated into driver number.

<div class="datatable-begin"></div>

|Pin Type|0 (X)|X Alias|1 (Y)|Y Alias|2 (Z)|Z Alias|3 (E0)|EXT Alias|
| :------------- |:-------------|:-------------|:-------------|:-------------|:-------------|:-------------|:-------------
|Enable Pins|PB2|X_EN|PD2|Y_EN|PC12|Z_EN|PC11|EXT_EN|
|Step Pins|PC13|X_STEP|PC14|Y_STEP|PC15|Z_STEP|PC3|EXT_STEP|
|Direction Pins|PC1|X_DIR|PC4|Y_DIR|PC5|Z_DIR|PC8|EXT_DIR|
|UART Pins|PB11|X_UART|PB9|Y_UART|PB8|Z_UART|PB7|EXT_UART|

<div class="datatable-end"></div>

## Fly-Gemini-V2 Other Pins in Firmware 

<div class="datatable-begin"></div>

|Pin Number|Pin Name 1|Pin Name 2|Alias|
| :------------- |:-------------|:-------------|:-------------|
|PA0|e0heat|he0|HE0|
|PA1|probe||PROBE_1|
|PA10|LCD_RS|RX1|EXP1_4|
|PA13|LCD_EN||EXP1_3|
|PA14|LCD_BTN_EN2|BTN_EN2|EXP2_5|
|PA15|LCD_BTN_EN1|BTN_EN1|EXP2_3|
|PA2|bed|hbed|HE1|
|PA3|xstop||LIMIT0|
|PA4|LCD_ENC_SW|BTN_ENC|EXP1_2|
|PA8|LCD_D5||EXP1_6|
|PA9|LCD_D4|TX1|EXP1_5|
|PB0|servo0|||
|PB1|ystop||LIMIT1|
|PB7|
|PB10|zstop||LIMIT2|
|PB12|LCD_SS||EXP2_4|
|PB13|LCD_SCK||EXP2_2|
|PB14|LCD_MISO||EXP2_1|
|PB15|LCD_MOSI||EXP2_6|
|PB3|LCD_CD||EXP2_7|
|PC0|e0temp|t0|TH0|
|PC2|bedtemp|tb|TH1|
|PC6|fan0|fan|FAN0|
|PC7|fan1||FAN1|
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

{% include custom/sbc/zh_sockets_datatable.html %}