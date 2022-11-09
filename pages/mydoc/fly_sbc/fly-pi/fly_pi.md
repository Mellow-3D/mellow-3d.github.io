---
title: Fly Pi General Information
tags: []
keywords: 
last_updated: 20/10/2022
summary: "General information regarding the Fly Pi"
sidebar: mydoc_sidebar
permalink: fly_pi.html
folder: mydoc
comments: false
toc: false
datatable: true
---
## Overview 
fly pi

### Getting Started

 - Install Bonjour support  so the Fly Pi will respond to http://flygemini.local/
  - Run the following commands to update and install Bonjour support. 
  
```
sudo apt-get update
```

```
sudo apt-get updgrade
```

```
sudo apt-get install avahi-daemon
```

- When complete your Fly Pi will respond to local dns queries for it's hostname.
