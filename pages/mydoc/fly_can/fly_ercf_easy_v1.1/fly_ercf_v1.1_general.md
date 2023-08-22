---

title: Fly-ERCF-Easy-BRD-V1.1 General Information
tags: []
keywords: 
last_updated: 22/08/2023
summary: "General information regarding the Fly-ERCF-Easy-BRD-V1.1"
sidebar: mydoc_sidebar
permalink: fly_ercf_v1.1_general.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: Fly-ERCF-Easy-BRD-V1.1
firmware: CAN bus
version: v1

overview_img1: "ercf_easy_v1.1/front_back.png"
overview_cap1: "Fly-ERCF-Easy-BRD-V1.1 Front and Rear view"

overview_img2: "ercf_easy_v1.1/dimensions.png"
overview_cap2: "Fly-ERCF-Easy-BRD-V1.1 dimensions"

overview_img3: "ercf_easy_v1.1/package_contents.png"
overview_cap3: "Fly-ERCF-Easy-BRD-V1.1 BOM"

overview_img3: "ercf_easy_v1.1/jumpers.png"
overview_cap3: "Fly-ERCF-Easy-BRD-V1.1 Driver Jumper Locations"

---
## {{ page.boardname }} Overview

    {% capture mcustep %}{{ page.mcustep }}{% endcapture %}
    {% capture mcustep2 %}{{ page.mcustep2 }}{% endcapture %}
    {% capture mcusch %}{{ page.mcusch }}{% endcapture %}

    {% capture overurl1 %}.\images\{{page.overview_img1}}{% endcapture %}
    {% capture overurl2 %}.\images\{{page.overview_img2}}{% endcapture %}       
    {% capture overurl3 %}.\images\{{page.overview_img3}}{% endcapture %}   

### Description

The {{page.boardname}} toolboard uses CAN communication to connect the host computer with a UTOC board, other USB to CAN adapters, Pi Hats, USB to CAN Bridge Mode in Klipper or USB. For USB use it is recommended to not to use a cable that exceeds 1 meter ( 3.2 feet ) in length.  
The {{page.boardname}} is available from [AliExpress](https://s.click.aliexpress.com/e/_DmjzdR5)

{% include image.html file=page.overview_img1 url=overurl1 alt=page.overview_cap1 caption=page.overview_cap1 %}

### Product Features

- CANbus connection for stable data transmission over long distaces.
- 24 volt max input
- 5 amp mosfet for heater control
- SPI/UART Driver Support
- Peripheral interface:USB*1, CAN*1, Servo*1, Probe*1, EndStop*1, Encoder*1
- 5V anti-backflow

{% include image.html file=page.overview_img2 url=overurl2 alt=page.overview_cap2 caption=page.overview_cap2 %}

### Driver Jumpers

The jumpers should be installed as below. “Common Interpolation” should be used for standalone drivers. “SPI mode Interpolation” is supported for TMC5160 drivers. “UART mode Interpolation” should be used when using smart drivers (i.e. TMC2208, TMC2209, TMC2225 and TMC2226)

{% include image.html file=page.overview_img4 url=overurl4 alt=page.overview_cap4 caption=page.overview_cap4 %}

### BOM

{% include image.html file=page.overview_img3 url=overurl3 alt=page.overview_cap3 caption=page.overview_cap3 %}

### Included parts

- {{ page.boardname }} Board
- Jumpers * 9
- JST-XH plugs and Female Crimp Terminals
- XT30+2 3 meter 4 wire harness
- USB-A to USB-C Cable

{% include custom/mcu/ercf_v1.1/ercf_v1.1_links.html %}
