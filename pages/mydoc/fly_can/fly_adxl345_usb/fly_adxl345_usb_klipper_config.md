---
title: Fly-ADXL345-USB Klipper configuration
tags: []
keywords: 
last_updated: 21/08/2023
summary: "Sample Configuration files for the Fly-ADXL345-USB"
sidebar: mydoc_sidebar
permalink: fly_adxl345_usb_klipper_config.html
folder: mydoc
comments: false
toc: true
datatable: true
---

## printer.cfg File Changes

Add the following line near the beginning of your printer.cfg

```text
[include accelerometer.cfg]
```

This way, when the accelerometer isn't connected the whole file can be commented out.  

### accelerometer.cfg

- [Download a sample file containing these sections](./files/fly_adxl345_usb/accelerometer.cfg)

Create a file called accerlerometer.cfg in your configuration files.  

```text
[mcu adxl]
serial: /dev/serial/by-id/usb-Klipper_rp2040_XXXXXXXXXXXXXXXXXXXXX

[adxl345]
cs_pin: adxl:gpio9
spi_software_sclk_pin: adxl:gpio10
spi_software_mosi_pin: adxl:gpio11
spi_software_miso_pin: adxl:gpio12

[resonance_tester]
accel_chip:adxl345
probe_points:
    150,150,20
```

{% include custom/mcu/adxl345_usb/adxl345_usb_links.html %}
