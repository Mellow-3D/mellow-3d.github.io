---
title: Klipper Host configuration
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Klipper Host Configuration"
sidebar: mydoc_sidebar
permalink: fly-utoc_firmware.html
folder: mydoc
comments: false
toc: true
datatable: true

utocfw_img1:  "fly-utoc/fly_utoc-dfu_jumpers.png"
utocfw_cap1:  "Fly UTOC DFU pins" 

utocfw_img2:  "fly-utoc/UTOC_DFU_Jumper.jpg"
utocfw_cap2:  "Fly UTOC DFU jumper installed" 

---

    {% capture utocfw_img1 %}{{page.utocfw_img1 }}{% endcapture %}
    {% capture utocfw_cap1 %}{{page.utocfw_cap1 }}{% endcapture %}
    {% capture utocfw_url1 %} .\images\{{ page.utocfw_img1 }} {% endcapture %}

    {% capture utocfw_img2 %}{{page.utocfw_img2 }}{% endcapture %}
    {% capture utocfw_cap2 %}{{page.utocfw_cap2 }}{% endcapture %}
    {% capture utocfw_url2 %} .\images\{{ page.utocfw_img2 }} {% endcapture %}    

## Flashing UTOC Firmware
{% include note.html content="The UTOC firmware is intalled at the manufacturer.  This procedure is only needed to restore the OEM firmware." %}


- Upload the utoc_firmware.bin file to the user folder on your klipper host.
  - Link to [utoc_firmware.bin](./files/utoc_firmware.bin)
- Install the DFU mode Jumper
  {% 
  include image.html 
  file=utocfw_img1
  url=utocfw_url1
  alt=utocfw_cap1
  caption=utocfw_cap1
  %}

    {% 
  include image.html 
  file=utocfw_img2
  url=utocfw_url2
  alt=utocfw_cap2
  caption=utocfw_cap2
  %}

- Connect the UTOC to the klipper host by the USB C port

- SSH to the klipper host

- From the klipper host command line run
```
lsusb
```

- It should return
```
Bus 001 Device 004: ID 0483:df11 STMicroelectronics STM Device in DFU Mode
```

- Run the following command to flash the UTOC.
```
sudo dfu-util --dfuse-address -d 0483:df11 -c 1 -i 0 -a 0 -s 0x08000000 -D ~/utoc_firmware.bin
```


{% include custom/can/sht_links.html %}