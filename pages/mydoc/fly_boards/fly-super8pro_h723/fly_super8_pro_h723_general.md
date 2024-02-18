---
title: Fly-Super8Pro H723 General Information
tags: []
keywords: 
last_updated: 18/02/2024
summary: "General information for the Fly-Super8Pro H723"
sidebar: mydoc_sidebar
permalink: fly_super8_pro_h723_general.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: "Fly-Super8Pro H723" 
ver: "V1.3" 
processor: "STM32H723"
super8_img1: "fly-super8_pro/fly-super8_pro_front_back.webp"
super8_cap1: "Super 8 Pro Front and Back"

---

        {% capture boardname %}{{ page.boardname }}{% endcapture %}
        {% capture ver %}{{ page.ver }}{% endcapture %}
    {% capture super8_img1 %}{{page.super8_img1 }}{% endcapture %}
    {% capture super8_cap1 %}{{page.super8_cap1 }}{% endcapture %}
    {% capture super8_url1 %} .\images\{{ page.super8_img1 }} {% endcapture %}

## Overview

{%
include image.html
file=super8_img1
url=super8_url1
alt=super8_cap1
caption=super8_cap1
%}

This page covers any general information for the {{boardname}} boards.  
It is currently available through [AliExpress](https://s.click.aliexpress.com/e/_DDiWwl3).
There are two versions of the Fly-Super8Pro. One has an STM32H743 MCU and the other has an STM32H723. This is the information for the STM32H723.  

- 32-bit ARM Cortex-M7 Kernel 550MHz, STM32H723ZGT6 Chip
- Supported Firmware: Marlin 2.0, Reprap, and Klipper
- Drivers supported: A4988, LV8729, DRV8225, TMC2208, 2209,5160, & 5160HV.
- Drive mode support: TMC: UART, & SPI
- Support for 8 independent motor drives, 5 extruders, and 10 PWM fans
- All drivers sockets support up to 48 volts.
- Supported Displays: serial touch screen, 12864 LCD, 2004 LCD , FLY 4.3, & 7.0 V1
- Supports automatic bed leveling sensor: BLTouch
- Optional limit switch power supply: 5V, 12V, & 24V
- On-board WiFi supported with Reprap firmware.
- PWM Fan MOS boards can be directly replaced in case of damage.

### Board Fuses

The board is supplied without the fuses installed.  
It is supplied with different fuses than the listing on AliExpress. The fuses should be installed as shown below.  

{% include image.html file="fly-super8_pro/fly_super8_fuses.png" alt="Fly-Super8 Fuses" caption="Fly-Super8 Fuses" %}

### Board Power

The Fly-Super8 has 4 lots of power inputs. The first one powers drivers 0 to 2, the second one powers drivers 3 to 7, the third one powers the boards, heaters and fans and the last one powers the bed.  

{% include image.html file="fly-super8_pro/fly_super8_power.png" alt="Fly-Super8 Power Connections" caption="Fly-Super8 Power Connections" %}

### Maximum Input voltage

#### Board/Bed Power

The main board and heated bed power inputs can handle voltage up to 30v.

#### Driver Power

{{boardname}} version 1.3, both of the driver power inputs 0-2 and 3-7 can handle voltage up to 62v.

{%
include image.html
file="fly-super8\fly-super8_drive_power.png"
alt="Fly-Super 8 Driver Voltage"
caption="Fly-Super 8 Driver Voltage"
%}

{% include warning.html content="In industry, 30 volts is generally considered to be a conservative threshold value for dangerous voltage. The cautious person should regard any voltage above 30 volts as threatening, not relying on normal body resistance for protection against shock." %}

### Driver Jumpers

The jumpers should be installed as below. "Common Interpolation" should be used for standalone drivers. "SPI mode Interpolation" is supported for TMC5160 drivers. "UART mode Interpolation" should be used when using smart drivers (i.e. TMC2208, TMC2209, TMC2225 and TMC2226)

{%
include image.html
file="fly-super8\fly-super8_driver_jumpers.png"
alt="Fly-Super 8 Driver Jumpers"
caption="Fly-Super 8 Driver Jumper Locations"
%}

### Driver Diag Pin

The driver diag pin is used for sensorless homing and stall detection.  
The {{boardname}} **does not** have a way of disabling the diag pin as it is designed to be used with [Fly-2209 drivers](https://s.click.aliexpress.com/e/_DnBFVNR) which have a switch on the underside of them for disabling the diag pin.  Set the dip switch to 'ON' to enable the diag pin.
If you plan on using endstops rather than sensorless homing and do not have the Fly-2209 drivers, you need to bend or remove the diag pin.

### Fan Mosfets

The {{boardname}} features 5 replacable fan mosfet modules (VS3622e) that control 10 fan outputs.

If the MOSFET is damaged by an accidental short circuit it can easily be replaced.
New Fly-MOS modules can be purchased from the [Mellow store](https://www.aliexpress.us/item/3256803593540212.html)

The Fan-MOS design allows it to be inserted in either orientation.

{%
include image.html
file="fly-super8\fly-super8_fan_mos.png"
alt="Fly-Super 8 Fan Mosfet"
caption="Fly-Super 8 Fan Mosfet"
%}

### Fan Voltage

The fan voltage can be set using jumpers to either 5v, 12v and Vin.  
Set them as shown below.  

{%
include image.html
file="fly-super8\fly-super8_fan_voltage.png"
alt="Fly-Super 8 Fan Voltage"
caption="Fly-Super 8 Fan Voltage"
%}

### IO Output Voltage

The IO output voltage can be set to either 3.3v, 5v or 12v. The default is 5v.  
Set them as shown below.  

{% include image.html file="fly-super8_pro/fly_super8_io_voltage.png" alt="Fly-Super8 IO Voltage" caption="Fly-Super8 IO Voltage" %}

### Thermistor Connection  

Thermistors should use the ADC inputs. The thermistors should be connected between ground and the signal pin.  

{% include image.html file="fly_super8_hotend_thermistors.png" alt="Fly-Super8 Hotend Thermistors" caption="Fly-Super8 Hotend Thermistors" %}

{% include image.html file="fly_super8_bed_thermistor.png" alt="Fly-Super8 Bed Thermistors" caption="Fly-Super8 Bed Thermistors" %}

{% include custom/mcu/super8/fly_super8pro_links.html %}
