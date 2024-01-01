# bikkhu-player

This page documents the build of a small mp3 player with two buttons. The first one will trigger a random track from the first folder, the second one a random track from the second folder. The idea here is the user loads meditation tracks in the two folders, the first one being tracks with shorts instructions (a.k.a, mostly silence, only istructions at the begining and the end, to use when you feel quite focused). The second one is loaded with tracks with long instructions (a.k.a, not much silence, you're guided the whole time, to use when your mind is quite volatile).

The microcontroller used here is a Seednuino Xiao SAMD21, which I choosed for it's amazing form factor while offering USB-C connectivity and being Arduino IDE compatible.

The MP3 player used here is a DY-SV19T, which I choosed for it's ease of control, size ratio, SD card, and on-board amp.

The speaker used is a Huawei Google Nexus 6P Speaker, which I used in the past to upgrade the speakers of an X230, and offers a very good sound quality for it's size and price.

The pcb layout was done in Kicad.


DY-SV19T


1.Description:

DY-SV19T integrates I/O subsection triggering, UART serial port control, ONE_line single bus serial port control,standard MP3 and other 7 working modes; Onboard 5W Class D amplifier circuit and can directly drive 4ohm 3~5W speakers.Support MP3,WAV decoding format. Support memory card (TF card) up to 32GB/FAT32 format; Support external volume adjustment potentiometer, configure the pin without welding pull-up/pull-down resistance, reserve USB external pin to facilitate external download interface.


2.Features:

1>.Support MP3 and WAV decoding format;

2>.Support sampling frequency (KHz) : 8/11.025/12/16/22.05/24/32/44.1/48;

3>.24-bit DAC output, dynamic range support 90dB, SNR support 85dB;

4>.Support memory card (TF card) up to 32GB, easy to replace audio files;

3>.Built in 5W Class D amplifier circuit and can directly drive 4ohm 3~5W speaker;

6>.Support UART serial port control voice broadcast function.It can control playback, pause, selections, turn up and down volume and other functions, the largest selection of 65535 songs.The baud rate is 9600 bit/s.

7>.Support I/O trigger function, 8bit I/O ports can trigger 8 musics or 8 I/O combinations to trigger 255 songs.

8>.Support One_line single bus serial port control, which can control playback, pause, selection, turn up and down volume and other functions.

9>.Support 3 configuration I/O for mode selection to make 7 work mode.

10>.Support external volume potentiometer adjustment.

11>.Supports external USB download port.


3.Parameter:

1>.Model:DY-SV19T

2>.Work Voltage:DC 3.7V~5V

3>.Work Temperature:-25℃~85℃

4>.Work Humidity:5%~95%RH

5>.Size:30*23mm




## Parts list:
-----------
- 1x......SAMD21 Seeduino Xiao.......................http://tinyurl.com/v936x666
- 1x......DY-SV19T MP3 Module........................http://tinyurl.com/5n7a68ca
- 1x......Huawei Google Nexus 6P Speaker.............http://tinyurl.com/543xytvt
- 2x......Micro Push Buttons 6x6x9.5mm w/ LED .......http://tinyurl.com/5ejt6jdb
- 1x......2N3904 transistor..........................http://tinyurl.com/md94f5cp
- 3x......1k resistor through hole...................http://tinyurl.com/53njj8zz
- 3x......10k resistor through hole..................http://tinyurl.com/ataa6tsh

## Assembly

Some general soldering rules:

Use "no-clean solder" for longevity of your circuit. If you're a beginner, use leaded solder (60/40) no clean. If you use lead free, make sure it has silver in it.



Start with the SAMD21, making sure you are aligned with the silkscreen. Then proceed with the DY-SV19T. Then the resistors (keep 2 clipped legs aside),  then switches, potentiometers. Lastly, the speaker. Glue it in place with thick mounting tape (I used 3M extreme mounting tape) then use the clipped legs from the resistors to solder to the connections.

