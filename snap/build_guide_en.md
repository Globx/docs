# SNAP 

## 75% Split Keyboard Kit
![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image000.jpg)
## Build Guide

# Contents
[Helpful Links](#helpful_links)

[Parts and Tools](#parts_and_tools)

[Assembly Steps](#assembly_steps)

[Troubleshooting](#troubleshooting)


## Thanks for purchasing!

// TODO: add this section

# <a name="helpful_links"></a> 1. Helpful links
* [Default Keymap](http://www.keyboard-layout-editor.com/#/gists/890976abaf7c77d768de9a0544e3bbc8)
* [QMK Firmware]()
* [Basic Skills: Soldering](https://www.youtube.com/watch?v=UpVx4wGukRc) - Make sure you're prepared to solder your keyboard kit!
* [Check the](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image048.png) quality of your [soldering joints!](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image049.png)
* [How to use a DMM](https://www.youtube.com/watch?v=SECWePatYjY) - Important if you need to troubleshoot your build!
* [Firmware Flashing Guide](https://github.com/nullbitsco/docs/blob/main/firmware/firmware_flashing.md)

# <a name="parts_and_tools"></a> 2. Parts and tools

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image001.jpg)

// TODO: These counts are off and need to be updated.

## 1. Parts included in the kit

### Hardware
| **Item** | **Qty.** | **Image** |
| --- | --- | --- |
| Standoff, M2x3 | 13 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image002.jpg) |
| Standoff, M2x10 | 2 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image004.jpg) |
| Screw, M2x3 | 26 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image006.jpg) |
| Screw, M2x6 | 2 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image008.jpg) |
| Screw, M2x10 | 2 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image010.jpg) |
| Machined Knob | 1 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image046.jpg) |

### Electronics
| **Item** | **Qty.** | **Image** |
| --- | --- | --- |
| 1N4148 Diode | 73 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image003.jpg) |
| 0.1μF Capacitor | 2 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image005.jpg) |
| 330Ω Resistor | 3 | ![]() |
| IC Socket | 2 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image007.jpg) |
| IC (74HC138N) | 2 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image009.jpg) |
| Reset Switch | 1 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image011.jpg) |
| WS2812B LED | 10 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image042.jpg) | 
| TRRS Jack | 1 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image043.jpg) |
| Rotary Encoder | 1 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image044.jpg) |
| Big RGB LED | 1 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image045.jpg) |
| Breakaway Header Pins | 40 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image047.jpg) |

### Core

| **Item** | **Qty.** | **Image** |
| --- | --- | --- |
| Top PCB plate | 1 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image012.jpg) |
| Bottom PCB plate | 1 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image013.jpg) |
| Middle acrylic spacer | 1 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image014.jpg) |
| Top acrylic guard | 1 | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image015.jpg) |

## 2. Parts you provide

- PCB-mount switches (Cherry MX footprint)
- PCB-mount stabilizers. Snap requires 5x 2u stabs. You’ll want 2x 2u stabs, one for each spacebar, along with 3x additional for left shift, enter, and backspace.
- Keycaps: [(black set pictured in product photos)](https://drop.com/buy/dsa-dolch-key-set) [(white set in product photos)](https://www.amazon.com/Sublimated-Suitable-Switches-Mechanical-Keyboard/dp/B07QN9128Z?th=1)
- [BIT-C](https://nullbits.co/bit-c/) or other Pro Micro compatible MCU
- **[OPTIONAL]** [0.91" 128x32 OLED Display](https://www.amazon.com/dp/B08KL8YKVW)
- **[OPTIONAL]** [FR4 switch plate](http://www.amazon.com/dp/B08KLGRS69)
- **[OPTIONAL]** Qty. 180 Mill-Max 0305 or 7305 hot-swap solder sockets


## 3. Tools required

- Fine-tip soldering iron &amp; solder
- Needle nose pliers
- Phillips #0 screwdriver
- Snips for cutting leads
- Rubbing alcohol
- **[Recommended]** DMM/Multimeter
- **[Recommended]** USB Current Meter

# <a name="assembly_steps"></a> 3. Assembly Steps

⚠️ **Important!** Notes marked with this icon are crucial, so be sure to read them carefully before moving on.

Steps marked [OPTIONAL] aren&#39;t required for the base kit, but may be needed depending on what you choose to include in your build.

## 1. [OPTIONAL] Solder Underglow LEDS

[Recommended resource: soldering 5050 SMT LEDs](https://electronics.stackexchange.com/questions/482626/how-to-solder-ws2812b-ledsindividual-not-a-strip-to-a-pcb)

Solder the 10x WS2812B underglow LEDs, 5x on each keyboard half. Start by tacking down one corner, and then soldering the remaining 3 leads. After soldering, clean with rubbing alcohol.

⚠️ **Orientation matters!** These parts have a small angled mark which should match up with the one on the PCB. If you don&#39;t get the orientation right, the LEDs will not work, and your keyboard may not boot up.

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image016.jpg)


## 2. Bend and solder resistors

Bend and solder R1 on each keyboard half.

| ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image017.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image018.jpg) |
| --- | --- |

After soldering, clean with rubbing alcohol and use the snips to clip the leads as close to the PCB as possible.


## 3. Solder reset switch

Fit and solder the reset switch on each keyboard half as shown below.

| ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image019.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image020.jpg) |
| --- | --- |

After soldering, clean with rubbing alcohol.


## 4. Solder IC sockets

Fit and solder the two IC sockets; one on each keyboard half. Match the notch in the socket with the one on the PCB. After soldering, clean with rubbing alcohol. **Note: if you accidentally solder one or both sockets backward, don't panic! The sockets are passive components and will work in either orientation. The notches make it easier to insert the IC in the right direction, so just make sure to insert the IC in the correct direction later on in the build.**

⚠️ **Do not solder the socket with the IC inserted!** The heat may damage the chip if it is in the socket during soldering.

| ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image021.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image022.jpg) |
| --- | --- |


## 5. Solder caps

Fit and solder the two capacitors; one on each keyboard half.

| ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image023.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image024.jpg) |
| --- | --- |

After soldering, clean with rubbing alcohol and use the snips to clip the leads as close to the PCB as possible.


## 6a. Bend and solder under-key diodes

There are a number of diodes that aren't in the main group on the top of the keyboard: 13 on the left half, and 11 on the right half. Bend and fit the 1N4148 diodes. Bend the leads inward to hold the diodes in place when the PCB is turned upside down. Begin by soldering one side of the diodes and adjust the diode alignment to your liking before soldering the second lead.

⚠️ **Orientation matters!** Solder the diodes with the black bar **UP** as shown in the images. The keyboard will not work if they are backward.

| ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image025.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image026.jpg) |
| --- | --- |

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image027.jpg)

## 6b. Bend and solder top row of diodes

Bend and fit the remaining 1N4148 diodes for the top row. Bend the leads inward to hold the diodes in place when the PCB is turned upside down. Begin by soldering one side of the diodes and adjust the diode alignment to your liking before soldering the second lead.

⚠️ **Orientation matters!** Solder the diodes with the black bar **UP** as shown in the images. The keyboard will not work if they are backward.

| ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image025.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image026.jpg) |

After soldering all diodes, clean with rubbing alcohol and use the snips to clip the leads as close to the PCB as possible.

# ⚠️ **STOP** ⚠️

It&#39;s highly recommended that you flash the MCU (Bit-C or Pro Micro) before soldering it so you can be sure it&#39;s working properly. [Jump to step](#firmware_flashing) 20 to flash QMK firmware.


## 7. Solder MCU

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image040.jpg)

Use header pins to solder the MCU to the keybpard. Fit and solder the BIT-C or Pro Micro MCU as shown below using 0.1" male header pins. After soldering, clean with rubbing alcohol and use the snips to clip the pins as close to the PCB as possible.

## 7. Solder Pogo Pins

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image040.jpg)

Solder the included pogo pins on the **Bottom Side** of the PCB. The male pogo pins go on the left half of the keyboard, and the female pins go on the right half.

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image028.jpg)

## 8. [OPTIONAL] Solder TRRS expansion jack

The TRRS footprint directly under the MCU is for the expansion jack. You can connect a TIDBIT without needing another USB cable! If you want to use this feature, you can solder the TRRS jack underneath the MCU of choice (left or right).

| ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image029.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image030.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image031.jpg) |
| --- | --- | --- |

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image051.png)


After soldering, clean with rubbing alcohol and use the snips to clip the leads as close to PCB as possible.


## 8. [OPTIONAL] Solder rotary encoder, speaker, and/or OLED

If building with the optional rotary encoder, speaker, or OLED display in place of the programmable macro keys, fit and solder each in the position each shown. After soldering, clean with rubbing alcohol and use the snips to clip the pins as close to the PCB as possible. Do not clip the large support pins on the encoder.

| ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image029.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image030.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image031.jpg) |
| --- | --- | --- |

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image051.png)



## 9. Insert ICs into IC sockets

⚠️ **Orientation matters!** Make sure that the side of the IC with the round mark is closest to the Bit-C on the left half and furthest from the Bit-C on the right half (both facing left) before inserting. Double check before inserting if you're not sure! The orientation should match the silkscreen.

Carefully bend the IC leads inward so that they are the width of the socket. It helps to set the IC on its side on a flat surface and use a tool to bend all leads at once.

While supporting the back of the PCB with one hand, push on the top of the IC using your thumb until it sits flush in the socket. If you feel leads bending, stop and carefully straighten them before continuing.

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image032.jpg)


## 10. Choose key layout and configuration

The snap PCB includes guide marks for the switches and stabilizers to make their placement easier. The center of each switch lines up with a letter for a particular layout. The tables below show which markings to follow based on key configuration. Familiarize yourself with the [standard layout](http://www.keyboard-layout-editor.com/#/gists/890976abaf7c77d768de9a0544e3bbc8).

⚠️ **Compatibility note:** Not all combinations are compatible with each other! See the compatibility notes in the table. Double-check that the chosen configuration matches your keycaps before soldering.

# ⚠️ **STOP** ⚠️

It&#39;s highly recommended that you test each key at this point before continuing. If you haven&#39;t already, [Jump to step](#firmware_flashing) 20 to flash QMK firmware. Use a keyboard tester ([this one](https://www.keyboardtester.com/) works) and short the switch pads for each switch using tweezers, a clipped lead from earlier, or something else conductive. If there is an issue, it will be much easier to debug now before everything has been soldered and assembled.

**Caps lock** 
| **Guide Mark** | **Layout Option** |
| --- | --- |
| A | Stepped 1.75U Caps Key |
| B | Standard 1.75U Caps Key |

**Left modifiers**
| **Guide Mark** | **Layout Option** |
| --- | --- |
| C | 3x 1.25U Modifiers |
| D | 2x 1.5U Modifiers |

**Spacebar**
| **Guide Mark** | **Layout Option** |
| --- | --- |
| E | 6.25U spacebar _**Only compatible with &quot;C&quot;**_ |
| F | 7U spacebar _**Only compatible with &quot;D&quot;**_ |
| G | 2.75U + 1U + 2.25 split spacebar _**Only compatible with &quot;C&quot;**_ |

**Right modifiers**
| **Guide Mark** | **Layout Option** |
| --- | --- |
| H | 3x 1U Modifiers |
| I | 2x 1.5U Modifiers _**Recommended when using &quot;G&quot;**_ |

**Left Shift**
| **Guide Mark** | **Layout Option** |
| --- | --- |
| J | 2.25U ANSI |
| K | 1.25U + 1U ISO |

**Enter Key**
| **Guide Mark** | **Layout Option** |
| --- | --- |
| L | 2.25U ANSI |
| M | 1.25U + 1U ISO |

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image033.jpg)


## 11. Screw together M2x3 standoffs using M2x3 screws

In the locations shown, screw the M2x3 standoffs into the **TOP** PCB plate. Fasten using 14 M2x3 screws (7 on each half). Use pliers to hold the standoff steady while tightening the screw. **Do not overtighten!** This step is extra important if you are building with a plate, since it's more difficult to access the screws with the plate in place.

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image034.jpg)


## 12. Snap in stabilizers

Snap in the PCB-mount stabilizers as shown below. The tab goes in the big hole, and the retaining clips go in the small holes. The stabilizers will only snap in one way. Make sure the stabilizer is fully seated, or the keycap won&#39;t move properly once it&#39;s installed.

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image035.jpg)


## 13. [OPTIONAL] Insert hot-swap sockets

If building with hotswap sockets, drop one into each plated lead hole and affix with tape (masking or electrical tape works well). Alternatively, insert them onto each lead of the PCB mount switch before proceeding.


## 14. Snap in switches

⚠️ **Stop!** Test fit your keycaps to make sure that the switch spacings are correct before soldering, especially the bottom row.

If you are using 5-pin PCB mount switches, they may take some force to insert. This is by design. For PCB mount switches, a tight fit makes the switches more stable. Snap in by supporting the back of the PCB, and then pushing hard on the top of the switch. It helps to use a spare keycap on the switch to take some of the pressure off your thumb. After snapping the switch in, make sure it&#39;s sitting flush against the PCB.

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image036.jpg)


## 15. Solder switches or hot-swap sockets

⚠️ **Stop!** If you are building with a switch plate, make sure that you have installed and tightened the mounting hardware ( **Step 2.11** ) and installed the stabilizers ( **Step 2.12** ) before continuing! Once the switches are installed on the plate, access to the items below is difficult.

Make sure each switch pin has enough solder to form a nice solid joint.


## 16. Slide the acrylic spacer onto the standoffs

Make sure the acrylic spacer sits flat against the PCB plate. Check for interreferences due to leads or solder joints. Trim if needed.

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image037.jpg)


## 17. Fasten the bottom with M2x3 screws

Place the bottom PCB plate on top of the acrylic spacer. In the same locations where the 14 standoffs were installed, fasten with 14 M2x3 screws (7 on each half). **Do not overtighten!**

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image038.jpg)


## 18. Fasten M2x10 standoffs from bottom using M2x10 screws

Fasten using 2 M2x10 screws. Use pliers to hold the standoff steady while tightening the screw.

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image039.jpg)


## 19. Attach the top guard using M2x6 screws

Fasten using 2 M2x6 screws. Don&#39;t overtighten these, as it can crack the top guard.

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image040.jpg)


## 20. <a name="firmware_flashing"></a> Flash firmware using QMK toolbox

Download either a precompiled binary (only if using a Pro Micro or BIT-C) or the QMK source files from [GitHub](https://github.com/nullbitsco/snap). Using [QMK Toolbox](https://qmk.fm/toolbox/), flash the firmware onto the keyboard. For more information, follow the [Firmware flashing guide](https://github.com/nullbitsco/docs/blob/main/firmware/firmware_flashing.md)


## 21. Enjoy!

![](https://github.com/nullbitsco/docs/raw/main/snap/build_guide_img/image041.jpg)


# <a name="troubleshooting"></a> 4. Troubleshooting

**None of the keys are working**

- Is the firmware loaded?
- Try with a different USB cable, USB port, and PC.
- If you soldered the LEDs, check that none have been soldered backward. The keyboard will not work if an LED was mistakenly soldered backward.
- Check the direction of the diodes. The back bar should be facing upwards.
- Check the direction of the ICs. The keyboard will not work if they are in the socket backward.
- Check that there are no shorts and that the keyboard is powering up properly.

**A single key is not working**

- Check that the switch is soldered properly at both pins.
- Bypass the switch by shorting the two pads with tweezers. If that works, the switch is to blame and should be replaced. If it does not, the diode soldering is likely the issue.
- Check that all of the diodes are soldered properly at both pins.
- Check that the keymap you are using is defined correctly and matches your keyboard layout.

**A whole row is not working**
 
- This is usually caused by a cold solder joint at the Bit-C. Check that all pins on the MCU are soldered properly.
- Check that the proper rows and columns are set in QMK config.h

**A whole column is not working**

- Check that all pins on the MCU are soldered properly.
- Check that the proper rows and columns are set in QMK config.h
- Check that all pins on the ICs are soldered properly.

**The rotary encoder is not working**

- Check that all pins on the rotary encoder are soldered properly.
- Check that the A and B pins are set in QMK config.h and that ENCODER\_ENABLE = yes in QMK rules.mk.

**The OLED is not working**

- The OLED is not enabled in the default firmware. Load the 'oled' firmware, available on the QMK repo. 

**Two or more keys are swapped**

- Check that the keymap you are using is defined correctly and matches your keyboard layout.

**The underglow LEDs are not working**

- Check that the RGB\_DI\_PIN pin is set in QMK config.h and that RGBLIGHT\_ENABLE = yes in QMK rules.mk.
- Check that all LEDs are soldered in the proper orientation.

**There&#39;s no power**

- Check that all LEDs are soldered in the proper orientation.
- Check the direction of the ICs.
- Check for other shorts – solder blobs, leads that were not clipped all the way, etc.

**How to I do X in firmware?**

- See the QMK docs, or make a post on r/olkb for help.
- Make a post on the [r/nullbits](https://www.reddit.com/r/nullbits/) subreddit, or join the #firmware channel in the [nullbits discord server](https://discord.gg/eSegJcY).

**Something else?**

- Visit [nullbits.co/support/](https://nullbits.co/support/)
- Reach out at [help@nullbits.co](mailto:help@nullbits.co)
- Join our [Discord](https://discord.gg/eSegJcY)!

snap 0x3 Assembly Instructions Rev04 03.25.20
