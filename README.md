A collection of information on ATmegaxxx4 Arduino variant files
==========

Although never used in an official [Arduino](http://arduino.cc) board, the ATmega644P and ATmega1284P has a long history of use in 3rd party Arduino hardware. These chips have several factors that make them attractive to the Arduino community:
- Availability in a breadboard-friendly, easy to solder DIP-40 package.
- Lots of memory.
- Plenty of IO pins.
- Well supported by 3rd party hardware packages.

Unfortunately the lack of an official pin mapping has lead to a plethora of pin mappings as each 3rd party hardware designer created their own. This can make it quite difficult for developers to provide good compatibility for these parts. This repository contains information on all existing Arduino variants for this chip family which hopefully can make this easier. Some of these variants are quite obscure but all known variants have been included for the sake of being thorough.

Please don't create any more pin mappings. We have far too many already. Certainly one of the existing ones should be suitable. The more common mappings should be preferred, especially **standard**, **bobuino**, or **sanguino**.

Note that, although the ATmega1284P and ATmega644P are the most commonly used, these variant files can be easily adapted to support other 32 IO pin AVR models such as ATmega324, ATmega164, ATmega32, ATmega16, and ATmega8535. The excellent [MightyCore](https://github.com/MCUdude/MightyCore) has done just that for the **[bobuino](https://github.com/MCUdude/MightyCore/blob/master/avr/variants/bobuino/pins_arduino.h)**, **[sanguino](https://github.com/MCUdude/MightyCore/blob/master/avr/variants/sanguino/pins_arduino.h)**, and **[standard](https://github.com/MCUdude/MightyCore/blob/master/avr/variants/standard/pins_arduino.h)** variants.

### Files
- [Pin Mapping Table](pin-mappings.tsv)
  - All known Arduino pin mappings of this chip family.
- [Variant Table](variants.tsv)
  - All known Arduino variants for this chip family. Multiple variants may use the same pin mapping.
- [Boards Table](boards.tsv)
  - All known boards that use this chip family.
- [Variant Files](variants/)
  - These are the source files for the information contained in this repository. They are stored here for the sake of preserving them from bit rot. If possible, I recommend using the official versions of these files, which are located at the Source URLs provided in the Variants Table.

### Contributing
If you find an error, want to suggest an improvement, or have found an additional variant please open a Pull Request or Issue. Thanks!
