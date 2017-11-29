
Arduino Adafruit PWM servo library
=========
## Description

16-Channel 12-bit PWM/Servo Driver – I2C interface – PCA9685 Module lets you add more IOs to your microcontroller boards (such as Arduino Boards, Raspberry Pi Boards and more). The Module has chainable I2C interface meaning for even more IOs more boards can be daisy chained. Its and excellent product for Robots that require lots of Servo motors to control using single microcontroller.
---> https://www.adafruit.com/product/815

![alt text](http://www.robotpark.com/image/cache/data/PRO/91098/91098-Adafruit-16-Channel-12-bit-PWM-Servo-Driver_Pic02-700x700.jpg)

### PCA9685 Highlights from datasheet

* 16 individually controlled channels
* 12bit (4096 steps) registers both for on and off time
* 1MHz fast I2C bus interface with 30mA high drive capability on SDA output for driving high capacitive buses
* 40MHz to 1000MHz PWM frequency for all LEDs with internal 25MHz oscillator
* Operating power supply voltage range of 2.3 V to 5.5 V
* Six hardware address pins allow up to 62 devices on the same bus

### Features

*   **Mutt** e-mail client also by [me] (*just* the Mutt colorscheme is
    [available here][Mutt Repository])

* it’s an i2c-controlled PWM driver with a built in clock. That means that, unlike the TLC5940 family, you do not need to continuously send it signal tying up your microcontroller, its completely free running.
It is 5V compliant, which means you can control it from a 3.3V microcontroller and still safely drive up to 6V outputs (this is good for when you want to control white or blue LEDs with 3.4+ forward voltages)
6 address select pins so you can wire up to 62 of these on a single i2c bus, a total of 992 outputs – that’s a lot of servos or LEDs
Adjustable frequency PWM up to about 1.6 KHz
12-bit resolution for each output – for servos, that means about 4us resolution at 60Hz update rate
Configurable push-pull or open-drain output
Output enable pin to quickly disable all the outputs
Terminal block for power input (or you can use the 0.1″ breakouts on the side)
Reverse polarity protection on the terminal block input
Power-good LED
3 pin connectors in groups of 4 so you can plug in 16 servos at once
“Chain-able” design
A big capacitor on the V+ line
220 ohm series resistors on all the output lines to protect them, and to make driving LEDs trivial
Solder jumpers for the 6 address select pins
Technical Specifications
IO expander chip: PCA9685PW
Operating Voltage: 2.3V – 5.5V
Dimensions (no headers or terminal block) 2.5″ x 1″ x 0.1″ (62.5mm x 25.4mm x 3mm)
Weight (with 3×4 headers & terminal block): 10.0 grams
I2C 7-bit address Range: between 0x40-0x7F, selectable with jumpers
