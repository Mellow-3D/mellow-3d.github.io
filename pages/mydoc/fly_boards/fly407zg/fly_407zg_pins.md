---
title: Fly-407ZG Pins
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly-407ZG Pin map"
sidebar: mydoc_sidebar
permalink: fly_407zg_pins.html
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

|Pin Type|0(X)|1(Y)|2(Z)|3(E0)|4(E1)|5(E2)|6(E3)|7(E4)|8(E5)|
| :------------- |:-------------|:-------------|:-------------|:-------------|:-------------|:-----|:--|:--|:--|
|Enable Pins|PE1|PG12|PD7|PD4|PD0|PG8|PG5|PG2|PD9|
|Step Pins|PB9|PB8|PA8|PC7|PC6|PD15|PD14|PD13|PD12|
|Direction Pins|PE0|PG11|PD6|PD3|PA15|PG7|PG4|PD11|PD8|
|UART Pins|PG13|PG10|PD5|PD1|PA14|PG6|PG3|PD10|PB12|

<div class="datatable-end"></div>

## Fly-407ZG Other Pins in Firmware 

<div class="datatable-begin"></div>

|Pin Number|Pin Name 1|Pin Name 2|Alias
| :------------- |:-------------|:-------------|:-------------|
|PA0|e0temp|t0|
|PA1|fan3||
|PA2|fan2||
|PA3|dljc||
|PA9|TX1||
|PA10|RX1||
|PB2|LCD_CD||EXP2_7|
|PB10|LCD_BEEP|BEEP|EXP1_1|
|PB11|fan5||
|PB13|LCD_SCK||EXP2_2|
|PB14|LCD_MISO||EXP2_1|
|PB15|LCD_MOSI||EXP2_6|
|PC0|e2temp|t2|
|PC1|e1temp|t1|
|PC2|xmax|xstopmax|
|PC3|xmin|xstop|
|PC4|LCD_BTN_EN2|BTN_EN2|EXP2_5|
|PC5|LCD_BTN_EN1|BTN_EN1|EXP2_3|
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
|PE7|LCD_D7||EXP1_8|
|PE8|LCD_D6||EXP1_7|
|PE9|LCD_D5||EXP1_6|
|PE10|LCD_D4||EXP1_5|
|PE11|servo0||
|PE12|LCD_RS||EXP1_4|
|PE13|fan4||
|PE14|LCD_EN||EXP1_3|
|PE15|LCD_BTN_ENC|BTN_ENC|EXP1_2|
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
|PF11|LCD_SS||EXP2_4|
|\<GND>|LCD_GND||EXP1_9|
|\<5V> |LCD_VCC||EXP1_10|
|\<RST>|LCD_RST||EXP2_8|
|\<GND>|LCD_GND||EXP2_9|
|\<NC> |LCD_KILL||EXP2_10|

<div class="datatable-end"></div>

{% include custom/can/sht_links.html %}