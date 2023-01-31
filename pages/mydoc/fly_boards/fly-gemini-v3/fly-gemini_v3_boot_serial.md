---
title: Fly Gemini V3 bootloader serial cable
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly Gemini bootloader serial cable"
sidebar: mydoc_sidebar
permalink: fly-gemini_v3_boot_serial.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: "Fly-Gemini V3" 

mcu_oem_serial_img1: "fly-gemini-v2/mcu_oem_bootloader_cable_zh2.jpg"
mcu_oem_serial_cap1: "Serial Cable ZH2 header"

mcu_oem_serial_img2: "fly-gemini-v2/mcu_oem_bootloader_cable_screen1.jpg"
mcu_oem_serial_cap2: "Serial Cable screen1 header"

mcu_oem_serial_img3: "fly-gemini-v2/mcu_oem_bootloader_cable_installed.jpg"
mcu_oem_serial_cap3: "Serial Cable installed"

---

{% capture title %}{{ page.title }}{% endcapture %}
{% capture mcu %}{{ page.mcu }}{% endcapture %}

{% capture boardname %}{{ page.boardname }}{% endcapture %}

{% capture mcu_oem_serial_img1 %}{{page.mcu_oem_serial_img1 }}{% endcapture %}
{% capture mcu_oem_serial_cap1 %}{{page.mcu_oem_serial_cap1 }}{% endcapture %}
{% capture mcu_oem_serial_url1 %} .\images\{{ page.mcu_oem_serial_img1 }}{% endcapture %}

{% capture mcu_oem_serial_img2 %}{{page.mcu_oem_serial_img2 }}{% endcapture %}
{% capture mcu_oem_serial_cap2 %}{{page.mcu_oem_serial_cap2 }}{% endcapture %}
{% capture mcu_oem_serial_url2 %} .\images\{{ page.mcu_oem_serial_img2 }}{% endcapture %}

{% capture mcu_oem_serial_img3 %}{{page.mcu_oem_serial_img3 }}{% endcapture %}
{% capture mcu_oem_serial_cap3 %}{{page.mcu_oem_serial_cap3 }}{% endcapture %}
{% capture mcu_oem_serial_url3 %} .\images\{{ page.mcu_oem_serial_img3 }}{% endcapture %}

## Building the serial cable

 - The serial cable needs to connect the ZH2 and screen1 headers

   - ZH2 RX to Screen1 TX

   - ZH2 TX to Screen1 RX  

   {%   
   include image.html 
   file=mcu_oem_serial_img1
   url=mcu_oem_serial_url1
   alt=mcu_oem_serial_cap1
   caption=mcu_oem_serial_cap1
   %} 

   {%   
   include image.html 
   file=mcu_oem_serial_img2
   url=mcu_oem_serial_url2
   alt=mcu_oem_serial_cap2
   caption=mcu_oem_serial_cap2
   %} 

 - Crimp the JST-XH connectors on the included 4 pin pigtail connector. The wires should be long enough to reach but you can extend them if you feel the need. 

 - Remove the extra 2 wires or tape them off as they connect to +5v and ground on the ZH2 header. 

   {%   
   include image.html 
   file=mcu_oem_serial_img3
   url=mcu_oem_serial_url3
   alt=mcu_oem_serial_cap3
   caption=mcu_oem_serial_cap3
   %} 

{% include custom/can/sht_links.html %}