# icinga2-temperaturesensor

This is an easy and inexpensive way to get a server room temperature monitoring solution without having to buy an expensive, proprietary device or being "vendor locked-in". 

The way this works is that an ESP8266 microcontroller with an attached DS18B20 thermometer continually measures the temperature and displays it on a webpage, that is reachable via the WLAN network it connects to. The Icinga plugin then polls the temperature value and returns an exit code that will trigger an alert (or not).

The `icinga-settings.txt` contain suggestions for entries to the commands.conf, hosts file and services file that you have to add to your server configuration.

More info on the whole thing on my blog: https://blog.morph.sh/posts/2019-08-06-serverraum-thermometer-de
