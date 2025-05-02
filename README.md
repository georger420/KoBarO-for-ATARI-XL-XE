# KoBarO-for-ATARI-XL/XE

Application for 8 bit ATARI XL or XE with at least 64 kb memory.

## Description

Following two pictures sey more, then long text:

The input is four color picture (Graphics 3, 5, 7 and 16):

![Space Lobsters](/pc-pictures/spalob_gr7.png)

The output is two color picture (Graphics 8):

![Space Lobsters](/pc-pictures/spalob_gr8.png)

In a nutshell, each color pixel in source picture is replaced by raster in target two color picture. Rasters are chosen according to brightness of original pixel. More detailed description is in [user guide](./kobarog_user_guide.pdf)

Application is written in ATARI BASIC and machine code. While ATARI BASIC is used mainly for user interface and for some not speed critical operations, machine code is used mainly for loading of pictures in Koala (compressed) format and also for conversion.

Here is [ATR disk image](./release/kobarog_master.ATR) and also standalone [xex executable](./release/KOBAROG.xex). Both are working in [Altirra emulator](https://virtualdub.org/altirra.html) and also in [ATARI800 emulator](https://atari800.github.io/) with "Atari XL/XE OS ver.2" and "Atari BASIC rev. C" firmware. Altirra basic was not tested.

Machine code is placed from $2000 address, basic program starts some bytes after $2800 address.

All preserved souce codes are placed in [src](./src/) directory. Unfortunately some machine code source code has not been preserved.

## Links

Most part of graphics editors for ATARI XL/XE mentioned in user guide are available on www.atarimania.com:

[DrawIt!](https://www.atarimania.com/utility-atari-400-800-xl-xe-drawit_29938.html)

[Design Master](https://www.atarimania.com/utility-atari-400-800-xl-xe-design-master_12516.html)

[Fun With Art](https://www.atarimania.com/utility-atari-400-800-xl-xe-fun-with-art_27410.html)

[Koala Micro Illustrator](https://www.atarimania.com/utility-atari-400-800-xl-xe-micro-illustrator_30240.html)

[MicroPainter](https://www.atarimania.com/utility-atari-400-800-xl-xe-micro-painter_31609.html)

[Ranbrandt](https://www.atarimania.com/utility-atari-400-800-xl-xe-rambrandt_12480.html)

Some applications are available on "Internet Archive":

[SAM Painter](https://archive.org/details/a8b_Screen_Aided_Management_v1.2_1987_Raindorfsoft)

[Magic Painter](https://archive.org/details/a8b_Magic_Painter_Documentation_1984_Fischer_Ralf_Manseicher_Harald)

Turbo 2000 Casette Operating system TOS 4.1 is available in [Česko slovenský archív programov pre ATARI XE/XL](http://atari.turiecfoto.sk/soft/):

[TOS 4.1](http://atari.turiecfoto.sk/soft/tos-41.zip)

To make the user manual look as if it was printed on an ATARI 1029 printer, a special font from [jeffpiep's](https://github.com/jeffpiep) repository was used:

[ATARI 1029 printer font](https://github.com/jeffpiep/Atari-Printer-Fonts/tree/master/Atari1029)
