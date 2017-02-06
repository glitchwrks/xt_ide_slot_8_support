# Slot 8 Support for the XT-IDE 8-Bit IDE Controller

*Caution: Work in Progress! Only submit the slot8_nosilk.zip file at the moment!*

[Glitch Works](http://www.glitchwrks.com/) daughterboard for Slot 8 Support on the XT-IDE. This module can be used with any XT-IDE that includes ISA pin `B8`, which is all [rev 3](http://www.glitchwrks.com/2016/07/06/xt-ide-rev3) boards, most rev 2 boards, and early rev 1 boards. Production rev 1 boards (2009-2010 era) had `B8` removed to reduce cost, and can't use this module

More info on the Glitch Works project to provide XT-IDE related boards, kits, and fully assembled units [can be found here](http://www.glitchwrks.com/xt-ide). A writeup on the Slot 8 Support design process [is available here](http://www.glitchwrks.com/2017/02/03/slot-8-support).

### Versions

There are two sets of Gerber files, one with silkscreen legends, and one where the legends are done in solder mask relief. The version using solder mask relief is what the Glitch Works kits include, and can be run through board houses that have lousy silkscreen quality.

![Silkscreen Version](https://github.com/glitchwrks/xt_ide_slot_8_support/blob/master/proto.png) ![Solder Mask Relief Version](https://github.com/glitchwrks/xt_ide_slot_8_support/blob/master/proto_nosilk.png)

### Bill of Materials

You can find a BOM with Mouser part numbers [here](https://github.com/glitchwrks/xt_ide_slot_8_support/blob/master/bill_of_materials.md). Pull requests with BOMs for other suppliers are welcome! Do note that you can purchase complete parts kits from [The Glitch Works](http://www.glitchwrks.com/xt-ide) in addition to bare PC boards.

### Notes on Running This Board

This is a single-sided board, but most (all?) board houses that do prototype quantities will run it as a double-sided board with nothing on the solder side. As such, be aware that you *do* need to include the solder side solder mask file -- solder masks are negative, so omitting the solder mask file when submitting to e.g. [OSH Park](https://oshpark.com) will result in a solid solder side mask, which will get in the through-holes and make assembly more difficult!
