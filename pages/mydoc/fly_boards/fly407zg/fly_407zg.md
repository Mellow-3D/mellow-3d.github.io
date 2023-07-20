---
title: Fly-407ZG General Information
tags: []
keywords: 
last_updated: 19/07/2023
summary: "General information regarding the Fly-407ZG"
sidebar: mydoc_sidebar
permalink: fly_407zg.html
folder: mydoc
comments: false
toc: false
datatable: true
---

## Overview

This page covers any general information for the Fly-407ZG board.  
It is currently available through [AliExpress](https://s.click.aliexpress.com/e/_DCwIy0h)

### Description:

- 32-bit ARM Cortex-M4 series 168 MHz, STM32F407ZGT6 chip
- Firmware: Marlin 2.0, Klipper and RRF
- Driver support: A4988, LV8729, DRV8825, TMC2208 / 2209, etc.
- Drive mode support: TMC: UART / SPI
- Support 9 independent motor drives, 6 extruders, 6 controllable fans, 3 uncontrollable fan sockets.
- FPC drive expansion socket, can also expand 3 additional stepper motors
- Display: serial touch screen, 12864 LCD, 2004 LCD
- Supports automatic bed leveling sensor: BLTouch
- Supports dual Z-axis printers and three Z-axis printers (the motherboard has a dedicated Z3 limit switch interface).
- Supports printer structure: XYZ, kossel, ultimaker, corexy, etc.
- Input voltage: DC12V-DC24V
- Motor driver interface: X Y Z E0 E1 E2 E3 E4 E5
- Temperature sensor interface: B, T0, T1, T2, T3, T4, T5, T6 (MAX6675 chip is not soldered by default) A total of 7 NTC 100K thermistor interfaces and one SPI thermocouple interface
- Supports one servo interface and one material detection module interface
- Optional limit switch power supply: 5V / 12V / 24V
- The hot end heater connector uses screw-free push-type terminals for quick and easy connection.

### Heatsinks

The Fly-407ZG is supplied with 2 heatsinks. They should be installed as per the image below.

{% include image.html file="fly-407zg/fly_407zg_heatsinks.jpg" alt="Fly-407ZG heatsink" caption="Fly-407ZG Heatsink Installation Location" %}

### Driver Jumpers

The jumpers should be installed as below. “Common Interpolation” should be used for standalone drivers. “SPI mode Interpolation” is supported for TMC5160 drivers. “UART mode Interpolation” should be used when using smart drivers (i.e. TMC2208, TMC2209, TMC2225 and TMC2226)

{% include image.html file="fly-407zg/fly_407zg_jumpers.png" alt="Fly-407ZG Jumpers" caption="Fly-407ZG Driver Jumper Locations" %}

### Z motor jumpers

- If the Z2 motor socket is not in use install the jumpers as shown.

{% include image.html file="fly-407zg/fly-f407zg_z_jumper.webp" alt="Fly-407ZG Z Jumpers" caption="Z2 motor jumper locations." %}

### Input voltage

The board can handle an input voltage up to 32v.

### Initial Installation

The board that you will receive doesn't have any firmware installed so when plugged into a computer, the board will show as an unidentified device.

## Issues

Some boards shipped are missing the bootloader.  
If your board has the Mellow logo on the back and when you place a firmware.bin file on the SD card and it doesn't get converted, then yours is one of these boards.  
Follow the guide for [restoring the OEM bootloader.](./fly_407zg_oem_bootloader.html) 

{% include custom/mcu/407zg/fly_407zg_links.html %}