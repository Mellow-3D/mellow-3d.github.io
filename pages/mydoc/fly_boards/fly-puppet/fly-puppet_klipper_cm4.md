---
title: Set up the Rasberry Pi CM4 for use with the Fly-Puppet.
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly-Puppet with CM4"
sidebar: mydoc_sidebar
permalink: fly-puppet_klipper_cm4.html
folder: mydoc
comments: false
toc: true
datatable: true


boardname: Fly-Puppet
firmware: Linux MCU
version: ""
host: Rasberry Pi CM4
micro: "Linux Process"
sd: "Fly-Puppet SD Slot"

linux_mcu_img1: "fly-puppet/fly-puppet_klipper_host_fw.png"
linux_mcu_cap1: "Configure Linux MCU Firmware"



cm4_img1: "fly-puppet/pi_boot.png"
cm4_cap1: "Booting the CM4"

cm4_img2: "fly-puppet/pi_boot_running.png"
cm4_cap2: "Rasberry Pi Boot Success"

rpi_config_img1: "fly-puppet/dt_pverlay.png"
rpi_config_cap1: "Edit config.txt"

rpi_config_img2: "fly-puppet/fly-puppet_wifi.png"
rpi_config_cap2: "Edit WIFI configuration file"

puppetpi_img1: "fly-puppet/puppet-cm4.png"
puppetpi_cap1: "Mounting the CM4 to the Fly puppet"




---

## Configuring and installing {{page.host}} for the {{page.boardname}}

{% include custom/mcu/rp2040/cm4_mounting.html %}

{% include custom/mcu/rp2040/cm4_build_os.html %}

{% include custom/mcu/rp2040/rpi_configure_os.html %}

{% include custom/mcu/rp2040/linux_mcu_klipper_menuconfig.html %}

{% include custom/mcu/rp2040/linux_mcu_klipper_makeflash.html %}