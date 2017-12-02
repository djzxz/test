
Arduino DS3231 High Precision Real Time Clock (RTC) library for Mongoose OS
=========

Tested and works on esp8266/esp32

## Description
DS3231 is a low-cost, extremely accurate I2C real-time clock (RTC), with an integrated temperature-compensated crystal oscillator (TCXO) and crystal. The device incorporates a battery input, disconnect the main power supply and maintains accurate timekeeping. Integrated oscillator improve long-term accuracy of the device and reduces the number of components of the production line.
RTC maintains seconds, minutes, hours, day, date, month, and year information. Less than 31 days of the month, the end date will be automatically adjusted, including corrections for leap year. The clock operates in either the 24 hours or band / AM / PM indication of the 12-hour format. Provides two configurable alarm clock and a calendar can be set to a square wave output. Address and data are transferred serially through an I2C bidirectional bus.See [product page link](https://www.adafruit.com/product/3013) for more information about the hardware.

![alt text](https://cdn-shop.adafruit.com/970x728/3013-02.jpg)

### Features
* Battery
* Operating voltage: 3.3 - 5.5V
* Clock chip: High-precision clock chip DS3231
* Clock Accuracy: 0-40 °C range, the accuracy 2ppm, the error was about 1 minute
* Calendar alarm clock with two
* Programmable square-wave output
* Real time clock generator seconds, minutes, hours, day, date, month and year timing and provide valid until the year 2100 leap year compensation

### Usage

mos.yml, add:
```
libs:
  - origin: https://github.com/mongoose-os-libs/arduino-ds3231
  ```
init.js, add:
```
load('api_ds3231.js');
```
main.c, add:
```
#include "mgos_arduino_DS3231.h" 
```


Arduino Adafruit ADS1015 12-BiT/ADS1115 16-Bit ADC - 4 Channel with Programmable Gain Amplifier library for Mongoose OS
=========

Tested and works on esp8266/esp32

## Description
Analog-to-digital converter or higher-precision ADC. 

|           | precision | samples\sec |
| :---      |     :---: | :---        |
| ADS1015   | 12-bit    | 3300        |
| ADS1115   | 16-bit    | 860         |

The chip can be configured as 4 single-ended input channels, or two differential channels. As a nice bonus, it even includes a programmable gain amplifier, up to x16, to help boost up smaller single/differential signals to the full range. See [ADS1015](https://www.adafruit.com/product/1083) [ADS1115](https://www.adafruit.com/product/1085) for more information about the hardware.   

![alt text](https://cdn-shop.adafruit.com/970x728/1083-00.jpg)
![alt text](https://cdn-shop.adafruit.com/970x728/1085-02.jpg)

### Features
* Wide supply range: 2.0V to 5.5V
* Low current consumption: Continuous Mode: Only 150uA Single-Shot Mode: Auto Shut-Down
* Programmable data rate: 8SPS to 860SPS
* Internal Low-drift voltage reference
* Internal oscillator
* Internal PGA
* I2C interface: Pin-Selectable Addresses
* Four Single-ended or two differential inputs
* Programmable comparator
* This board/chip uses I2C 7-bit addresses between 0x48-0x4B, selectable with jumpers

### Usage

mos.yml, add:
```
libs:
  - origin: https://github.com/mongoose-os-libs/arduino-adafruit-ads1x15
  ```
init.js, add:
```
load('api_ads1015.js');
```
main.c, add:
```
#include "mgos_arduino_Adafruit_ADS1015.h"
```

### Slave address
* Address pin connected to GND = 0x48 Offset = binary 1001000
* Address pin connected to VDD = 0x49 Offset = binary 1001001
* Address pin connected to SDA = 0x4A Offset = binary 1001010
* Address pin connected to SCL = 0x4B Offset = binary 1001011



Arduino Adafruit - 16-Channel 12-bit PWM/Servo Driver - I2C interface - PCA9685 library for Mongoose OS
=========

Tested and works on esp8266/esp32
## Description

16-Channel 12-bit PWM/Servo Driver – I2C interface – PCA9685 Module lets you add more IOs to your microcontroller boards. The Module has chainable I2C interface meaning for even more IOs more boards can be daisy chained. Its and excellent product for Robots that require lots of Servo motors to control using single microcontroller.See [product page link](https://www.adafruit.com/product/815) for more information about the hardware.

![alt text](https://cdn-shop.adafruit.com/970x728/815-06.jpg)
### Features

* It is 5V compliant, which means you can control it from a 3.3V microcontroller and still safely drive up to 6V outputs (this is good for when you want to control white or blue LEDs with 3.4+ forward voltages)
* 6 address select pins so you can wire up to 62 of these on a single i2c bus, a total of 992 outputs – that’s a lot of servos or LEDs
* Adjustable frequency PWM up to about 1.6 KHz
* 12-bit resolution for each output – for servos, that means about 4us resolution at 60Hz update rate
* Configurable push-pull or open-drain output
* Output enable pin to quickly disable all the outputs
* Reverse polarity protection on the terminal block input
* Power-good LED
* 3 pin connectors in groups of 4 so you can plug in 16 servos at once
* A big capacitor on the V+ line
* 220 ohm series resistors on all the output lines to protect them, and to make driving LEDs trivial
* IO expander chip: PCA9685PW
* Operating Voltage: 2.3V – 5.5V
* Solder jumpers for the 6 address select pins
* I2C 7-bit address Range: between 0x40-0x7F, selectable with jumpers

### Usage

mos.yml, add:
```
libs:
  - origin: https://github.com/mongoose-os-libs/arduino-adafruit-pwm-servo
  ```
init.js, add:
```
load('api_pwm_servo.js');
```
main.c, add:
```
#include "mgos_arduino_PWMServoDriver.h"
```

### Slave address
* Board 0: Address = 0x40 Offset = binary 00000 (no jumpers required) 
* Board 1: Address = 0x41 Offset = binary 00001 (bridge A0 ) 
* Board 2: Address = 0x42 Offset = binary 00010 (bridge A1) 
* Board 3: Address = 0x43 Offset = binary 00011 (bridge A0 & A1) 
* ...
