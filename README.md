# bikkhu-player

## Project Overview

An audio player featuring two 'play random track' buttons, each linked to a different folder on the SD card. 

The player is primarily intended for use as an audio support for meditation, with one folder containing audio tracks with short instructions, and the other containing tracks with long instructions.

It contains an onboard speaker, an SD card reader, a volume knob, and a USB-C connector.

## The hardware 

- A seeeduino XIAO SAMD21 --- Arduino compatible, USB-C, ultra compact, castellated vias.
- A DY-SV19T audio player --- WAV/MP3 decoder, UART enabled, SD card reader, onboard 5W amp, low cost, castellated vias.
- A Huawei Google Nexus 6P Speaker --- 4 ohms, low profile, decent sound.
- 2 push buttons, 1 potentiometer, 1 NPN transistor, some resistors
- A custom pcb

## Bill Of Materials

|Qty|Designation|Link|
|---|---|---|
|1|SAMD21 Seeduino Xiao|[buy](https://www.digikey.ca/en/products/detail/seeed-technology-co-ltd/102010328/11506471)|
|1|DY-SV19T|[buy](https://www.aliexpress.com/item/1005004486314473.html)|
|1|Huawei Google Nexus 6P Speaker|[buy](https://www.aliexpress.com/item/32811356640.html)|
|2|Micro Push Buttons 6x6 w/ LED|[buy](https://www.aliexpress.com/item/1005001680172078.html)|
|1|Trimmer potentiometer 10k|   |
|1|2N3904 NPN transistor|[buy](https://www.digikey.ca/en/products/detail/onsemi/2N3904BU/1413)|
|3|1k resistor through hole|[buy](https://www.digikey.ca/en/products/detail/yageo/MFR-25FRF52-1K/14891)|
|1|Bikkhu player pcb V1.1|   |


## About the DY-SV19T

- Support MP3,WAV decoding format
- Support sampling frequency (KHz) : 8/11.025/12/16/22.05/24/32/44.1/48
- UART serial port control (baud rate: 9600 bit/s)
- Onboard 5W Class D amplifier circuit can directly drive 4ohm 3~5W speakers
- 24-bit DAC output, dynamic range support 90dB, SNR support 85dB
- Can read SD cards up to 32GB (FAT 32 format)
- Supply voltage: 3.7V~5V DC 
- Logic level : 3.3V
- Onboard 4.7K pull-up/down resistors already present (for mode selection)

## Assembly

Some general soldering rules:

Use "no-clean solder" for longevity of your circuit. If you're a beginner, use leaded solder (60/40) no clean. If you use lead free, make sure it has silver in it.



Start with the SAMD21, making sure you are aligned with the silkscreen. Then proceed with the DY-SV19T. Then the resistors (keep 2 clipped legs aside),  then switches, potentiometers. Lastly, the speaker. Glue it in place with thick mounting tape (I used 3M extreme mounting tape) then use the clipped legs from the resistors to solder to the connections.

