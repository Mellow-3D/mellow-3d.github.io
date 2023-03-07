---
title: Fly Pi Klipper Core Fan configuration
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly Pi Core Fan Setup in Klipper"
sidebar: mydoc_sidebar
permalink: fly_pi_core_fan.html
folder: mydoc
comments: false
toc: false
datatable: true

fly_pi_fan_img1: "fly-pi/fly_pi_core_Fan_socket.jpg"
fly_pi_fan_cap1: "Fly Pi Core Fan"



---

    {% capture mcu %}{{ page.mcu }}{% endcapture %}

    {% capture mcufile %}{{ page.mcufile }}{% endcapture %}

    {% capture fly_pi_fan_img1 %}{{page.fly_pi_fan_img1 }}{% endcapture %}
    {% capture fly_pi_fan_cap1 %}{{page.fly_pi_fan_cap1 }}{% endcapture %}
    {% capture fly_pi_fan_url1 %} .\images\{{ page.fly_pi_fan_img1 }} {% endcapture %}



## Klipper Core Fan Configuration

The Fly Pi has a 5V controllable fan interface on board, which is used for CPU Cooling. The wiring method is as shown in the figure below       


### Pin location

{% 
include image.html 
file=fly_pi_fan_img1
url=fly_pi_fan_url1
alt=fly_pi_fan_cap1
caption=fly_pi_fan_cap1
%}

### Klipper Configuration
 - Add the following to your printer.cfg to enable the core fan. 
 - Klipper Host MCU is enabled by default in Fly OS. 

```
[mcu host]
serial: /tmp/klipper_host_mcu
```

```
[temperature_fan core_fan]
pin: host:gpio3
max_power: 1.0
sensor_type: temperature_host
control:watermark
target_temp: 48
min_temp: 0
max_temp: 90
off_below: 0.10
kick_start_time: 0.50
max_speed: 0.8
min_speed: 0.3
```



{% include custom/can/sht_links.html %}