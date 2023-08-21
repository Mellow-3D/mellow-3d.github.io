---
title: Katapult Configuration for the Fly-ADXL345-USB on USB
tags: []
keywords: 
last_updated: 21/08/2023
summary: "How to Configure Katapult for USB Operation on the Fly-ADXL345-USB"
sidebar: mydoc_sidebar
permalink: fly_adxl345_usb_canboot_usb.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: Fly-ADXL345-USB
firmware: USB
mcu: "rp2040"
version: v1
kconfig_name: adxl345
architecture: "(Raspberry Pi RP2040)"
flash: "(W25Q080 with CLKDIV 2)"
deployment: "(Do not build)"
communication: "(USB)"
gpio_bootloader_set: "()"
support_bootloader_entry: "[*]"
enable_bootloader_gpio: "[&nbsp;]"
enable_status: "[&nbsp;]"
status_pin: ""
board_type: "toolboard"
katapult_file: "katapult.uf2"

katapult_img1: "katapult/rp2040_usb.png"
katapult_cap1: "Katapult Menu Config USB"

katapult_img2: "fly_adxl345_usb/boot_button.png"
katapult_cap2: "Fly-ADXL345-USB Boot Button Location"

katapult_img3: "fly-sb2040_v1/fly-sb2040_lsusb_screenshot.png"
katapult_cap3: "lsusb Results"

installKlipperURL: "./fly_adxl345_usb_klipper_usb.html"
installKlipperName: "Klipper for USB configuration section"

---
{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}

{% include custom/katapult/compile.html %}

{% include custom/katapult/rp2040_usb_flash.html %}

{% include custom/mcu/adxl345_usb/adxl345_usb_links.html %}
