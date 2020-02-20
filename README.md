# arduino-usb-tester

arduino-usb-tester is (the beginning of) a collection of Arduino firmware implementing different USB gadgets.
Its main purpose is testing USB stacks or pieces of stacks (for example, PyUSB).
It can also be used to capture protocol data with access to real devices.

_Note: I'm using an Arduino Uno rev. 3 I had laying around; LUFA parameters and the DFU target will need to be adjusted if a different board is used._


## A primer of Arduino Uno firmware flashing

### LUFA

### Adjusting LUFA parameters and building the firmware

### Physically entering DFU mode

### Flashing stock or custom firmware

To flash a new firmware to an Uno in DFU mode, stock or custom, use [dfu-programmer]:

```
# physically set the Uno to enter DFU mode

sudo dfu-programmer atmega16u2 erase
sudo dfu-programmer atmega16u2 flash <firmware file>

# physically reconnect the Uno
```


## h115i-emulatinum

Dumb emulation of a H115i Platinum for development of Linux/macOS drivers.

Related: [liquidctl#76](https://github.com/jonasmalacofilho/liquidctl/issues/76) ("Support for Corsair H115i Platinum").


## arduino-keyboard

Archived Arduino Keyboard firmware by Darran, and corresponding blog posts.

Fetched from the Wayback Machine:

 - [Arduino UNO Keyboard HID part 2](https://web.archive.org/web/20130215045104/http://hunt.net.nz/users/darran/weblog/faf5e/Arduino_UNO_Keyboard_HID_part_2.html)
 - [Arduino UNO Keyboard HID version 0.3](https://web.archive.org/web/20120127004113/http://hunt.net.nz/users/darran/weblog/b3029/Arduino_UNO_Keyboard_HID_version_03.html)


## uno-rev3-backup

Backup dump of the factory firmware from my Uno rev. 3.  Not useful as is, but could just a conversion to the correct hex format.

Regardless, it is probably better to just use [Arduino-usbserial-atmega16u2-Uno-Rev3.hex](https://github.com/arduino/ArduinoCore-avr/blob/master/firmwares/atmegaxxu2/arduino-usbserial/Arduino-usbserial-atmega16u2-Uno-Rev3.hex).
