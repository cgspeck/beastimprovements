# Repetier 1.x.y firmware for the beast

The Beast comes supplied with Repetier 0.92 firmware.

These are the configuration files needed to create a 1.x.y firmware at the [configuration tool].

Flavours:

 * `config-4x.json`: vanilla 4 extruder configuration, as close to the original 0.92.x firmware as possible
 * `config-3x.json`: 3 extruder configuration, created this when fourth extruder failed
 * `config-4x-bltouch.json`: as per `config-4x.json` but with software bed levelling support using a BL Touch probe and removal of the mechanical Z end-stop per this post: [BLTouch Auto Leveling / Distortion Correction.](http://3dbeastbuilders.boards.net/thread/231/bltouch-auto-leveling-distortion-correction)
 * `config-1x-bltouch-min.json`: as per `config-4x-bltouch-min.json` but only instructing extruder number one of four, in a 217x214 area (i.e. other three extruders remain physically attached to gantry)

[Installing and tuning the BL Touch](https://www.youtube.com/watch?time_continue=374&v=U2zxzn0K_5U)

## Compiling

### Prerequisites

Download and install Arduino IDE using a package manager or from the [site](https://www.arduino.cc/en/Main/Software). This will work with recent version such as 1.8.9.

### Process

Upload the selected `config-xxx.json` file to the [configuration tool].

Click on the "Download" tab.

Click "Download complete firmware incl. these settings".

Extract the archive somewhere.

Connect the Beast to your machine and turn it on.

Open `Repetier-Firmware\Repetier\Repetier.ino` in Arduino IDE. Ignore any errors concerning file encoding.

Check that:

* the board is set to Mega 256
* the port is correct

Click on the "Right arrow" button to compile and upload the new firmware.



[configuration tool]: https://www.repetier.com/firmware/v100/index.php

