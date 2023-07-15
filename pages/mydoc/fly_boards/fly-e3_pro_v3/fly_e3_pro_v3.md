---
title: Fly-E3-Pro-v3 General Information
tags: []
keywords: 
last_updated: 15/07/2023
summary: "General information regarding the Fly-E3-Pro-v3"
sidebar: mydoc_sidebar
permalink: fly_e3_pro_v3.html
folder: mydoc
comments: false
toc: false
datatable: true

fly_e3_prov3_img1: "fly-e3_pro_v3/fly-e3_pro_v3_image.webp"
fly_e3_prov3_cap1: "Fly-E3 Pro V3 Overview"

fly_e3_prov3_img2: "fly-e3_pro_v3/fly_e3_pro_zdriver.png"
fly_e3_prov3_cap2: "Fly-E3-Pro V3 Driver Z Jumper Locations"

fly_e3_prov3_img3: "fly-e3_pro_v3/fly_e3_pro_diag.png"
fly_e3_prov3_cap3: "Fly-E3-Pro V3 Diag Jumper Locations"

fly_e3_prov3_img4: "fly-e3_pro_v3/fly_e3_pro_vol.png"
fly_e3_prov3_cap4: "Fly-E3-Pro V3 12v Jumper Locations"

fly_e3_prov3_img5: "fly-e3_pro_v3/fly-e3_pro_v3_pins.webp"
fly_e3_prov3_cap5: "Fly-E3-Pro V3 IO pins"

fly_e3_prov3_img6: "fly-e3_pro_v3/fly-e3_pro_v3_dimensions.webp"
fly_e3_prov3_cap6: "Fly-E3-Pro V3 dimensions"



---

    {% capture boardname %}{{ page.boardname }}{% endcapture %}

    {% capture mcu %}{{ page.mcu }}{% endcapture %}

    {% capture fly_e3_prov3_img1 %}{{page.fly_e3_prov3_img1 }}{% endcapture %}
    {% capture ffly_e3_prov3_cap1 %}{{page.fly_e3_prov3_cap1 }}{% endcapture %}
    {% capture fly_e3_prov3_url1 %} .\images\{{ page.fly_e3_prov3_img1 }} {% endcapture %}

    {% capture fly_e3_prov3_img2 %}{{page.fly_e3_prov3_img2 }}{% endcapture %}
    {% capture fly_e3_prov3_cap2 %}{{page.fly_e3_prov3_cap2 }}{% endcapture %}
    {% capture fly_e3_prov3_url2 %} .\images\{{ page.fly_e3_v2_img2 }} {% endcapture %}

    {% capture fly_e3_prov3_img3 %}{{page.fly_e3_prov3_img3 }}{% endcapture %}
    {% capture fly_e3_prov3_cap3 %}{{page.fly_e3_prov3_cap3 }}{% endcapture %}
    {% capture fly_e3_prov3_url3 %} .\images\{{ page.fly_e3_prov3_img3 }} {% endcapture %}

    {% capture fly_e3_prov3_img4 %}{{page.fly_e3_prov3_img4 }}{% endcapture %}
    {% capture fly_e3_prov3_cap4 %}{{page.fly_e3_prov3_cap4 }}{% endcapture %}
    {% capture fly_e3_prov3_url4 %} .\images\{{ page.fly_e3_prov3_img4 }} {% endcapture %}

    {% capture fly_e3_prov3_img5 %}{{page.fly_e3_prov3_img5 }}{% endcapture %}
    {% capture fly_e3_prov3_cap5 %}{{page.fly_e3_prov3_cap5 }}{% endcapture %}
    {% capture fly_e3_prov3_url5 %} .\images\{{ page.fly_e3_prov3_img5 }} {% endcapture %}

    {% capture fly_e3_prov3_img6 %}{{page.fly_e3_prov3_img6 }}{% endcapture %}
    {% capture fly_e3_prov3_cap6 %}{{page.fly_e3_prov3_cap6 }}{% endcapture %}
    {% capture fly_e3_prov3_url6 %} .\images\{{ page.fly_e3_prov3_img6 }} {% endcapture %}    

## Overview

This page covers any general information for the Fly-E3-Pro-v3 board.  
It is currently available through [AliExpress](https://s.click.aliexpress.com/e/_DCEqwdT). 

{% 
include image.html 
file=fly_e3_prov3_img1
url=fly_e3_prov3_url1
alt=fly_e3_prov3_cap1
caption=fly_e3_prov3_cap1
%}

### Features
 - 32-bit ARM Cortex-M4 series 168 MHz, STM32F407ZGT6 chip
 - Supported Firmware: Marlin 2.0, Reprap, and Klipper
 - Drivers: Onboard TMC2209
 - Drive mode support: TMC UART
 - Support for 5 independent motor drives, 2 extruders, and 4 PWM fans
 - All drivers support up to 24 volts.
 - Supported Displays: serial touch screen, 12864 LCD, 2004 LCD , FLY 4.3, & 7.0 V1
 - Supports automatic bed leveling sensor: BLTouch
 - WiFi module supported with Reprap firmware.
 - PWM Fan MOS boards can be directly replaced in case of damage.

### Z Driver Jumpers

If only one Z output is being used, jumpers should be installed on the other Z output as shown below.

{% 
include image.html 
file=fly_e3_prov3_img2
url=fly_e3_prov3_url2
alt=fly_e3_prov3_cap2
caption=fly_e3_prov3_cap2
%}

### Driver Diag Pin

To use sensorless homing, a jumper must be installed on the diag header.

{% 
include image.html 
file=fly_e3_prov3_img3
url=fly_e3_prov3_url3
alt=fly_e3_prov3_cap3
caption=fly_e3_prov3_cap3
%}

### Power Configuration

The Fly-E3-Pro-v3 has two 24v inputs and one ground. The right 24v input powers the MCU and WiFi (as well as anything else that runs from 5v) and the left 24v input powers the motors, heaters and bed. This allows a relay to be used to turn off the motors, heaters and bed using a relay without having to use a separate 5v PSU to power the MCU. A diagragm can be found below.  

{% 
include image.html 
file=fly_e3_prov3_img4
url=fly_e3_prov3_url4
alt=fly_e3_prov3_cap4
caption=fly_e3_prov3_cap4
%}

### Maximum Input voltage

The board can handle an input voltage up to 32v.

### Thermistor inputs

The Fly-E3-Pro-v3 supports PT1000 on the thermistor inputs by using a 2k2 resistor rather than a 4k7.

{% include important.html content="The Fly-E3-Pro-v3 uses a 2k2 resistor on the thermistor inputs rather than 4k7." %}

### Initial Installation

The board that you will receive doesn't have any firmware installed so when plugged into a computer, the board will show as an unidentified device.

### IO Pins

{% 
include image.html 
file=fly_e3_prov3_img5
url=fly_e3_prov3_url5
alt=fly_e3_prov3_cap5
caption=fly_e3_prov3_cap5
%}

### Dimensions

{% 
include image.html 
file=fly_e3_prov3_img6
url=fly_e3_prov3_url6
alt=fly_e3_prov3_cap6
caption=fly_e3_prov3_cap6
%}

{% include custom/mcu/e3prov3/fly_e3_pro_v3_links.html %}