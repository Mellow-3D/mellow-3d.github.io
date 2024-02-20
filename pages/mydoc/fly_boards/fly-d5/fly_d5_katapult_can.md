---
title: Katapult Configuration for the Fly-D5 on CAN
tags: []
keywords: 
last_updated: 19/02/2024
summary: "How to Configure Katapult for CAN bus Operation on the Fly-D5"
sidebar: mydoc_sidebar
permalink: fly_D5_katapult_can.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-D5
firmware: CANbus
mcu: "STM32"
kconfig_name: d5
architecture: "(STMicroelectronics STM32)"
processor: "(STM32F072)"
deployment: "(8KiB bootloader)"
clock: "(8 MHz crystal)"
communication: "(CAN bus (on PB8/PB9))"
application_offset: "(8KiB offset)"
can_bus_speed: "(1000000)"
gpio_bootloader_set: "()"
support_bootloader_entry: "[*]"
enable_bootloader_gpio: "[&nbsp;]"
enable_status: "[&nbsp;]"
board_type: "mainboard"
katapult_file: "katapult.bin"
dfu_method: buttons

katapult_img1: "katapult/stm32f072_can_deployer_pb8pb9.png"
katapult_cap1: "Katapult Menu Config CAN"

katapult_img2: "dfu/stm32_dfu.png"
katapult_cap2: "STM32 DFU Mode Detected"

katapult_img3: "dfu/stm32_dfu_flash.png"
katapult_cap3: "DFU Mode Flash Successful"

installKlipperURL: "./fly_d5_klipper_can.html"
installKlipperName: "Klipper for CAN bus configuration section"

---

## Configuring and installing Katapult bootloader for CAN bus

{% include custom/katapult/compile.html %}

{% include custom/katapult/flash_dfu.html %}

{% include custom/mcu/d5/fly_d5_links.html %}
