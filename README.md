Arduino_Make
=======================

Use make on macos Darwin or linux instead of arduino IDE.

```
Requires:
  Arduino 1.6.9 or newer to be installed, and to manage installed boards.
  GNU Make

Installation:
  Install in ~/Arduino/Arduino_Make
  It is best to install Arduino under /opt and have a symlink pointing to it.
          /opt/Arduino -> adduino-1.6.9
          /opt/bin/Arduino -> ../Arduino/Arduino
          You then have that added to your PATH.
          This will allow automatic detection, and allow you to change the Arduino IDE
          by just modifying the /opt/Arduino symlink.

NOTE:
  Even though arduino builder does a lot for you...
    * If your sketch (.ino) does not compile because YOU did not include Arduino.h or 
    * then YOU need to fix YOUR code.
    * YOU need to also properly do all function prototypes as well.
    * Avoid problems! Do your code the proper way from the start.

Features:
  Supports all boards that are installed.
  Separated build output for each target. Builds go into ~Arduino/build/SKETCHNAME.ino/...
          example: ~/Arduino/build/TEST.ino/_arduino/_AVR_MEGA2560/_AVR/_atmega2560
```
