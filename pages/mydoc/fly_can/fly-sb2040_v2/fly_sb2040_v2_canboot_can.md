---
title: Katapult Configuration for the Fly-SB2040-V2 on CANbus
tags: []
keywords: 
last_updated: 17/08/2023
summary: "How to Configure Katapult for CANbus Operation on the Fly-SB2040-V2"
sidebar: mydoc_sidebar
permalink: fly_sb2040_v2_canboot_can.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: Fly-SB2040-V2
firmware: CANbus
mcu: "rp2040"
version: v1
kconfig_name: sb2040v2
architecture: "(Raspberry Pi RP2040)"
flash: "(W25Q080 with CLKDIV 2)"
deployment: "(Do not build)"
communication: "(CAN bus)"
can_rx: "(4)"
can_tx: "(5)"
can_bus_speed: "(500000)"
gpio_bootloader_set: "()"
support_bootloader_entry: "[*]"
enable_bootloader_gpio: "[&nbsp;]"
enable_status: "[*]"
status_pin: "(gpio24)"
board_type: "toolboard"
katapult_file: "katapult.uf2"

katapult_img1: "katapult/rp2040_can_gpio24.png"
katapult_cap1: "Katapult Menu Config CAN"

katapult_img2: "fly-sb2040_v1/sb2040_button.png"
katapult_cap2: "Fly-SB2040-V2 Boot Button Location"

katapult_img3: "fly-sb2040_v1/fly-sb2040_lsusb_screenshot.png"
katapult_cap3: "lsusb Results"

installKlipperURL: "./fly_sb2040_v1_klipper_can.html"
installKlipperName: "Klipper for CANbus configuration section"

---
{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}

{% include custom/katapult/compile.html %}

{% include custom/katapult/rp2040_usb_flash.html %}

{% include custom/mcu/sb2040v2/sb2040_v2_links.html %}
