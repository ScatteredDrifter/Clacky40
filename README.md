# Clacky40: 

Yet another replacement Board for the Daisy40. 
Running with a RP2040, adapted from elmos:![Dizzy40](https://github.com/kb-elmo/Dizzy40)

--- 
## Status:
- PCB tested, _Vial support available_, working
- compatible with Case!
- minor issue with footprint fixed, pcb is fully functional now
 

## Features:
- RP2040 
- _(TODO) ZMK support_
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

Gathering PCBs is fairly simple, at least with JLCPCB ( which I usually default to and base my workflow around).
under the `/production/*` section you can find a zip-archive that contains the required gerber for the newest version of this board. 

1. upload the `*_gerber.zip` to JLCs website and select your prefered parameters ( pcb color, etc)
2. select "assembly" if you want to order this pcb **fully assembled with MCU etc** 
3. you will now have to supply the _positions_ and _bom (bill of materials)_ as **.csv**. You can find those at `/production/assembly/*` and should then upload them accordingly.
4. check whether every component is selected in the BOM-overview ( pinouts like J1 to Jx or keyswitches are listed but dont require any component, you can leave them out so to say)
5. finally confirm placement of the selected components ( usually I have them correct them anyway so its more or less a _sanity check_)
6. you have now ordered pcbs successfully

## Images:


### | Images of PCB | 

![front image of pcb](/material/images/clacky40_front_2.jpg)

![back image of pcb](/material/images/clacky40_back_1.jpg)

### | Built with Daisy40-Case from KPrepbulic | 

![built keyboard with pcb in the back](/material/images/clacky40_built_front.jpg)

![built keyboard backside](/material/images/clacky40_built_back_off.jpg)

![built keyboard backside with LEDS on](/material/images/clacky40_built_back_on.jpg)

---

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
