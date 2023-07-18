## The OS/9 MMU
In the SuperPet system, the additional 64K of RAM is only accessible in 16 banks of 4KB, mapped in the $9000-9FFF address range (usually reserved for option ROMs) with a bank select register $EFFC.

The OS/9 MMU, designed by members of the Toronto PET Users Group (TPUG) expands the SuperPET expansion RAM bank select latch at $EFFC.

With the MMU installed, when bit 5 is set at $EFFC, the 6809 can access all of the 64K in the $0000-FFFF continuous address range.

# The three connector rows

The MMU interfaces with the SuperPet boards using the 6809 processor socket and the socket of the 74LS273 $EFFC latch IC controlling the memory bank select lines.

For the original, two-board SuperPet (U9) and the Comboboard Version (U36) different units of the total of eight flip flops contained in this IC had been used. Luckily, only one of the signals needed (EFFC) isn't mirror-symmetric between the two variants.

Thus, using only 3 Rows of connectors and one jumper is enough to be able to interface with either version of the SuperPet boards.


* For *ComboBoard SuperPets*, connect the ribbon cable going to the U36 Socket on the leftmost rows and set the jumper to 1-2. (Option A)
  
![OS/9 MMU addon board Option A](https://github.com/InsaneDruid/CommonPET/blob/main/os9_mmu/images/option_a_comboboard.png) 
* For *two-board SuperPets*, connect the ribbon cable going to the U9 Socket on the rightmost rows and set the jumper to 2-3. (Option B)
  
![OS/9 MMU addon board Option B](https://github.com/InsaneDruid/CommonPET/blob/main/os9_mmu/images/option_b_dualboard.png) 
