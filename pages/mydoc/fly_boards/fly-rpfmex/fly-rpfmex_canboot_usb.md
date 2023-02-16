---
title: Fly RPFMEX CanBoot bootloader for USB
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly RPFMEX CanBoot bootloader for USB"
sidebar: mydoc_sidebar
permalink: fly-rpfmex_canboot_usb.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: "Fly RPFMEX"
firmware: usb
ver: "" 
klipperurl: "[Compiling Klipper](./fly-rpfmex_klipper_usb.html)"

com: "USB"

cancom_img1: "fly-rpfmex/fly-rpfmex_canboot_menuconfig.png"
cancom_cap1: "RPFMEX CanBoot Menu Config for USB"

canburn_img1: "fly-rpfmex/fly_rpfmex_boot.png"
canburn_cap1: "Fly RPFMEX boot button"

canburn_img2: "fly-puppet/fly_puppet_klipper_mkae_flash_rpi_boot.png"
canburn_cap2: "RPFMEX lsusb"

canburn_img3: "fly-puppet/fly_puppet_klipper_mkae_flash_rpi_boot.png"
canburn_cap3: "RPFMEX lsusb"

---

## Configuring and installing CanBoot bootloader for USB

{% include custom/mcu/rp2040/rp2040_canboot_compile.html %}

{% include custom/mcu/rp2040/rp2040_canboot_burn.html %}

{% include custom/can/sht_links.html %}

