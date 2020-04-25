# ATMEGA328 SMD Bootloader Flashing

This is a little project I built to be able to flash my ATMEGA328 SMD chips with an Arduino bootloader.

I allways use the [Optiloader](https://github.com/WestfW/OptiLoader). To flash it to an out-of-factory chip you need to connect the RESET, MISO, MOSI & SCK pins. Additionally a crystal and +5V are required. I designed this simple shield for an Uno with the mentioned connections.

![KiCad PCB](pics/PCB_Kicad.png)

The used components are just a 10k pullup resistor for the RESET pin, a 16MHz crystal with two 22pF capacitors and a few pin headers.

I milled the PCB on my desktop CNC with a 60° V-bit. 
