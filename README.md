# Slot 8 Support for the XT-IDE 8-Bit IDE Controller

[Glitch Works](http://www.glitchwrks.com/) daughterboard for Slot 8 Support on the XT-IDE. This module can be used with any XT-IDE that includes ISA pin `B8`, which is all [rev 3](http://www.glitchwrks.com/2016/07/06/xt-ide-rev3) boards, most rev 2 boards, and early rev 1 boards. Production rev 1 boards (2009-2010 era) had `B8` removed to reduce cost, and can't use this module

More info on the Glitch Works project to provide XT-IDE related boards, kits, and fully assembled units [can be found here](http://www.glitchwrks.com/xt-ide). A writeup on the Slot 8 Support design process [is available here](http://www.glitchwrks.com/2017/02/03/slot-8-support).

### Versions

Originally there were two sets of Gerber files for this project, one with silkscreen legends, and one where the legend was done as solder mask relief. I've since dropped the silkscreened version since the "nosilk" version can be run at any board house, even those with lousy silkscreen quality. Here's the current production board, with castellated mounting holes:

![Solder Mask Relief Version](https://github.com/glitchwrks/xt_ide_slot_8_support/blob/master/proto_nosilk.png)

This version is 100% functional and the Gerbers can be submitted directly to OSH Park. You'll receive a board with [castellated holes](http://docs.oshpark.com/tips+tricks/castellation/) (which may require some deburring). OSH Park boards have been run and tested, and found to be completely functional.

### Bill of Materials

You can find a BOM with Mouser part numbers [here](https://github.com/glitchwrks/xt_ide_slot_8_support/blob/master/bill_of_materials.md). Pull requests with BOMs for other suppliers are welcome! Do note that you can purchase complete parts kits from [The Glitch Works](http://www.glitchwrks.com/xt-ide) in addition to bare PC boards.

### Notes on Running This Board

This is a single-sided board, but most (all?) board houses that do prototype quantities will run it as a double-sided board with nothing on the solder side. As such, be aware that you *do* need to include the solder side solder mask file -- solder masks are negative, so omitting the solder mask file when submitting to e.g. [OSH Park](https://oshpark.com) will result in a solid solder side mask, which will get in the through-holes and make assembly more difficult!

The design files for this board now specify [castellated holes](http://docs.oshpark.com/tips+tricks/castellation/) for the mounting tabs. Not all board houses can do this -- OSH Park can, and you can submit the Gerber ZIP directly to them and get a functional board.
