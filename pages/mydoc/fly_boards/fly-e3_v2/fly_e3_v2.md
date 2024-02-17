---
title: Fly-E3-v2 General Information
tags: []
keywords: 
last_updated: 17/02/2024
summary: "General information regarding the Fly-E3-v2"
sidebar: mydoc_sidebar
permalink: fly_e3_v2.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-E3-v2
version: v2

mcu: "fly-e3_v2"

fly_e3_v2_img1: "fly-e3_v2/fly-e3_v2_image.webp"
fly_e3_v2_cap1: "Fly-E3-v2 Overview"

fly_e3_v2_img2: "fly-e3_v2/fly_e3_jumpers.png"
fly_3_v2_cap2: "Fly-E3-v2 Driver Jumper Locations"

fly_e3_v2_img3: "fly-e3_v2/fly-e3_v2_dimensions.webp"
fly_3_v2_cap3: "Fly-E3-v2 dimensions"



---
    {% capture boardname %}{{ page.boardname }}{% endcapture %}

    {% capture mcu %}{{ page.mcu }}{% endcapture %}

    {% capture fly_e3_v2_img1 %}{{page.fly_e3_v2_img1 }}{% endcapture %}
    {% capture fly_e3_v2_cap1 %}{{page.fly_e3_v2_cap1 }}{% endcapture %}
    {% capture fly_e3_v2_url1 %} .\images\{{ page.fly_e3_v2_img1 }} {% endcapture %}

    {% capture fly_e3_v2_img2 %}{{page.fly_e3_v2_img2 }}{% endcapture %}
    {% capture fly_e3_v2_cap2 %}{{page.fly_e3_v2_cap2 }}{% endcapture %}
    {% capture fly_e3_v2_url2 %} .\images\{{ page.fly_e3_v2_img2 }} {% endcapture %}

    {% capture fly_e3_v2_img3 %}{{page.fly_e3_v2_img3 }}{% endcapture %}
    {% capture fly_e3_v2_cap3 %}{{page.fly_e3_v2_cap3 }}{% endcapture %}
    {% capture fly_e3_v2_url3 %} .\images\{{ page.fly_e3_v2_img3 }} {% endcapture %}

## Fly-E3-v2 General Information

{% 
include image.html 
file=fly_e3_v2_img1
url=fly_e3_v2_url1
alt=fly_e3_v2_cap1
caption=fly_e3_v2_cap1
%}

### Overview

This page covers any general information for the Fly-E3-v2 board.
It is currently available through [AliExpress](https://s.click.aliexpress.com/e/_Dm8O04D).

{% include tip.html content="You need to also buy the WiFi module from Mellow to be able to use RRF with this board." %}

### Features

- 32-bit ARM Cortex-M4 series 168 MHz, STM32F407ZGT6 chip
- Supported Firmware: Marlin 2.0, Reprap, and Klipper
- Drivers supported: A4988, LV8729, DRV8225, TMC2208, 2209, & 5160
- Drive mode support: TMC: UART, & SPI
- Support for 5 independent motor drives, 2 extruders, and 4 PWM fans
- All drivers sockets support up to 24 volts.
- Supported Displays: serial touch screen, 12864 LCD, 2004 LCD , FLY 4.3, & 7.0 V1
- Supports automatic bed leveling sensor: BLTouch
- Onboard CAN bus transciever.
- Optional  WiFi module supported with Reprap firmware.
- PWM Fan MOS boards can be directly replaced in case of damage.

### Driver Jumpers

The jumpers should be installed as below. “Common Interpolation” should be used for standalone drivers. “SPI mode Interpolation” is supported for TMC5160 drivers. “UART mode Interpolation” should be used when using smart drivers (i.e. TMC2208, TMC2209, TMC2225 and TMC2226)

{% 
include image.html 
file=fly_e3_v2_img2
url=fly_e3_v2_url2
alt=fly_e3_v2_cap2
caption=fly_e3_v2_cap2
%}

### Driver Diag Pin

The driver diag pin is used for sensorless homing and stall detection.
The Fly-E3-v2 does not have a way of disabling the diag pin as it is designed to be used with Fly-2209 drivers which have a switch on the underside of them for disabling the diag pin.
If you plan on using endstops rather than sensorless homing and do not have the Fly-2209 drivers, you need to bend or remove the diag pin.

### Fan Mosfets

The Fly-E3-v2 has a unique feature in that the fan mosfets are replaceable.
Each mosfet (VS3622e) controls two of the fan outputs.
The orientation that the fan mostfet is plugged into the board doesn't matter.

### Input voltage

The board can handle an input voltage up to 32v.

### Initial Installation

The board that you will receive doesn’t have any firmware installed so when plugged into a computer, the board will show as an unidentified device.

### Dimensions

{% 
include image.html 
file=fly_e3_v2_img3
url=fly_e3_v2_url3
alt=fly_e3_v2_cap3
caption=fly_e3_v2_cap3
%}

{% include custom/mcu/e3v2/fly_e3_v2_links.html %}
