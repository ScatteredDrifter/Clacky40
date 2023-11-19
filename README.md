# Clacky40: 

Yet another replacement Board for the Daisy40. 
Running with a RP2040, adapted from elmos:![Dizzy40](https://github.com/kb-elmo/Dizzy40)

--- 
## Status:
- PCB tested, _Vial support available_
- compatible with Case!
- minor issue with footprint fixed, pcb is fully functional now
 

## Features:
- RP2040 
- (TODO) ZMK support
- VIAL / QMK support
- supports two encoders
- additional layout options
- additional pinouts for additional LEDS ( 5V+, GND, GPIO)

--- 

## Layouting:
![image of available layouts](/material/images/kle_layout.png)

## Firmware:
pre-compiled file for vial can be found in the **"/firmware"** section.
To enter the bootloader - which is necessary in order to flash a new firmware - press both buttons on the back while its plugged into your computer. It should show up as a regular usb-stick in your file explorer now and you can drag the .utf onto this usb-stick. Once done it will restart and use your newly flashed firmware!
You can confirm that everything went well by opening Vial or listing the available usb-devices (`lsusb` in lin)

**Alternatively** one could download my fork of vial-qmk [here](https://github.com/ScatteredDrifter/vial-qmk) and compile the firmware themself.
For that you will have to:
1. have set up qmk and be ready to compile and flash. ( See `qmk setup` or consult [the qmk tutorial](https://docs.qmk.fm/#/newbs))
2. **find my** keyboards,  under `../keyboards/scattereddrifter/*` and choose **clacky40**.
3. make your changes
4. compile with `qmk compile --kb scattereddrifter/clacky40 --km yourKeyMap` 


### Getting PCBs:

TODO, once prototypes are functional

## Images: 

![front image of pcb](/material/images/clacky40_front_2.jpg)

![back image of pcb](/material/images/clacky40_back_1.jpg)


---

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
