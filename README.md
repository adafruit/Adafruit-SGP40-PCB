## Adafruit SGP40 Air Quality Sensor PCB

<a href="http://www.adafruit.com/products/4829"><img src="assets/4829.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit SGP40 Air Quality Sensor.

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/4829

### Description

*sniff* *sniff* ... do you smell that? No need to stick your nose into a carton of milk anymore, you can build a digital nose with the SGP40 Multi-Pixel Gas Sensor, a fully integrated MOX gas sensor. This is a very fine air quality sensor from the sensor experts at Sensirion, with I2C interfacing so you don't have to manage the heater and analog reading of a MOX sensor. It combines multiple metal-oxide sensing and heating elements on one chip to provide more detailed air quality signals.

The SGP40 has a 'standard' hot-plate MOX sensor, as well as a small microcontroller that controls power to the plate, reads the analog voltage and provides an I2C interface to read from. Unlike the CCS811, this sensor does not require I2C clock stretching. We currently have an Arduino library with examples of reading the raw value and also running the Sensirion algorithm to calculate VOC index but do not have Python support (the Sensirion library is in C and requires a port)

This is a gas sensor that can detect a wide range of Volatile Organic Compounds (VOCs) and H2 and is intended for indoor air quality monitoring. The SGP40 is the next generation after the SGP30, but does not give TVOC/eCO2 values out like the SGP30. Instead, raw signal from the sensor is processed using their software algorithm to give an overall 'air quality' value form 0 to 500.

Please note, this sensor, like all VOC/gas sensors, has variability, and to get precise measurements you will want to calibrate it against known sources! That said, for general environmental sensors, it will give you a good idea of trends and comparison.

Another nice element to this sensor is the ability to set humidity compensation for better accuracy. An external humidity sensor is required and then the RH% is written over I2C to the sensor, so it can better calibrate the MOX sensor reading and reduce humidity/temperature-based variations..

Nice sensor right? So we made it easy for you to get right into your next project. The surface-mount sensor is soldered onto a custom made PCB in the STEMMA QT form factor, making them easy to interface with. The STEMMA QT connectors on either side are compatible with the SparkFun Qwiic I2C connectors. This allows you to make solderless connections between your development board and the SGP40 or to chain it with a wide range of other sensors and accessories using a compatible cable. QT Cable is not included, but we have a variety in the shop

We’ve of course broken out all the pins to standard headers and added a 3.3V voltage regulator and level shifting so allow you to use it with either 3.3V or 5V systems such as the Arduino Uno, or Feather M4.

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution.
See license.txt for additional details.
