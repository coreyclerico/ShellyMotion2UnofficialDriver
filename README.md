# ShellyMotion2UnofficialDriver
Shelly Motion 2 Hubitat Unofficial Driver

Here is a unofficial driver for Shelly Motion 2 for the Hubitat.  It uses a IP address much like the switching products, no need for mqtt.   
Install your Motion 2 device on WiFi, upgrade the firmware and set the sensor requirement on the Shelly Web GUI.

https://www.shelly.cloud/en-us/products/product-overview/shelly-motion-2-1

Add the Web Actions to each of the catagories and user the url for callback

http://172.16.1.111:39501   (your Hubitat IP address)

Set the preferences in the device driver to query every 1 or 5 minutes.   If the device detects motion or tampering it will do a callback to the Hubitat to requery.

This is built on the same initial code of Scott Grayban's Shelly framework, please thank him for the work.   I'm sure eventually there will be a official version.

As far as DHCP settings, I use pre-set DHCP static IPs for all Shelly's on a Juniper router just to give an example.

set system services dhcp static-binding 8c:f6:81:14:93:25 fixed-address 172.16.2.130
set system services dhcp static-binding 8c:f6:81:14:93:25 host-name shellymotion-FamilyRoom

If your going across a router hop to get the callback to work a hex IP must be used in the device network id (edit). For example: AC100282

Shelly Motion 2 are fabulous tech.  Love them already.  Enjoy.
