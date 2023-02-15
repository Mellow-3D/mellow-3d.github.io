---
title: Fly Puppet General Information
tags: []
keywords: 
last_updated: 20/10/2022
summary: "General information regarding the Fly Puppet"
sidebar: mydoc_sidebar
permalink: fly-puppet.html
folder: mydoc
comments: false
toc: false
datatable: true


boardname: "Fly Puppet"

fly_puppet_img1: "fly-puppet/fly_puppet.png"
fly_puppet_cap1: "Fly-puppet board"

fly_puppet_img2: "fly-puppet/fly-puppet_dimensions.webp"
fly_puppet_cap2: "Fly-puppet board dimensions"

fly_puppet_img3: "fly-puppet/fly-puppet_bom.webp"
fly_puppet_cap3: "Fly-puppet BOM"


---
    {% capture boardname %}{{ page.boardname }}{% endcapture %}

    {% capture mcu %}{{ page.mcu }}{% endcapture %}

    {% capture fly_puppet_img1 %}{{page.fly_puppet_img1 }}{% endcapture %}
    {% capture fly_puppet_cap1 %}{{page.fly_puppet_cap1 }}{% endcapture %}
    {% capture fly_puppet_url1 %} .\images\{{ page.fly_puppet_img1 }} {% endcapture %}

    {% capture fly_puppet_img2 %}{{page.fly_puppet_img2 }}{% endcapture %}
    {% capture fly_puppet_cap2 %}{{page.fly_puppet_cap2 }}{% endcapture %}
    {% capture fly_puppet_url2 %} .\images\{{ page.fly_puppet_img2 }} {% endcapture %}

    {% capture fly_puppet_img3 %}{{page.fly_puppet_img3 }}{% endcapture %}
    {% capture fly_puppet_cap3 %}{{page.fly_puppet_cap3 }}{% endcapture %}
    {% capture fly_puppet_url3 %} .\images\{{ page.fly_puppet_img3 }} {% endcapture %}

## Overview 

  {% 
  include image.html 
  file=fly_puppet_img1
  url=fly_puppet_url1
  alt=fly_puppet_cap1
  caption=fly_puppet_cap1
  %}

## Description
This page covers any general information for the {{boardname}} board.  
Avaliable from the Mellow store on [Aiexpress](https://www.aliexpress.us/item/3256804305416750.html)

In order to meet the needs of customers using RP2040 5-axis, we made a fly-puppet motherboard. If you use Raspberry Pi cm4, then this motherboard will become an integrated board of Raspberry Pi 4 + 3D printer motherboard, and run klipper firmware directly. At the same time, it can also connect to Fly Pi, Raspberry PI 3/3b/4b through the 40p GPIO header. 5-axis fits most machines on the market today, and it's a very interesting board.

### Features
 - Supports mounting Rasberry Pi CM4, 4B, 3B, 3, and Fly Pi 
 - MCU: RPI RP2040
 - Communication: UART
 - 12/24V input
 - 3A 5V power supply
 - Drivers supported: A4988, LV8729, DRV8225, TMC2208, 2209, & 5160
 - Interfaces
  - 2 CNC Fans with replacable Fly MOS
  - 1 Full power fan
  - Bed and Hotend Tempreture
  - RGB LED port 
  - BLtouch port
  - 3 Limit switch inputs
  - HDMI, CSI, DSI, USB and Ethernet with CM4

### Dimensions

  {% 
  include image.html 
  file=fly_puppet_img2
  url=fly_puppet_url2
  alt=fly_puppet_cap2
  caption=fly_puppet_cap2
  %}

### BOM

  {% 
  include image.html 
  file=fly_puppet_img3
  url=fly_puppet_url3
  alt=fly_puppet_cap3
  caption=fly_puppet_cap3
  %}

   - Fly Puppet Board
   - Fuse
   - JST-XH connectors and crimp terminals
   - Fly MOS
   - USB C Cable
   - Serial header pigtail
   - Jumpers