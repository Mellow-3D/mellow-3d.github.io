---
title: Fly RPFMex General Information
tags: []
keywords: 
last_updated: 20/10/2022
summary: "General information regarding the Fly RPFMex"
sidebar: mydoc_sidebar
permalink: fly-rpfmex.html
folder: mydoc
comments: false
toc: false
datatable: true

boardname: "Fly RPFMEX"

fly_rpfmex_img1: "fly-rpfmex/fly_rpfmex.png"
fly_rpfmex_cap1: "Fly-rpfmex board"

fly_rpfmex_img2: "fly-rpfmex/fly-rpfmex_dimensions.webp"
fly_rpfmex_cap2: "Fly-rpfmex board dimensions"

fly_rpfmex_img3: "fly-rpfmex/fly-rpfmex_bom.webp"
fly_rpfmex_cap3: "Fly-rpfmex BOM"


---
    {% capture boardname %}{{ page.boardname }}{% endcapture %}

    {% capture mcu %}{{ page.mcu }}{% endcapture %}

    {% capture fly_rpfmex_img1 %}{{page.fly_rpfmex_img1 }}{% endcapture %}
    {% capture fly_rpfmex_cap1 %}{{page.fly_rpfmex_cap1 }}{% endcapture %}
    {% capture fly_rpfmex_url1 %} .\images\{{ page.fly_rpfmex_img1 }} {% endcapture %}

    {% capture fly_rpfmex_img2 %}{{page.fly_rpfmex_img2 }}{% endcapture %}
    {% capture fly_rpfmex_cap2 %}{{page.fly_rpfmex_cap2 }}{% endcapture %}
    {% capture fly_rpfmex_url2 %} .\images\{{ page.fly_rpfmex_img2 }} {% endcapture %}

    {% capture fly_rpfmex_img3 %}{{page.fly_rpfmex_img3 }}{% endcapture %}
    {% capture fly_rpfmex_cap3 %}{{page.fly_rpfmex_cap3 }}{% endcapture %}
    {% capture fly_rpfmex_url3 %} .\images\{{ page.fly_rpfmex_img3 }} {% endcapture %}

## Overview 

  {% 
  include image.html 
  file=fly_rpfmex_img1
  url=fly_rpfmex_url1
  alt=fly_rpfmex_cap1
  caption=fly_rpfmex_cap1
  %}

## Description
This page covers any general information for the {{boardname}} board.  
Avaliable from the Mellow store on [Aiexpress](https://www.aliexpress.us/item/3256804203395779.html)

In order to meet the customer for expanding Gemini, we made a 4-axis expansion board. The original Gemini 4-axis board can be expanded to 8-axis to meet the needs of more 3D printers. This expansion board would have limited functionality in a stand alone configuration as a 3D printer motherboard because it does not include heating and temperature measurement functions.

### Features

 - MCU: RPI RP2040
 - Communication: USB
 - 12/24V input
 - 2A 5V power supply
 - Drivers: 4 - TMC2209 onboard drivers
  - Sensorless Homing is not supported
 - Interfaces
  - 2 CNC Fans with replacable Fly MOS.
  - 1 Full power fan
  - RGB LED port 
  - 3 Limit switch inputs

### Dimensions

  {% 
  include image.html 
  file=fly_rpfmex_img2
  url=fly_rpfmex_url2
  alt=fly_rpfmex_cap2
  caption=fly_rpfmex_cap2
  %}

### BOM

  {% 
  include image.html 
  file=fly_rpfmex_img3
  url=fly_rpfmex_url3
  alt=fly_rpfmex_cap3
  caption=fly_rpfmex_cap3
  %}

   - Fly RPFMEX Board
   - 4 heatinks for TMC2209 drivers
   - JST-XH connectors and crimp terminals
   - Fly MOS
   - USB C Cable