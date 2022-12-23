# WLED Stuff and Resources


**WLED First Install WiFi AP Password**
> wled1234

## How to setup

#### Flashing method 2: esptool
  + adapted from [Install WLED Binary]()

  * First of all, install [esptool](https://github.com/espressif/esptool)

  * Download the latest [release binary file](https://github.com/Aircoookie/WLED/releases)!
  
  * Make sure only one ESP device/microcontroller is connected to your computer!
    Otherwise you could accidentally overwrite the wrong one.
    If you know the serial port, you can also add the `-port COM3` attribute after `write_flash`

  * Execute this command:
    * ESP8266
        `esptool.py write_flash --verify 0x0 ./WLED_XXX.bin`
    * ESP32
      * Firstly, flash the version 4 bootloader [file, which you can find here.](https://github.com/Aircoookie/WLED/releases/download/v0.13.1/esp32_bootloader_v4.bin)
        This step only has to be done once, to update afterwards the bootloader does not have to be re-installed.
        `esptool.py write_flash 0x0 ./esp32_bootloader_v4.bin`
      * Now you can flash the actual firmware binary. Keep in mind the bootloader needs to have a flash offset of 0, but the firmware 0x10000.
        `esptool.py write_flash 0x10000 ./WLED_XXX.bin`

  When esptool.py says Connecting..., some ESP32 boards require you to hold the
  boot button (to the right of the USB port) for a few seconds

  If you experience issues, run this command before trying write_flash again (Note: this will erase all settings stored on the ESP!)

  esptool.py erase_flash
  If you have a MagicHome controller, here is a good video tutorial on how to flash it.



## Links

* [WLED Wemos Shield (tindie)](https://github.com/srg74/WLED-wemos-shield)
* [Adafruit - Huzzah ESP8266](https://learn.adafruit.com/adafruit-huzzah-esp8266-breakout/pinouts)


