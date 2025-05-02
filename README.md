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

