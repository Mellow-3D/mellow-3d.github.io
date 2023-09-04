---
title: Klipper Configuration for the Fly-SB2040-V1 on CANbus
tags: []
keywords: 
last_updated: 04/09/2023
summary: "Klipper Configuration for the Fly-SB2040-V1 on CANbus"
sidebar: mydoc_sidebar
permalink: fly_sb2040_v1_klipper_can.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: Fly-SB2040-V1
firmware: CANbus
mcu: "rp2040"
version: v1
kconfig_name: sb2040v1
low_level: "[*]"
architecture: "(Raspberry Pi RP2040)"
bootloader_offset: "(16KiB bootloader)"
communication: "(CAN bus)"
can_rx: "(4)"
can_tx: "(5)"
can_bus_speed: "(1000000)"
gpio_startup: "(gpio24)"
board_type: "toolboard"
klipper_file: "klipper.uf2"
120rurl: "./fly_sb2040_v1_120r.html"
state: "install"

klipper_img1: "klipper/rp2040_can_gpio24.png"
klipper_cap1: "Klipper Menu Config CAN"

klipper_img2: "fly-super8/flash-can_query.png"
klipper_cap2: "Flash Can Query"

klipper_img3: "fly-super8/fly-super8_klipper_canboot_burn.png"
klipper_cap3: "Burn Klipper firmware over CANbus"

---

{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_canboot_can.html %}

{% include custom/mcu/sb2040v1/sb2040_v1_links.html %}
