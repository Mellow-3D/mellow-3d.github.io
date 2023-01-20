---
title: Fly Pi Pins
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly Pi Pin map"
sidebar: mydoc_sidebar
permalink: fly_pi_pins.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: "Fly-Pi" 

fly_pi_img0: "fly-pi/fly_pi_pin_diagram.webp"
fly_pi_cap0: "Fly Pi pin diagram"

fly_pi_img1: "fly-pi/pins.png"
fly_pi_cap1: "Fly Pi 40 Pin Header"

fly_pi_img2: "fly-pi/fly_pi_gpio_pins.jpg"
fly_pi_cap2: "Fly Pi GPIO header pin numbers"

fly_pi_img3: "fly-pi/fly_pi_core_Fan_socket.jpg"
fly_pi_cap3: "Fly Pi Core Fan Socket"

fly_pi_img4: "fly-pi/fly_pi_vcc_socket.jpg"
fly_pi_cap4: "Fly Pi VCC Socket"

fly_pi_img5: "fly-pi/canhat.png"
fly_pi_cap5: "Fly Pi CANhat socket"

---


    {% capture mcu %}{{ page.mcu }}{% endcapture %}

    {% capture mcufile %}{{ page.mcufile }}{% endcapture %}

    {% capture fly_pi_img0 %}{{page.fly_pi_img0 }}{% endcapture %}
    {% capture fly_pi_cap0 %}{{page.fly_pi_cap0 }}{% endcapture %}
    {% capture fly_pi_url0 %} .\images\{{ page.fly_pi_img0 }}{% endcapture %}

    {% capture fly_pi_img1 %}{{page.fly_pi_img1 }}{% endcapture %}
    {% capture fly_pi_cap1 %}{{page.fly_pi_cap1 }}{% endcapture %}
    {% capture fly_pi_url1 %} .\images\{{ page.fly_pi_img1 }}{% endcapture %}

    {% capture fly_pi_img2 %}{{page.fly_pi_img2 }}{% endcapture %}
    {% capture fly_pi_cap2 %}{{page.fly_pi_cap2 }}{% endcapture %}
    {% capture fly_pi_url2 %} .\images\{{ page.fly_pi_img2 }}{% endcapture %}

    {% capture fly_pi_img3 %}{{page.fly_pi_img3 }}{% endcapture %}
    {% capture fly_pi_cap3 %}{{page.fly_pi_cap3 }}{% endcapture %}
    {% capture fly_pi_url3 %} .\images\{{ page.fly_pi_img3 }}{% endcapture %}

    {% capture fly_pi_img4 %}{{page.fly_pi_img4 }}{% endcapture %}
    {% capture fly_pi_cap4 %}{{page.fly_pi_cap4 }}{% endcapture %}
    {% capture fly_pi_url4 %} .\images\{{ page.fly_pi_img4 }}{% endcapture %}

    {% capture fly_pi_img5 %}{{page.fly_pi_img5 }}{% endcapture %}
    {% capture fly_pi_cap5 %}{{page.fly_pi_cap5 }}{% endcapture %}
    {% capture fly_pi_url5 %} .\images\{{ page.fly_pi_img5 }}{% endcapture %}

## Fly Pi Pin Diagram

{% 
include image.html 
file=fly_pi_img0
url=fly_pi_url0
alt=fly_pi_cap0
caption=fly_pi_cap0
%}

### 40 Pin GPIO Header

{% 
include image.html 
file=fly_pi_img1
url=fly_pi_url1
alt=fly_pi_cap1
caption=fly_pi_cap1
%}

- Refrence for the locatipons of Pin a and Pin 40. See above chart for GPIO pin functions. 
{% 
include image.html 
file=fly_pi_img2
url=fly_pi_url2
alt=fly_pi_cap2
caption=fly_pi_cap2
%}


### ZH TFT Headers

{% include custom/sbc/zh_sockets_datatable.html %}

### Core Fan Header
- The Fly Pi Fan header supplies +5v for a CPU cooling fan.

{% 
include image.html 
file=fly_pi_img3
url=fly_pi_url3
alt=fly_pi_cap3
caption=fly_pi_cap3
%}

# VCC header
- Supplies line level voltage

{% 
include image.html 
file=fly_pi_img4
url=fly_pi_url4
alt=fly_pi_cap4
caption=fly_pi_cap4
%}

# CAN Hat
 - The red pins of CANHat correspond to the blue female headers of FLY-Pi, and the black ones correspond to black (inserting them backwards will short out the CANHat)
 - The CAN interface of FLY-Pi has an incorrect silk screen, please connect according to the figure below. 

{% 
include image.html 
file=fly_pi_img5
url=fly_pi_url5
alt=fly_pi_cap5
caption=fly_pi_cap5
%}