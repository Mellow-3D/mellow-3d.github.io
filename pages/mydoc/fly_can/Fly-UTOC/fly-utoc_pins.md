---
title: Fly UTOC-1 and UTOC-3 pin diagram
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly UTOC-1 and UTOC-3 pin diagram"
sidebar: mydoc_sidebar
permalink: fly-utoc_pins.html
folder: mydoc
comments: false
toc: true
datatable: true

mcu: "UTOC-1 and UTOC-3"

fly-utoc_pins_img1:  "fly-utoc/fly_utoc-pins.png"
fly-utoc_pins_cap1:  "Fly UTOC-1 and UTOC-3 pin locations" 


---
    {% capture fly-utoc_pins_img1 %}{{page.fly-utoc_pins_img1 }}{% endcapture %}
    {% capture fly-utoc_pins_cap1 %}{{page.fly-utoc_pins_cap1 }}{% endcapture %}
    {% capture fly-utoc_pins_url1 %} .\images\{{ page.fly-utoc_pins_img1 }} {% endcapture %}

## {{page.summary}}

  {% 
  include image.html 
  file=fly-utoc_pins_img1
  url=fly-utoc_pins_url1
  alt=fly-utoc_pins_cap1
  caption=fly-utoc_cap1
  %}

### Table of pin functions

<div class="datatable-begin"></div>

| **Device** |  **Function** | 
|:-----------|:--------------|
|**USB C** |USB in from host |
|**DFU** |Device Firmware Update. Add jumper and restart the board to enter DFU mode for flashing firmware.|
|**+5V** |5v from USB or from onboard 24v to 5v regulator.  |
|**12-24V** | VCC in 12 to 24 volts
|**GND** | Ground  |
|**120r** | 120 ohm resistor for CAN bus termination |
|**CAN L** | CAN bus high line |
|**CAN H** | CAN bus low line | 
|**CAN bus**| USB A ports for connecting to STM32 boards without an onboard CAN port. Supports CAN bus with some STM32 CPUs connected to the PA11/PA12 USB port with klipper firmware. 

{% include custom/can/sht_links.html %}