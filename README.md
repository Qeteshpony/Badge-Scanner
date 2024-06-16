# NFC-Badge Scanner

[![CI](https://github.com/Qeteshpony/Badge-Scanner/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Qeteshpony/Badge-Scanner/actions/workflows/ci.yml)

![3D Render](https://qeteshpony.github.io/Badge-Scanner/3D/Badge-Scanner-3D_top.png)

[Hardware Documentation](https://qeteshpony.github.io/Badge-Scanner)

Raspberry Pi Pico W powered device to scan NFC-Badges and show a status on display

It is meant to be used with the widely available RFID-RC522 reader and the [DFROBOT LCD1602 RGB Backlight Module](https://raw.githubusercontent.com/DFRobot/DFRobot_RGBLCD/master/DFR0464%20Datasheet.pdf) but any other I2C Display should work as well. 

The device also features an [I2C RTC](https://www.analog.com/media/en/technical-documentation/data-sheets/ds3231m.pdf) with backup battery and an SD-Card reader for data storage. 

There is also a connector for a 5V buzzer that can be used for audible signals. 