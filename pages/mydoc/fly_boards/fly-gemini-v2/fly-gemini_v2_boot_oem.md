---
title: Fly Gemini V2 OEM bootloader
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly Gemini OEM bootloader"
sidebar: mydoc_sidebar
permalink: fly-gemini_v2_boot_oem.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: "Fly-Gemini V2" 

mcu_oem_bootloader_img1: "fly-gemini-v2/mcu_oem_bootloader_cable_installed.jpg"
mcu_oem_bootloader_cap1: "Serial Cable installed"

mcu_oem_bootloader_img2: "fly-gemini-v2/mcu_oem_bootloader_boot0.png"
mcu_oem_bootloader_cap2: "Install boot0 jumper"

mcu_oem_bootloader_img3: "fly-gemini-v2/mcu_oem_bootloader_boot1.png"
mcu_oem_bootloader_cap3: "Install boot1 jumper"

mcu_oem_bootloader_img4: "fly-gemini-v2/gemini_v2_sbc_usb.png"
mcu_oem_bootloader_cap4: "Connect USB cable to the USB C port in the red box"

---

{% capture title %}{{ page.title }}{% endcapture %}
{% capture mcu %}{{ page.mcu }}{% endcapture %}

{% capture boardname %}{{ page.boardname }}{% endcapture %}

{% capture mcu_oem_bootloader_img1 %}{{page.mcu_oem_bootloader_img1 }}{% endcapture %}
{% capture mcu_oem_bootloader_cap1 %}{{page.mcu_oem_bootloader_cap1}}{% endcapture %}
{% capture mcu_oem_bootloader_url1 %} .\images\{{ page.mcu_oem_bootloader_img1 }}{% endcapture %}

{% capture mcu_oem_bootloader_img2 %}{{page.mcu_oem_bootloader_img2 }}{% endcapture %}
{% capture mcu_oem_bootloader_cap2 %}{{page.mcu_oem_bootloader_cap2 }}{% endcapture %}
{% capture mcu_oem_bootloader_url2 %} .\images\{{ page.mcu_oem_bootloader_img2 }}{% endcapture %}

{% capture mcu_oem_bootloader_img3 %}{{page.mcu_oem_bootloader_img3 }}{% endcapture %}
{% capture mcu_oem_bootloader_cap3 %}{{page.mcu_oem_bootloader_cap3 }}{% endcapture %}
{% capture mcu_oem_bootloader_url3 %} .\images\{{ page.mcu_oem_bootloader_img3 }}{% endcapture %}

{% capture mcu_oem_bootloader_img4 %}{{page.mcu_oem_bootloader_img4 }}{% endcapture %}
{% capture mcu_oem_bootloader_cap4 %}{{page.mcu_oem_bootloader_cap4 }}{% endcapture %}
{% capture mcu_oem_bootloader_url4 %} ./images/{{ page.mcu_oem_bootloader_img4 }}{% endcapture %}

## Restoring the factory bootloader

###  Install the serial cable 

- Install the serial cable as pictured connecting header ZH2 RX and TX to header Screen1 TX and RX

   {%   
   include image.html 
   file=mcu_oem_bootloader_img1
   url=mcu_oem_bootloader_url1
   alt=mcu_oem_bootloader_cap1
   caption=mcu_oem_bootloader_cap1
   %} 

- [See instructions for building the cable](./fly-gemini_v2_boot_serial.html) 

### Install the DFU jumpers

- Boot0 jumper inserted

  {%   
  include image.html 
  file=mcu_oem_bootloader_img2
  url=mcu_oem_bootloader_url2
  alt=mcu_oem_bootloader_cap2
  caption=mcu_oem_bootloader_cap2
  %} 

- Boot1 jumper inserted on the pins to the right side. 

  {%   
  include image.html 
  file=mcu_oem_bootloader_img3
  url=mcu_oem_bootloader_url3
  alt=mcu_oem_bootloader_cap3
  caption=mcu_oem_bootloader_cap3
  %} 

### Connect USB cable to the {{boardname}}

- Connect the {{boardname}} to your PC using the SBC USB C port. 
  
  {%   
  include image.html 
  file=mcu_oem_bootloader_img4
  url=mcu_oem_bootloader_url4
  alt=mcu_oem_bootloader_cap4
  caption=mcu_oem_bootloader_cap4
  %} 

### Flash the bootloader

- Using Putty open a telnet session to the CH340 com port. 
- Run the following stm32flash command in the telnet session. 
  ```
  stm32flash -w /root/.BL/Gemini_v1.1_BL.bin -v -g 0 /dev/ttyS2
  ```
- Wait for the flash to complete
  Add screen shot of flash complete 
  
- Shut down the {{boardname}}
  ```
  shutdown
  ```
- Disconect the USB cable, remove both boot jumpers and the serial cable.     

{% include custom/can/sht_links.html %}