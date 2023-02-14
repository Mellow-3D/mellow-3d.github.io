---
title: Set up the Fly Pi for use with the Fly-Puppet.
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly-Puppet with Fly pi"
sidebar: mydoc_sidebar
permalink: fly-puppet_klipper_fly.html
folder: mydoc
comments: false
toc: true
datatable: true


boardname: Fly-Puppet
firmware: Linux MCU
version: ""
host: Fly Pi
sd: "Fly Pi"
micro: "Linux Process"

linux_mcu_img1: "fly-puppet/fly-puppet_klipper_host_fw.png"
linux_mcu_cap1: "Configure Linux MCU Firmware"

cm4_img1: "fly-puppet/pi_boot.png"
cm4_cap1: "Booting the Raspberry Pi"

cm4_img2: "fly-puppet/pi_boot_running.png"
cm4_cap2: "Rasberry Pi Boot Success"

rpi_config_img1: "fly-puppet/dt_pverlay.png"
rpi_config_cap1: "Edit config.txt"

rpi_config_img2: "fly-puppet/fly-puppet_wifi.png"
rpi_config_cap2: "Edit WIFI configuration file"

puppetpi_img1: "fly-puppet/puppet-flypi.png"
puppetpi_cap1: "Mounting the Fly Pi to the Fly puppet"




---

## Configuring and installing {{page.host}} for the {{page.boardname}}

{% include custom/mcu/rp2040/cm4_mounting.html %}

###  Configure Fly OS on SD or M2WE 
- Folllow the Fly Pi setup guides to Configure Fly OS on an [SD card](./fly_pi_sbc.html) or the [M2WE](./fly_pi_m2we.html). When setup is complete return to this page and perform the Linux MCU setup.

{% include custom/mcu/rp2040/linux_mcu_klipper_menuconfig.html %}

{% include custom/mcu/rp2040/linux_mcu_klipper_makeflash.html %}