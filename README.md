# ShellyMotion2UnofficialDriver
Shelly Motion 2 Hubitat Unofficial Driver

Here is a unofficial driver for Shelly Motion 2 for the Hubitat.  It uses a IP address much like the switching products, no need for mqtt.   
Install your Motion 2 device on WiFi, upgrade the firmware and set the sensor requirement on the Shelly Web GUI.

Add the Web Actions to each of the catagories and user the url for callback

http://172.16.1.111:39501   (your hubitat IP address)

Set the preferences in the device driver to query every 1 or 5 minutes.   If the device detects motion or tampering it will do a callback to the Hubitat to requery.

This is built on the same initial code of Scott Grayban's Shelly framework, please thank him for the work.   I'm sure eventually there will be a official version.

Enjoy.
