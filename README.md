# The CommonPET
The CommonPET is a 100% compatible replica of the SuperPet combo board for PET/CBM 8032 computers from 1981.
It implements all the features, including the 64K RAM addon, compatibility for the OS9 MMU well as the support for the internal RS-232 connector.

![CommonPET render](https://github.com/InsaneDruid/CommonPET/blob/main/images/CommonPET_render.png)

Most of the components are readily available. Chips not available from Mouser or Digikey can still be purchased as NOS from a variety of sources.

[Schematic](https://github.com/InsaneDruid/CommonPET/blob/main/CommonPET.pdf "Schematic")  

[Bill of Materials](https://htmlpreview.github.io/?https://github.com/InsaneDruid/CommonPET/blob/main/bom/CommonPET_bom.html "Bill of Materials")
## The Firmware
The Firmware of the SuperPET is available at zimmers.net: http://www.zimmers.net/anonftp/pub/cbm/firmware/computers/pet/SuperPET/index.html

UA3: characters.901640-01.bin (PETside CharROM):

U47: waterloo-a000-bfff.970018-12.bin

U48: waterloo-c000-dfff.970019-12.bin

U49: waterloo-e000-ffff-970034-12.bin (50Hz Version)

U49: waterloo-e000-ffff.970020-12.bin (60Hz Version)

Adapters to use 2764 EPROM work, 27hc641 that are programmed to be pin compatible to 2364 are recommended.

## The RS232 interface
CBM in its infinite wisdom only provided +5V and -9V for the 1488 line driver. A low voltage 1488E or 14C88 is recommended.

## The OS/9 MMU addon board
A replica of the OS/9 addon board can be found in the [os9_mmu folder](https://github.com/InsaneDruid/CommonPET/blob/main/os9_mmu/ "os9_mmu folder")

![OS/9 MMU addon board render](https://github.com/InsaneDruid/CommonPET/blob/main/os9_mmu/images/os9_mmu_render.png) 

## The License
This work is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.  
See https://creativecommons.org/licenses/by-sa/4.0/.

## The Credits
This work would not have been possible without the help from a bunch of amazing people from [VzEkC e. V. forums](https://forum.classic-computing.de/forum/ "forum.classic-computing.de"). Many thanks go out to:

* *for(;;)* - for creating the amazing µMMF project that inspired this work
* *vossi* - for providing excellent images of a ASSY 324100 board
* *CBM_Ba* and *Richi*- for building and testing the first prototype

Special credits go out to *Mike Naberezny* for researching the OS/9 MMU schematics
