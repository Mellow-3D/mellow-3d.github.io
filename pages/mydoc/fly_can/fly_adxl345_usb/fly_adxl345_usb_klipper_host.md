---
title: Fly-ADXL345-USB Klipper host configuration
tags: []
keywords: 
last_updated: 24/07/2023
summary: "Fly-ADXL345-USB Klipper host preparation"
sidebar: mydoc_sidebar
permalink: fly_adxl345_usb_klipper_host.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: "Fly-ADXL345-USB" 

---

## Overview

In preparation for using the Fly-ADXL345-USB, some software is required to be installed on your SBC.  

### Software installation

Please run the following lines

```console
sudo apt update
sudo apt install python3-numpy python3-matplotlib libatlas-base-dev
~/klippy-env/bin/pip install -v numpy
```

{% include custom/mcu/adxl345_usb/adxl345_usb_links.html %}
