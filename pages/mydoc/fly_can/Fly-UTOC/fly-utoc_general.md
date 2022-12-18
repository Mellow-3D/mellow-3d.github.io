---
title: Fly UTOC-1 and UTOC-3 General Information
tags: []
keywords: 
last_updated: 20/10/2022
summary: "General information regarding the Fly UTOC-1 and UTOC-3"
sidebar: mydoc_sidebar
permalink: fly-utoc_general.html
folder: mydoc
comments: false
toc: true
datatable: true

mcu: "UTOC-1 and UTOC-3"

utoc_img1:  "fly-utoc/fly_utoc-1_3_front_back.png"
utoc_cap1:  "Fly UTOC1 and UTOC-3 boards" 

utoc_img2:  "fly-utoc/fly-utoc_dimensions.png"
utoc_cap2:  "Fly UTOC1 and UTOC-3 boards" 

utoc_img3:  "fly-utoc/fly-utoc_1_bom.webp"
utoc_cap3:  "Fly UTOC1 and UTOC-3 boards" 

---


    {% capture mcu %}{{ page.mcu }}{% endcapture %}

    {% capture utoc_img1 %}{{page.utoc_img1 }}{% endcapture %}
    {% capture utoc_cap1 %}{{page.utoc_cap1 }}{% endcapture %}
    {% capture utoc_url1 %} .\images\{{ page.utoc_img1 }} {% endcapture %}

    {% capture utoc_img2 %}{{page.utoc_img2 }}{% endcapture %}
    {% capture utoc_cap2 %}{{page.utoc_cap2 }}{% endcapture %}
    {% capture utoc_url2 %} .\images\{{ page.utoc_img2 }} {% endcapture %}    

    {% capture utoc_img3 %}{{page.utoc_img3 }}{% endcapture %}
    {% capture utoc_cap3 %}{{page.utoc_cap3 }}{% endcapture %}
    {% capture utoc_url3 %} .\images\{{ page.utoc_img3 }} {% endcapture %}

## Overview 

{% 
include image.html 
file=utoc_img1
url=utoc_url1
alt=utoc_cap1
caption=utoc_cap1
%}


### Fly UTOC-1 and UTOC-3 General Information.


- USB-IN : USB to CAN input interface , connected to the host computer
- 12-24V & GND : Power connector

- CANBUS : CAN interface , connected to expansion motherboardsand tool boards , etc ( connected to devices with on-board CANtransceiver chips

- CANBUS * : For connecting to motherboards withoutCAN port ( only for connecting to STM32 , s USB ( PA11 / PA12 ) portplease pay attention to purchase the corresponding UTOC version )√The volume is compressed to the extreme , SHT36 adopts a6-layer board design

- Support for CAN bus connections , data transmission is more stable , delay is smaller , and distance is longer

- The {{mcu}} is suitable for all devices that can run linux , such as raspberry pi

### Dimensions

{% 
include image.html 
file=utoc_img2
url=utoc_url2
alt=utoc_cap2
caption=utoc_cap2
%}

### BOM

{% 
include image.html 
file=utoc_img3
url=utoc_url3
alt=utoc_cap3
caption=utoc_cap3
%}

### Common questions:

- What cable should be used to connect Can board to {{mcu}}?

  - Four wires, two signal wires are more than 26AWG, two power supply wires up the 18AWG.

- What is the difference between UTOC-1 and UTOC-3?

  - UTOC-1 can only be connected to board with CAN transceiver. The UTOC-3 can be connected to boards that supports CAN but do not have an onboard CAN transceiver (only stm32, using PA11/PA12 of the usb port). UTOC-3 supports connecting 2 boards without can transcievers.

- What host computer does the  {{mcu}} support?

  - You can use it if your host computer system kernel supports can. Operating systems such as Rasbian, Armbian, Debian, and others.

{% include custom/can/sht_links.html %}