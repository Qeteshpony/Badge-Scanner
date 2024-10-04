# NFC-Badge Scanner

[![CI](https://github.com/Qeteshpony/Badge-Scanner/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Qeteshpony/Badge-Scanner/actions/workflows/ci.yml)

![3D Render](https://qeteshpony.github.io/Badge-Scanner/3D/Badge-Scanner-3D_top.png)
![3D Render](https://qeteshpony.github.io/Badge-Scanner/3D/Badge-Scanner-3D_bottom.png)

[Hardware Documentation](https://qeteshpony.github.io/Badge-Scanner)

Raspberry Pi Pico W powered device to scan NFC-Badges and show a status on display

It is meant to be used with the widely available RFID-RC522 reader and the [DFROBOT LCD1602 RGB Backlight Module](https://raw.githubusercontent.com/DFRobot/DFRobot_RGBLCD/master/DFR0464%20Datasheet.pdf) but any other I2C Display should work as well. 

The device features an [I2C RTC](https://www.analog.com/media/en/technical-documentation/data-sheets/ds3231m.pdf) with backup battery connector and an SD-Card reader connected via SPI for data storage. 

There is also a buzzer that can be used for audible signals. 

Power can be provided through the USB port of the Pico or through a LiPo battery connected to the board. The LiPo battery can also be charged via the USB port and the device will switch seamlessly between battery and usb power.

The button can be used to send a shutdown signal to the microcontroller which then can power the whole device off by pulling a GPIO low. Pressing the button while the device is off or pluggin in USB will power it up again. 
