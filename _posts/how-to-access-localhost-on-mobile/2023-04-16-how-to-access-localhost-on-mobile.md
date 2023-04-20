---
layout: post
title: How to access localhost on mobile
date: 2023-04-16 01:00 +0700
modified: 2023-04-16 16:49:47 +07:00
description: Assume that you donot have any USB cables for some reason and you all i have a wifi or mobile hotspot, now you want to access your locally hosted app on an mobile browser.
tag:
  - localhost
  - WiFi
  - hotspot
  - mobile
  - laptop
---
Assume that you donot have any USB cables for some reason and you all i have a wifi or mobile hotspot, now you want to access your locally hosted app on an mobile browser.

1.  Connect all devices to same WiFi or Create a hotspot in your mobile and connect your laptop to it.
2.  Get ipaddress of the device using ifconfig,ipconfig in Laptop or About phone > Status in mobile device.
3.  Open your mobile browser and enter locally hosted server's ip and port for example `http://192.168.58.33:4000`. If all goes well you should be able to access the app in mobile device.
4.  If you still get any issues you could try setting "0.0.0.0" to devServer or server object in package json example `devServer:{"host":"0.0.0.0"} server:{"host":"0.0.0.0"}` or turn of the firewall

