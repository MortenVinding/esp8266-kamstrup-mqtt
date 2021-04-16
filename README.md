# esp8266-kamstrup-mqtt

Fork of https://github.com/Claustn/esp8266-kamstrup-mqtt since I need the ESP to run only on power supplied from the meter it self.

To keep it simple and not have any circurity not needed and using power, I changed it to work on a ESP-01.

Serial swap is removed so we use the serial on GPIO2 and GPIO3 available on the ESP-01.
That means debug is still going to GPIO2 (TX), but we only receive from the meter (on GPIO3 RX), but it means debug is reduced to 2400 baud.

Also added a meaning full hostname and a status topic to tell when data is received.
