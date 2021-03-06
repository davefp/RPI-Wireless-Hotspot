RPI-Wireless-Hotspot
--------------------

Configures your Raspberry Pi to use an attatched WiFi dongle as a hotspot,
broadcasting your ethernet connection to other devices. Could be useful in hotel rooms, college dorms
or if you just don't feel like buying a router!


Features:
=========

* The created hotspot runs automatically on boot, no extra configuration necessary

* Your new network is WPA encryped, default SSID is "RaspberryPiFi", WPA key
  is "123456789A".

* Once set up, the local network facilites of the Pi will still operate as 
  normal

Requirements:
=============

1. A Raspberry Pi model B running raspbian

2. A Raspbian compatible Wifi dongle. This script assumes that your adapter uses the nl80211 drivers in hostapd (the majority of new products should support this). Others can be made to work, but require a custom compilation of hostapd (guides are out there).

3. An active ethernet connection


Installation:
=============

* In the terminal, run:
    git clone https://github.com/harryallerston/RPI-Wireless-Hotspot.git

* Navigate to folder, and execute "./install"

* This should automatically set everything up and leave you ready to go


Notes and configuration
=======================

* to change default SSID, WPA key or WiFi channel, edit /etc/hostapd/hostapd.conf accordingly

* This setup has been tested on a fresh install of raspbian.

* It is advised that this be set up on a fresh install

* if set up on an existing install then any current config files will be backed up with the extension ".old" in the       relevant folders prior to installation (this allows returning to original network settings if required)

