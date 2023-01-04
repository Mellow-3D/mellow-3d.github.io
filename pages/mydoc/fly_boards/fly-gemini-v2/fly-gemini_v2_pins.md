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
toc: false
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
|Enable Pins|B.2|X_EN|D.2|Y_EN|C.12|Z_EN|C.11|EXT_EN|
|Step Pins|C.13|X_STEP|C.14|Y_STEP|C.15|Z_STEP|C.3|EXT_STEP|
|Direction Pins|C.1|X_DIR|C.4|Y_DIR|C.5|Z_DIR|C.8|EXT_DIR|
|UART Pins|B.11|X_UART|B.9|Y_UART|B.8|Z_UART|B.7|EXT_UART|

<div class="datatable-end"></div>

## Fly-Gemini-V2 Other Pins in Firmware 

If more than one pin name is availble, either name can be used in the firmware (config.g).  
If the pins aren't in the table (due to not having a special name), then the pin itself can be used in the form of PA0, PA.0, PA_0, A0, A.0 or A_0.  

<div class="datatable-begin"></div>

|Pin Number|Pin Name 1|Pin Name 2|Alias|PWM Hardware Timer|
| :------------- |:-------------|:-------------|:-------------|:-------------|
|A.0|e0heat|he0|HE0|Timer 2|
|A.1|probe||PROBE_1|Timer 2|
|A.10|RX1||||
|A.13|LCD_EN|||
|A.14|BTN_EN2||||
|A.15|BTN_EN1|||Timer 2|
|A.2|bed|hbed|HE1|Timer 2|
|A.3|xstop||LIMIT0|Timer 2|
|A.4|BTN_ENC||||
|A.8|LCD_D5||||
|A.9|TX1||||
|B.0|servo0|||Timer 3|
|B.1|ystop||LIMIT1|Timer 3|
|B.10|zstop||LIMIT2|Timer 2|
|B.12|LCD_SS|||Timer 2|
|B.13|LCD_SCK||||
|B.14|LCD_MISO|||Timer 12|
|B.15|LCD_MOSI|||Timer 8|
|B.3|LCD_CD|||Timer 2|
|C.0|e0temp|t0|TH0||
|C.2|bedtemp|tb|TH1||
|C.6|fan0|fan|FAN0|Timer 8|
|C.7|fan1||FAN1|Timer 3|

<div class="datatable-end"></div>