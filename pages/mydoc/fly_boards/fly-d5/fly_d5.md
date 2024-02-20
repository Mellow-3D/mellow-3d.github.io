---
title: Fly-D5 General Information
tags: []
keywords: 
last_updated: 17/02/2024
summary: "General information regarding the Fly-D5"
sidebar: mydoc_sidebar
permalink: fly_d5.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-D5
version: v2

mcu: "fly-D5"

img1: "fly-d5/fly_d5.png" 
cap1: "Fly-D5 Overview"

img2: "fly-d5/driver_jumpers.png"
cap2: "Fly-D5 Driver Jumper Locations"

img3: "fly-d5/dimensions.png"
cap3: "Fly-D5 Dimensions"

img4: "fly-d5/sensorless.png"
cap4: "Fly-D5 Senorless Jumpers"

---

    {% capture url1 %} .\images\{{ page.img1 }} {% endcapture %}
    {% capture url2 %} .\images\{{ page.img2 }} {% endcapture %}
    {% capture url3 %} .\images\{{ page.img3 }} {% endcapture %}
    {% capture url4 %} .\images\{{ page.img4 }} {% endcapture %}

## {{page.boardname}} General Information

{%
include image.html
file=page.img1
url=url1
alt=page.cap1
caption=page.cap1
%}

### Overview

This page covers any general information for the {{page.boardname}} board.
It is currently available through [AliExpress](https://s.click.aliexpress.com/e/_DFbcrJJ).

### Features

- MCU: STM32F072RBT6
- Firmware: Klipper
- Supports 12-24V DC power supply, which makes the power supply more stable and eliminates the need for step-down modules.
- Driver working mode support: SPI, UART, STEP/DIR
- Support driver: supports external TMC5160Pro, TMC5160, TMC2209, TMC2225, TMC2226, TMC2208, TMC2130, A4988, etc.
- Expansion interface: BLTouch (Servos, Probe), UART X1, 12864 X1
- Fans: Two-wire controllable fan X2, parallel fan X2, normally open fan X2
- Temperature sensor: 2-way NTC 100K
- Supported machine structures: Cartesian, Delta, Kossel, Ultimaker, CoreXY

### Driver Jumpers

The jumpers should be installed as below. “Common Interpolation” should be used for standalone drivers. “SPI mode Interpolation” is supported for TMC5160 drivers. “UART mode Interpolation” should be used when using smart drivers (i.e. TMC2208, TMC2209, TMC2225 and TMC2226)

{%
include image.html
file=page.img2
url=url2
alt=page.cap2
caption=page.cap2
%}

### Driver Diag Pin

The driver diag pin is used for sensorless homing and stall detection.
To enable the diag pin, add a jumper as shown in the image below.  

{%
include image.html
file=page.img4
url=url4
alt=page.cap4
caption=page.cap4
%}

### Input voltage

The board can handle an input voltage up to 32v.

### Initial Installation

The board that you will receive doesn’t have any firmware installed so when plugged into a computer, the board will show as an unidentified device.

### Dimensions

{%
include image.html
file=page.img3
url=url3
alt=page.cap3
caption=page.cap3
%}

{% include custom/mcu/d5/fly_d5_links.html %}
