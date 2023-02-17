---
title: Fly HV-TMC5160 Pro External Driver
tags: []
keywords: 
last_updated: 20/10/2022
summary: "General information regarding the Fly HV-TMC5160 Pro"
sidebar: mydoc_sidebar
permalink: fly_hv-tmc5160pro_general.html
folder: mydoc
comments: false
toc: true
datatable: true

driver_img1: "fly-5160_pro/fly-hv5160pro.webp"
driver_cap1: "Fly-TMC5160 Pro Overview"

driver_img2: "fly-5160_pro/fly-hv5160pro_dimensions.webp"
driver_cap2: "Fly-TMC5160 Pro Dimensions"

driver_img3: "fly-5160_pro/fly-hv5160pro_stepper_wiring.webp"
driver_cap3: "Fly-TMC5160 Pro Stepper Wiring"

driver_img4: "fly-5160_pro/fly-hv5160pro_fan.webp"
driver_cap4: "Fly-TMC5160 Pro Fan"

driver_img5: "fly-5160_pro/fly-hv5160pro_spi_jumper.webp"
driver_cap5: "Fly-TMC5160 Pro SPI Jumpers"

driver_img6: "fly-5160_pro/5160pro_diag.png"
driver_cap6: "Fly-TMC5160 Pro Diag Pin"

driver_img7: "fly-5160_pro/fly-hv5160pro_firmware.webp"
driver_cap7: "Fly-TMC5160 Pro Firmware Settings"

driver_img8: "fly-5160_pro/fly-hv5160pro_front_back.webp"
driver_cap8: "Fly-TMC5160 Pro Front & Back"

driver_img9: "fly-5160_pro/fly-hv5160pro_stepper_adapter.webp"
driver_cap9: "Fly-TMC5160 Pro Stepper Adapter"

driver_img10: "fly-5160_pro/fly-hv5160pro_bom.webp"
driver_cap10: "Fly-TMC5160 Pro BOM"



---

    {% capture driver_img1 %}{{page.driver_img1 }}{% endcapture %}
    {% capture driver_cap1 %}{{page.driver_cap1 }}{% endcapture %}
    {% capture driver_url1 %} .\images\{{ page.driver_img1 }} {% endcapture %}

    {% capture driver_img2 %}{{page.driver_img2 }}{% endcapture %}
    {% capture driver_cap2 %}{{page.driver_cap2 }}{% endcapture %}
    {% capture driver_url2 %} .\images\{{ page.driver_img2 }} {% endcapture %}

    {% capture driver_img3 %}{{page.driver_img3 }}{% endcapture %}
    {% capture driver_cap3 %}{{page.driver_cap3 }}{% endcapture %}
    {% capture driver_url3 %} .\images\{{ page.driver_img3 }} {% endcapture %}

    {% capture driver_img4 %}{{page.driver_img4 }}{% endcapture %}
    {% capture driver_cap4 %}{{page.driver_cap4 }}{% endcapture %}
    {% capture driver_url4 %} .\images\{{ page.driver_img4 }} {% endcapture %}

    {% capture driver_img5 %}{{page.driver_img5 }}{% endcapture %}
    {% capture driver_cap5 %}{{page.driver_cap5 }}{% endcapture %}
    {% capture driver_url5 %} .\images\{{ page.driver_img5 }} {% endcapture %}

    {% capture driver_img6 %}{{page.driver_img6 }}{% endcapture %}
    {% capture driver_cap6 %}{{page.driver_cap6 }}{% endcapture %}
    {% capture driver_url6 %} .\images\{{ page.driver_img6 }} {% endcapture %}

    {% capture driver_img7 %}{{page.driver_img7 }}{% endcapture %}
    {% capture driver_cap7 %}{{page.driver_cap7 }}{% endcapture %}
    {% capture driver_url7 %} .\images\{{ page.driver_img7 }} {% endcapture %}

    {% capture driver_img8 %}{{page.driver_img8 }}{% endcapture %}
    {% capture driver_cap8 %}{{page.driver_cap8 }}{% endcapture %}
    {% capture driver_url8 %} .\images\{{ page.driver_img8 }} {% endcapture %}

    {% capture driver_img9 %}{{page.driver_img9 }}{% endcapture %}
    {% capture driver_cap9 %}{{page.driver_cap9 }}{% endcapture %}
    {% capture driver_url9 %} .\images\{{ page.driver_img9 }} {% endcapture %}

    {% capture driver_img10 %}{{page.driver_img10 }}{% endcapture %}
    {% capture driver_cap10 %}{{page.driver_cap10 }}{% endcapture %}
    {% capture driver_url20 %} .\images\{{ page.driver_img10 }} {% endcapture %}

## Overview 

  {% 
  include image.html 
  file=driver_img1
  url=driver_url1
  alt=driver_cap1
  caption=driver_cap1
  %}

### Fly HV-TCM5160 Pro Driver

The HV-TMC5160 Pro V1.2 driver is made according to customer requirements. We have designed a high voltage driver to support 48V voltage, but high voltage represents a greater risk. We do not recommend customers with no technical experience to use 48V voltage. 24V has satisfied most customers.

### New features in Version 1.2
 Added a separate VSA power supply port, VSA power supply uses 12V power supply by default, add a 470uf capacitor.The matching small module adds a 12V power supply chip to supply 12V to the vsa of the 5160 chip.Of course, a larger voltage means that a larger motor can be used, which is of great help to the moving speed of the 3D printer. Please select the operating voltage with safety as the first criterion.


### Product parameters

 - Product name: FLY HV-TMC5160 PRO V1.2
 - Features: External high voltage TMC5160 drive
 - Input voltage: 24-48V
 - Maximum current: 6
 - Capacitor: 2*470uf
 - Supported Firmware:Marlin/RRF/Klipper
 - Product material: PCB copper 2oz thick, gold plated
 - Step/direction interface with microstep interpolation microPlyer
 - The highest resolution is 256 microsteps
 - StealthChop2 silent work and smooth motion
 - Resonance suppression for mid-range resonance
 - SpreadCycle high dynamic motor control chopper
 - DcStep load related speed control
 - StallGuard2 high-precision sensorless motor load detection
 - CoolStep current control, which can achieve up to 75% energy savings

### Dimensions

  {% 
  include image.html 
  file=driver_img2
  url=driver_url2
  alt=driver_cap2
  caption=driver_cap2
  %}

### Stepper Wiring
  {% 
  include image.html 
  file=driver_img3
  url=driver_url3
  alt=driver_cap3
  caption=driver_cap3
  %}

### Cooling Fan
  {% 
  include image.html 
  file=driver_img4
  url=driver_url4
  alt=driver_cap4
  caption=driver_cap4
  %}

### SPI Jumpers
  {% 
  include image.html 
  file=driver_img5
  url=driver_url5
  alt=driver_cap5
  caption=driver_cap5
  %}

### Diag Pin
  {% 
  include image.html 
  file=driver_img6
  url=driver_url6
  alt=driver_cap6
  caption=driver_cap6
  %}

### Firmware
  {% 
  include image.html 
  file=driver_img7
  url=driver_url7
  alt=driver_cap7
  caption=driver_cap7
  %}

### Front and Back View
  {% 
  include image.html 
  file=driver_img8
  url=driver_url8
  alt=driver_cap8
  caption=driver_cap8
  %}

### Stepper Adapter
  {% 
  include image.html 
  file=driver_img9
  url=driver_url9
  alt=driver_cap9
  caption=driver_cap9
  %}

### BOM
  {% 
  include image.html 
  file=driver_img10
  url=driver_url10
  alt=driver_cap10
  caption=driver_cap10
  %}