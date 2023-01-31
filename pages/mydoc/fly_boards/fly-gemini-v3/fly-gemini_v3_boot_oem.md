---
title: Fly Gemini V3 OEM bootloader
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly Gemini OEM bootloader"
sidebar: mydoc_sidebar
permalink: fly-gemini_v3_boot_oem.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: "Fly-Gemini V3" 

mcu_oem_bootloader_img1: "fly-gemini-v2/mcu_oem_bootloader_cable_installed.jpg"
mcu_oem_bootloader_cap1: "Serial Cable installed"

mcu_oem_bootloader_img2: "fly-gemini-v3/fly-gemini_v3_dfu_jumpers.jpg"
mcu_oem_bootloader_cap2: "Install boot0 and boot1 jumpers"

mcu_oem_bootloader_img3: "fly-sht36-42/sht-36_42_lsusb_screenshot.png"
mcu_oem_bootloader_cap3: "Run lsusb"


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

### Install the DFU jumpers

- Install the boot0 and boot1 jumpers as shown.

  {%   
  include image.html 
  file=mcu_oem_bootloader_img2
  url=mcu_oem_bootloader_url2
  alt=mcu_oem_bootloader_cap2
  caption=mcu_oem_bootloader_cap2
  %} 


### Upload the HID Bootloader
- power on the {{boardname}}
- Download the [hid_bootloader.bin](https://github.com/Mellow-3D/Fly-Gemini-V3/tree/main/Bootloader) file from the Mellow github.
- Use an FTP client to upload the hid_bootloader.bin file to the Fly home folder /home/fly/ on the Gemini V3 klipper host. 

### Flash the bootloader

- Using Putty open an SSH session to the {{boardname}}

- Run lsusb to see if the connection is successful, Verify the USB ID indicated DFU mode. If the MCU is not in DFU press the reset button a few times and run again. If that fails verify the DFU jumpers are installed correctly. 

  {%   
  include image.html 
  file=mcu_oem_bootloader_img3
  url=mcu_oem_bootloader_url3
  alt=mcu_oem_bootloader_cap3
  caption=mcu_oem_bootloader_cap3
  %} 


- Erase and Burn the firmware.
 ```
 sudo dfu-util -a 0 -D /home/fly/hid_bootloader.bin --dfuse-address 0x08000000:force:mass-erase:leave -d 0483:df11
  ```

- Wait for the flash to complete. This can take a minute or two. 

  
- If successfull shut down the {{boardname}}
  ```
  shutdown
  ```
- Remove the bootO jumper and boot1 jumper. 

- Continue on to flashing the MCU for [USB to CAN bridge mode](./fly-gemini_v3_klipper_usbtocan.html) or [USB](./fly-gemini_v3_klipper_mcu_usb.html)

{% include custom/can/sht_links.html %}