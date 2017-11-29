
Arduino DS3231 High Precision Real Time library for Mongoose OS
=========

Tested and works on esp8266/esp32

## Description
DS3231 is a low-cost, extremely accurate I2C real-time clock (RTC), with an integrated temperature-compensated crystal oscillator (TCXO) and crystal. The device incorporates a battery input, disconnect the main power supply and maintains accurate timekeeping. Integrated oscillator improve long-term accuracy of the device and reduces the number of components of the production line. The DS3231 is available in commercial and industrial temperature ranges, using a 16-pin 300mil SO package.
RTC maintains seconds, minutes, hours, day, date, month, and year information. Less than 31 days of the month, the end date will be automatically adjusted, including corrections for leap year. The clock operates in either the 24 hours or band / AM / PM indication of the 12-hour format. Provides two configurable alarm clock and a calendar can be set to a square wave output. Address and data are transferred serially through an I2C bidirectional bus. 

![alt text](http://www.continentalee.com.sg/content/images/thumbs/0000720_clock-module-ds3231_70.jpeg)

### Features
* Battery
* Operating voltage: 3.3 - 5.5V
* Clock chip: High-precision clock chip DS3231
* Clock Accuracy: 0-40 °C range, the accuracy 2ppm, the error was about 1 minute
* Calendar alarm clock with two
* Programmable square-wave output
* Real time clock generator seconds, minutes, hours, day, date, month and year timing and provide valid until the year 2100 leap year compensation
* Chip temperature sensor comes with an accuracy of ± 3 °C

### Slave address 
* Address pin connected to GND = 0x48 Offset = binary 1001000
* Address pin connected to VDD = 0x49 Offset = binary 1001001
* Address pin connected to SDA = 0x4A Offset = binary 1001010
* Address pin connected to SCL = 0x4B Offset = binary 1001011

