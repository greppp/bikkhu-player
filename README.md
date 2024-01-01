# bikkhu-player

This page documents the build of a small mp3 player with two buttons. The first one will trigger a random track from the first folder, the second one a random track from the second folder. The idea here is the user loads meditation tracks in the two folders, the first one being tracks with shorts instructions (a.k.a, mostly silence, only istructions at the begining and the end, to use when you feel quite focused). The second one is loaded with tracks with long instructions (a.k.a, not much silence, you're guided the whole time, to use when your mind is quite volatile).

The microcontroller used here is a Seednuino Xiao SAMD21, which I choosed for it's amazing form factor while offering USB-C connectivity and being Arduino IDE compatible.

The MP3 player used here is a DY-SV19T, which I choosed for it's ease of control, size ratio, SD card, and on-board amp.

The speaker used is a Huawei Google Nexus 6P Speaker, which I used in the past to upgrade the speakers of an X230, and offers a very good sound quality for it's size and price.

The pcb layout was done in Kicad.

Parts list:
-----------
1x......SAMD21 Seeduino Xiao.......................http://tinyurl.com/v936x666
1x......DY-SV19T MP3 Module........................http://tinyurl.com/5n7a68ca
1x......Huawei Google Nexus 6P Speaker.............http://tinyurl.com/543xytvt
2x......Micro Push Buttons 6x6x9.5mm w/ LED .......http://tinyurl.com/5ejt6jdb
1x......2N3904 transistor..........................http://tinyurl.com/md94f5cp
3x......1k resistor through hole...................http://tinyurl.com/53njj8zz
3x......10k resistor through hole..................http://tinyurl.com/ataa6tsh

Assembly

A couple of general soldering rules

Start with the SAMD21, making sure you are aligned with the silkscreen. Then proceed with the DY-SV19T.
