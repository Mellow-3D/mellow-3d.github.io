---
title: Fly-ERCF-Easy-BRD-V1.1 Pin Definitions
tags: []
keywords: 
last_updated: 22/08/2023
summary: "Fly-ERCF-Easy-BRD-V1.1 pin map"
sidebar: mydoc_sidebar
permalink: fly_ercf_v1.1_pins.html
folder: mydoc
comments: false
toc: true
datatable: true

mcu: "Fly-ERCF-Easy-BRD-V1.1"

ercf_v1.1_cfg: "./files/ercf_v1.1/ercf_v1.1.cfg"
---

## {{page.summary}}

{% include image.html file="ercf_easy_v1.1/pins1.png" url="./images/ercf_easy_v1.1/pins1.png" alt="Fly-ERCF-Easy-BRD-V1.1 Pins 1" caption="Fly-ERCF-Easy-BRD-V1.1 Pins 1" %}

{% include image.html file="ercf_easy_v1.1/pins2.png" url="./images/ercf_easy_v1.1/pins2.png" alt="Fly-ERCF-Easy-BRD-V1.1 Pins 2" caption="Fly-ERCF-Easy-BRD-V1.1 Pins 2" %}

### Table of pin functions

<div class="datatable-begin"></div>

| **Device** |  **Function** | **Pin number** | **Alias** |
|:-----------|:--------------|:---------------|:----------|
|**CAN BUS** |CAN-RX| **gpio4**  | |
|**CAN BUS** |CAN-TX| **gpio5**  | |
|**Selector** |EN| **gpio3** |S_EN |
|**Selector** |STEP| **gpio2**  | S_STEP |
|**Selector** |DIR| **gpio1**  | S_DIR |
|**Selector** |UART| **gpio0**  | S_CS |
|**Selector** |DIAG| **gpio22** | S_DIAG |
|**Gear** |EN| **gpio6** |G_EN |
|**Gear** |STEP| **gpio7**  | G_STEP |
|**Gear** |DIR| **gpio8**  | G_DIR |
|**Gear** |UART| **gpio9**  | G_CS |
|**Gear** |DIAG| **gpio23** | G_DIAG |
|**Endstop** |Endstop| **gpio20** | STOP |
|**Encoder** |Encoder| **gpio15** | ENCODER|
|**Extra** |Extra IO| **gpio14** | EXTRA|
|**Servo** |Servo| **gpio21** | SERVO|
|**IO Expanison** |Expansion| **gpio26** | IO_1|
|**IO Expanison** |Expansion| **gpio27** | IO_2|
|**IO Expanison** |Expansion| **gpio28** | IO_3|
|**IO Expanison** |Expansion| **gpio29** | IO_4|
|**IO Expanison** |Expansion| **gpio25** | IO_5|
|**IO Expanison** |Expansion| **gpio10** | IO_6|
|**IO Expanison** |Expansion| **gpio11** | IO_7|
|**IO Expanison** |Expansion| **gpio12** | IO_8|
|**IO Expanison** |Expansion| **gpio24** | IO_9|
|**IO Expanison** |Expansion| **gpio13** | IO_10|

<div class="datatable-end"></div>

### Sample Configuration file: [{{page.mcu}}.cfg](./files/ercf_v1.1/ercf_v1.1.cfg)

### CANbus Termination Resistor

CANbus bus protocol there must be only two 120 ohm resistors on a bus.  
No matter how many USB devices you connect, as long as it is on the same bus only two 120-ohm resistors are to be configured. These resistors should be at either ends of the bus.  
After connecting CAN H and CAN L signal lines, use a multimeter to measure between CAN H and CAN L. The resistance between the two should be 60 ohms.  

{% include image.html file="ercf_easy_v1.1/120r.png" url="./images/ercf_easy_v1.1/120r.png" alt="Fly-ERCF-Easy-BRD-V1.1 120 Ohm Resistor" caption="Fly-ERCF-Easy-BRD-V1.1 120 Ohm Resistor" %}

### XT30 2+2 Wiring

<div class="datatable-begin"></div>

| **Color* |  **Function** |
|:-----------|:--------------|
|**RED** | 12/24V|
|**BLACK** | GND|
|**YELLOW**| CAN H |
|**WHITE**| CAN L |

<div class="datatable-end"></div>

{% include image.html file=sb2040pins_img3 url=sb2040pins_url3 alt=sb2040pins_cap3 caption=sb2040pins_cap3 %}

{% include custom/mcu/ercf_v1.1/ercf_v1.1_links.html %}
