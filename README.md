# Twomes Presence Detector firmware (template)

This is a template for a repository with a PlatformIO project that uses the [twomes-generic-esp-firmware](https://github.com/energietransitie/twomes-generic-esp-firmware) library. To create your own Twomes measurement device, select `Use this template`, consult the [documentation how to use this template and add code for measurement of specific properties](https://www.energietransitiewindesheim.nl/twomes-generic-esp-firmware).

## Table of contents
* [General info](#general-info)
* [Deploying](#deploying)
* [Developing](#developing) 
* [Supported devices](#supported-devices)
* [Features](#features)
* [Status](#status)
* [License](#license)
* [Credits](#credits)

## General info
The Twomes Presence-Detector example sends [generic data sent by any Twomes measurement device](https://github.com/energietransitie/twomes-generic-esp-firmware#readme) to a Twomes server. In addition, it also sends presence detection data to the Twomes server:

| Sensor | Property           | Unit | [Printf format](https://en.wikipedia.org/wiki/Printf_format_string) | Default measurement interval \[h:mm:ss\] | Description                            |
|--------|--------------------|------|--------|-------------------|----------------------------------------|
| Bluetooth  | `countPresence`         | [-]   | %u   | 0:10:00           | number of smartphones responding to Bluetooth name request                        |

## Deploying
To deploy this software, see the [deploying section in the twomes-generic-esp-firmware library documentation](https://www.energietransitiewindesheim.nl/twomes-generic-esp-firmware/deploying/prerequisites/).

## Developing
To develop software for, or based on this software, see the [developing section in the twomes-generic-esp-firmware library documentation](https://www.energietransitiewindesheim.nl/twomes-generic-esp-firmware/developing-library-getstarted/prerequisites/)

## Supported devices
This example was tested on:
- [M5Stack CoreInk](https://github.com/m5stack/M5-CoreInk)

This example still needs to be tested n:
- [LilyGO TTGO T7 Mini32 V1.3 ESP32](https://github.com/LilyGO/ESP32-MINI-32-V1.3)

## Features
The example features generic firmware tasks, including Bluetooth-based presence detection. For an example that does not include presence detection, we refer to the Twomes GEneric-Test example](../generic-test/README.md).

Ready:
* Generic firmware tasks
* Use [Twomes generic ESP32 firmware library](https://github.com/energietransitie/twomes-generic-esp-firmware)

To-do:
* Automate build of device installation manual pages.
* Automate build of device info page.

## Status
Project is: _in progress_

## License
This software is available under the [Apache 2.0 license](./LICENSE), Copyright 2022 [Research group Energy Transition, Windesheim University of Applied Sciences](https://windesheim.nl/energietransitie) 

## Credits
This software was created by:
* Nick van Ravenzwaaij · [@n-vr](https://github.com/n-vr)

Product owners:
* Henri ter Hofte · [@henriterhofte](https://github.com/henriterhofte) · Twitter [@HeNRGi](https://twitter.com/HeNRGi)

We use and gratefully acknowlegde the efforts of the makers of the following source code and libraries:
* [ESP-IDF](https://github.com/espressif/esp-idf), by Espressif Systems, licensed under [Apache License 2.0](https://github.com/espressif/esp-idf/blob/9d34a1cd42f6f63b3c699c3fe8ec7216dd56f36a/LICENSE)
* [Twomes Generic ESP Firmware](https://github.com/energietransitie/twomes-generic-esp-firmware), by Research group Energy Transition, Windesheim University of Applied Sciences, licensed under [Apache License 2.0](https://github.com/energietransitie/twomes-generic-esp-firmware/blob/main/LICENSE.md)
