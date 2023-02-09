---
title: Fly-407ZG Pins
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly-407ZG Pin map"
sidebar: mydoc_sidebar
permalink: fly-407zg_pins.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: "Fly-407ZG" 
ver: "" 

---
## Fly-407ZG Pinout Diagram

<a href="https://teamgloomy.github.io/images/fly_407zg_pins.svg"><img src="https://github.com/TeamGloomy/TeamGloomy.github.io/raw/main/images/fly_407zg_pins.svg?sanitize=true"></a>

## Fly-407ZG Driver Pins in Firmware

Driver pin numbers. They are separated into driver number.

<div class="datatable-begin"></div>

|Pin Type|0|1|2|3|4|5|6|7|8|
| :------------- |:-------------|:-------------|:-------------|:-------------|:-------------|:-----|:--|:--|:--|
|Enable Pins|PE1|PG12|PD7|PD4|PD0|PG8|PG5|PG2|PD9|
|Step Pins|PB9|PB8|PA8|PC7|PC6|PD15|PD14|PD13|PD12|
|Direction Pins|PE0|PG11|PD6|PD3|PA15|PG7|PG4|PD11|PD8|
|UART Pins|PG13|PG10|PD5|PD1|PA14|PG6|PG3|PD10|PB12|

<div class="datatable-end"></div>

## Fly-407ZG Other Pins in Firmware 

If more than one pin name is availble, either name can be used in the firmware (config.g).  
If the pins aren't in the table (due to not having a special name), then the pin itself can be used in the form of PA0, PA.0, PA_0, A0, A.0 or A_0.  

<div class="datatable-begin"></div>

|Pin Number|Pin Name 1|Pin Name 2|
| :------------- |:-------------|:-------------|
|PA0|e0temp|t0|
|PA1|fan3||
|PA2|fan2||
|PA3|dljc||
|PA9|TX1||
|PA10|RX1||
|PB2|LCD_CD||
|PB10|BEEP||
|PB11|fan5||
|PB13|LCD_SCK||
|PB14|LCD_EN||
|PB15|LCD_MOSI||
|PC0|e2temp|t2|
|PC1|e1temp|t1|
|PC2|xmax|xstopmax|
|PC3|xmin|xstop|
|PC4|BTN_EN2||
|PC5|BTN_EN1||
|PC8|SDD0||
|PC9|SDD1||
|PC10|SDD2||
|PC11|SDD3||
|PC12|SDSCK||
|PC13|SDCD||
|PC14|z3||
|PC15|zmax|zstopmax|
|PD2|SDCMD||
|PE2|bed|hbed|
|PE3|e5heat|he5|
|PE4|e4heat|he4|
|PE5|e3heat|he3|
|PE6|e2heat|he2|
|PE7|LCD_D7||
|PE8|LCD_D6||
|PE9|LCD_D5||
|PE10|LCD_D4||
|PE11|servo0||
|PE12|LCD_RS||
|PE13|fan4||
|PE14|LCD_EN||
|PE15|BTN_ENC||
|PF0|zmin|zstop|
|PF2|ymin|ystop|
|PF3|bedtemp|tb|
|PF1|ymax|ystopmax|
|PF4|e5temp|t5|
|PF5|e4temp|t4|
|PF6|e1heat|he1|
|PF7|e0heat|he0|
|PF8|fan0|fan|
|PF9|fan1||
|PF10|e3temp|t3|
|PF11|LCD_SS||

<div class="datatable-end"></div>

{% include custom/can/sht_links.html %}