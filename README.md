# Clacky40: 

Yet another replacement Board for the Daisy40. 
Running with a RP2040, adapted from elmos:![Dizzy40](https://github.com/kb-elmo/Dizzy40)

--- 
## Status:
- prototypes ordered and on the way!
- PCBs not tested 
- compatibility with case not validated ( should fit however)

## Features:
- RP2040 
- likely ZMK firmware
- supports two encoders
- additional layout options
- additional pinouts for additional LEDS ( 5V+, GND, GPIO)

--- 

## Layouting:
![image of available layouts](/material/images/kle_layout.png)

## Firmware:
pre-compiled file for vial can be found in the **"/firmware"** section.
To enter the bootloader - which is necessary in order to flash a new firmware - press the button next to the encoder on the back of the pcb and plug-it into your keyboard while keeping the button pressed. It should show up as a regular usb-stick in your file explorer now and you can drag the .utf onto this usb-stick. Once done it will restart and use your newly flashed firmware!


## Building your own:

On the verge to build this keyboard your own?
Below you can find a little guideline on what is required and how to obtain everything: 

### Getting PCBs:

TODO, once prototypes are functional

---

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
