---
title: Fly-CDYv3 General Information
tags: []
keywords: 
last_updated: 09/07/2023
summary: "General information regarding the Fly-CDYv3"
sidebar: mydoc_sidebar
permalink: fly_cdyv3.html
folder: mydoc
comments: false
toc: false
datatable: true

fly-cdy_v3_img1: "fly-cdy_v3/fly-cdy_v3_front_back.webp"
ffly-cdy_v3_cap1: "Fly-CDYv3 Overview"

fly-cdy_v3_img2: "fly-cdy_v3/fly-cdy_v3_z1_z2_jumper.webp"
fly-cdy_v3_cap2: "Fly-CDYv3 Driver Z Jumper Locations"

fly-cdy_v3_img3: "fly-cdy_v3/fly-cdy_v3_driver_jumpers.png"
fly-cdy_v3_cap3: "Fly-CDYv3 Driver Jumpers"

#IMG 4 not used
fly-cdy_v3_img4: "fly-cdy_v3/fly_e3_pro_vol.png"
fly-cdy_v3_cap4: "Fly-CDYv3 12v Jumper Locations"

fly-cdy_v3_img5: "fly-cdy_v3/fly-cdy_v3_pin_diagram.webp"
ffly-cdy_v3_cap5: "Fly-CDYv3 IO pins"

fly-cdy_v3_img6: "fly-cdy_v3/fly-cdy_v3_dimensions.webp"
fly-cdy_v3_cap6: "Fly-CDYv3 dimensions"
boardname: Fly-CDYv3
mcu: "STM32F407VGT6"

---

    {% capture boardname %}{{ page.boardname }}{% endcapture %}

    {% capture mcu %}{{ page.mcu }}{% endcapture %}

    {% capture fly-cdy_v3_img1 %}{{page.fly-cdy_v3_img1 }}{% endcapture %}
    {% capture ffly-cdy_v3_cap1 %}{{page.fly-cdy_v3_cap1 }}{% endcapture %}
    {% capture fly-cdy_v3_url1 %} .\images\{{ page.fly-cdy_v3_img1 }} {% endcapture %}

    {% capture fly-cdy_v3_img2 %}{{page.fly-cdy_v3_img2 }}{% endcapture %}
    {% capture fly-cdy_v3_cap2 %}{{page.fly-cdy_v3_cap2 }}{% endcapture %}
    {% capture fly-cdy_v3_url2 %} .\images\{{ page.fly_e3_v2_img2 }} {% endcapture %}

    {% capture fly-cdy_v3_img3 %}{{page.fly-cdy_v3_img3 }}{% endcapture %}
    {% capture fly-cdy_v3_cap3 %}{{page.fly-cdy_v3_cap3 }}{% endcapture %}
    {% capture fly-cdy_v3_url3 %} .\images\{{ page.fly-cdy_v3_img3 }} {% endcapture %}

    {% capture fly-cdy_v3_img4 %}{{page.fly-cdy_v3_img4 }}{% endcapture %}
    {% capture fly-cdy_v3_cap4 %}{{page.fly-cdy_v3_cap4 }}{% endcapture %}
    {% capture fly-cdy_v3_url4 %} .\images\{{ page.fly-cdy_v3_img4 }} {% endcapture %}

    {% capture fly-cdy_v3_img5 %}{{page.fly-cdy_v3_img5 }}{% endcapture %}
    {% capture fly-cdy_v3_cap5 %}{{page.fly-cdy_v3_cap5 }}{% endcapture %}
    {% capture fly-cdy_v3_url5 %} .\images\{{ page.fly-cdy_v3_img5 }} {% endcapture %}

    {% capture fly-cdy_v3_img6 %}{{page.fly-cdy_v3_img6 }}{% endcapture %}
    {% capture fly-cdy_v3_cap6 %}{{page.fly-cdy_v3_cap6 }}{% endcapture %}
    {% capture fly-cdy_v3_url6 %} .\images\{{ page.fly-cdy_v3_img6 }} {% endcapture %}    

## Overview

This page covers any general information for the Fly-CDYv3 board.  
It is currently available through [AliExpress](https://s.click.aliexpress.com/e/_DBNB4zb). 

{% 
include image.html 
file=fly-cdy_v3_img1
url=fly-cdy_v3_url1
alt=fly-cdy_v3_cap1
caption=fly-cdy_v3_cap1
%}

### Features

 - 32-bit ARM Cortex-M4 series 168 MHz, STM32F407ZGT6 chip
 - Supported Firmware: Marlin 2.0, Reprap, and Klipper
 - Drivers supported: A4988, LV8729, DRV8225, TMC2208, TMC2209, & TMC5160
 - Drive mode support: TMC: UART, & SPI
 - Support for 6 independent motor drives, 3 extruders, and 3 PWM fans
 - All drivers support up to 24 volts.
 - Supported Displays: serial touch screen, 12864 LCD, 2004 LCD , FLY 4.3, & 7.0 V1
 - Supports automatic bed leveling sensor: BLTouch
 - WIFI chip:esp32 ( 1 . 6M / s ) Supported with Reprap firmware
 - PWM Fan MOS boards can be directly replaced in case of damage.
 - Drive signal output voltage：3.3V 5v ( default ) 12V
 
### Z Driver Jumpers

If only one Z output is being used, jumpers should be installed on the other Z output as shown below.

{% 
include image.html 
file=fly-cdy_v3_img2
url=fly-cdy_v3_url2
alt=fly-cdy_v3_cap2
caption=fly-cdy_v3_cap2
%}

### Driver Jumpers

Driver communication jumpers

{% 
include image.html 
file=fly-cdy_v3_img3
url=fly-cdy_v3_url3
alt=fly-cdy_v3_cap3
caption=fly-cdy_v3_cap3
%}

### Power Configuration

The Fly-CDYv3 has one 24v input and one ground. 

### Maximum Input voltage

The board can handle an input voltage up to 32v.

### Thermistor inputs

Natively, the Fly-CDYv3 supports PT1000 and standard thermistors (with a 4k7 pullup resistor) and has a total of 4 temperature sensor inputs.  
It is possible to connect a PT100 or K type thermocouple using an external module.  

### Initial Installation

The board that you will receive doesn't have any firmware installed so when plugged into a computer, the board will show as an unidentified device.

### IO Pins

{% 
include image.html 
file=fly-cdy_v3_img5
url=fly-cdy_v3_url5
alt=fly-cdy_v3_cap5
caption=fly-cdy_v3_cap5
%}

### Dimensions

{% 
include image.html 
file=fly-cdy_v3_img6
url=fly-cdy_v3_url6
alt=fly-cdy_v3_cap6
caption=fly-cdy_v3_cap6
%}

{% include custom/mcu/cdyv3/fly_cdyv3_links.html %}