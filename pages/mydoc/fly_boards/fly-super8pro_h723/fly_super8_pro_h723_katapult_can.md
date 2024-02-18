---
title: Katapult Configuration for the Fly-Super8Pro H723 on CAN
tags: []
keywords: 
last_updated: 18/02/2024
summary: "How to Configure Katapult for CAN bus Operation on the Fly-Super8Pro H723"
sidebar: mydoc_sidebar
permalink: fly_super8_pro_h723_canboot_can.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-Super8Pro
firmware: CANbus
mcu: "STM32"
kconfig_name: super8proh723
architecture: "(STMicroelectronics STM32)"
processor: "(STM32H723)"
deployment: "(128KiB bootloader (SKR SE BX v2.0))"
clock: "(25 MHz crystal)"
communication: "(CAN bus (on PB8/PB9))"
application_offset: "(128KiB offset)"
can_bus_speed: "(1000000)"
gpio_bootloader_set: "()"
support_bootloader_entry: "[*]"
enable_bootloader_gpio: "[&nbsp;]"
enable_status: "[&nbsp;]"
board_type: "mainboard"
katapult_file: "deployer.bin"

katapult_img1: "katapult/stm32h723_can_deployer_pb8pb9.png"
katapult_cap1: "Katapult Menu Config CAN"

katapult_img2: "fly-super8_pro/fly_super8pro_sd_card.png"
katapult_cap2: "Fly-Super8Pro SD card"

katapult_img3: "fly-super8_pro/fly_super8pro_reset.png"
katapult_cap3: "Fly-Super8Pro reset button"

installKlipperURL: "./fly_super8_pro_klipper_can.html"
installKlipperName: "Klipper for CAN bus configuration section"

---

## Configuring and installing Katapult bootloader for CAN bus

{% include custom/katapult/compile.html %}

## USB Power Jumper

Add a jumper as shown below to ensure the board can be powered from USB power.  

{% include image.html file="fly-super8_pro/fly_super8pro_usb_power.png" alt="Fly-Super8Pro H723 USB Power Jumper" caption="Fly-Super8Pro H723 USB Power Jumper" %}

{% include custom/katapult/flash_deployer.html %}

{% include custom/mcu/super8/fly_super8pro_links.html %}
