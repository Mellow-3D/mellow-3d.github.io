---
title: Fly_Super5Pro General Information
tags: []
keywords: 
last_updated: 18/02/2024
summary: "General information for the Fly-Super5Pro"
sidebar: mydoc_sidebar
permalink: fly_super5_pro_general.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: "Fly-Super 5 Pro" 
ver: "V1.3" 
processor: "STM32H723"
super5_img1: "fly-super5_pro/fly-super5_pro.webp"
super5_cap1: "Super 5 Pro"

---

        {% capture boardname %}{{ page.boardname }}{% endcapture %}
        {% capture ver %}{{ page.ver }}{% endcapture %}
    {% capture super5_img1 %}{{page.super5_img1 }}{% endcapture %}
    {% capture super5_cap1 %}{{page.super5_cap1 }}{% endcapture %}
    {% capture super5_url1 %} .\images\{{ page.super5_img1 }} {% endcapture %}

## Overview

{%
include image.html
file=super5_img1
url=super5_url1
alt=super5_cap1
caption=super5_cap1
%}

This page covers any general information for the {{boardname}} boards.  
It is currently available through [AliExpress](https://s.click.aliexpress.com/e/_DFkyueN).
This is the information for the Fly Super 5 Pro with STM32H723 CPU.  

- 32-bit ARM Cortex-M7 Kernel 550MHz, STM32H723ZGT6 Chip
- 5A 5v power supply
- Supported Firmware: Marlin 2.0, Reprap, and Klipper
- Drivers supported: A4988, LV8729, DRV8225, TMC2208, 2209,5160, & 5160HV.
- Drive mode support: TMC: UART, & SPI
- Support for 5 independent motor drives, 2 extruders, and 4 PWM fans
- All drivers sockets support up to 48 volts.
- Supported Displays: serial touch screen, 12864 LCD, 2004 LCD , FLY 4.3, & 7.0 V1
- Supports automatic bed leveling sensor: BLTouch
- 3 ADC interfaces
- 6 I/O ports
- 1 high voltage IN port
- Optional limit switch power supply: 5V, 12V, & 24V
- Optional -On-board WiFi module supported with Reprap firmware.
- PWM Fan MOS boards can be directly replaced in case of damage.\
- On-Board 8Mhigh speed CAN-FD interface

### Board Fuses

The board is supplied without the fuses installed. The fuse should be installed before powering on.

{% include image.html file="fly-super5_pro/fly_super5pro_fuses.png" alt="Fly-Super5Pro Fuses" caption="Fly-Super5Pro Fuses" %}

### Thermistor inputs

The Fly-Super5Pro H723 supports PT1000 on the thermistor inputs by using a 2k2 resistor rather than a 4k7.

{% include important.html content="The Fly-Super5Pro H723 uses a 2k2 resistor on the thermistor inputs rather than 4k7. Please make sure you add R2200 to each M308 in your config" %}

### Thermistor Connection  

Thermistors should use the ADC inputs. The thermistors should be connected between ground and the signal pin.  

{% include image.html file="fly-super5_pro/fly_super5pro_thermistors.png" alt="Fly-Super5Pro Thermistor Connection" caption="Fly-Super5Pro Thermistor Connection" %}

### Driver Jumpers

The jumpers should be installed as below. "Common Interpolation" should be used for standalone drivers. "SPI mode Interpolation" is supported for TMC5160 drivers. "UART mode Interpolation" should be used when using smart drivers (i.e. TMC2208, TMC2209, TMC2225 and TMC2226)

{%
include image.html
file="fly-super5_pro\fly-super5_driver_jumpers.png"
alt="Fly-Super 5 pro Driver Jumpers"
caption="Fly-Super 5 Driver Jumper Locations"
%}

### Driver Diag Pin

The driver diag pin is used for sensorless homing and stall detection.  
The {{boardname}} **does not** have a way of disabling the diag pin as it is designed to be used with [Fly-2209 drivers](https://www.aliexpress.com/item/1005001877899893.html) which have a switch on the underside of them for disabling the diag pin.  Set the dip switch to 'ON' to enable the diag pin.
If you plan on using endstops rather than sensorless homing and do not have the Fly-2209 drivers, you need to bend or remove the diag pin.

### Fan Mosfets

The {{boardname}} features 2 replacable fan mosfet modules (VS3622e) that control 4 fan outputs.

If the MOSFET is damaged by an accidental short circuit it can easily be replaced.
New Fly-MOS modules can be purchased from the [Mellow store](https://www.aliexpress.us/item/3256803593540212.html)

The Fan-MOS design allows it to be inserted in either orientation.

{%
include image.html
file="fly-super5_pro\fly-super5_fan_mos.png"
alt="Fly-Super 5 Fan Mosfet"
caption="Fly-Super 5 Fan Mosfet"
%}

### Fan Voltage

The fan voltage can be set using jumpers to either 5v, 12v and Vin.  
Set them as shown below.  

{%
include image.html
file="fly-super5_pro\fly-super5_fan_voltage.png"
alt="Fly-Super 5 Fan Voltage"
caption="Fly-Super 5 Fan Voltage"
%}

### Endstop Output Voltage

The Endstop output voltage can be set to either 5v or 12v. The default is 0v until a jumper is added.

{% include image.html file="fly-super5_pro/fly_super5pro_limit_voltage.png" alt="Fly-Super5Pro Endstop Voltage" caption="Fly-Super5Pro Endstop Voltage" %}

### Maximum Input voltage

#### Board/Bed Power

The main board and heated bed power inputs can handle voltage up to 30v.

#### Driver Power

{{boardname}} driver power inputs can handle voltage up to 62v.

{%
include image.html
file="fly-super5_pro\fly-super5_drive_power.png"
alt="Fly-Super 5 Driver Voltage"
caption="Fly-Super 5 Driver Voltage"
%}

{% include warning.html content="In industry, 30 volts is generally considered to be a conservative threshold value for dangerous voltage. The cautious person should regard any voltage above 30 volts as threatening, not relying on normal body resistance for protection against shock." %}

{% include custom/mcu/super5_pro/fly_super5pro_links.html %}
