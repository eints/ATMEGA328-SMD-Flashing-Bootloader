# ATMEGA328 SMD Bootloader Flashing

![Uno Flashing Shield](pics/IMAG2413.jpg)

This is a little project I built to be able to flash my ATMEGA328 SMD chips with an Arduino bootloader.

I allways use the [Optiloader](https://github.com/WestfW/OptiLoader). To flash it to an out-of-factory chip you need to connect the RESET, MISO, MOSI & SCK pins. Additionally a crystal and +5V are required. I designed this simple shield for an Uno with the mentioned connections.

![KiCad PCB](pics/PCB_Kicad.png)

The used components are just a 10k pullup resistor for the RESET pin, a 16MHz crystal with two 22pF capacitors and a few pin headers.

I milled the PCB on my desktop CNC with a 60° V-bit. The resulting PCB looks like this:
![Shield on Uno Front](pics/IMAG2404.jpg)
![Shield on Uno Back](pics/IMAG2414.jpg)

To press the chip onto the PCB the 3D printed chip holder is used.
![The Chip Holder](pics/IMAG2405.jpg)
The chip perfectly fits in the recess. At first the recess was slightly to large. I could have reprinted the older with a smalle recess but roughing the inner walls of the recess with a knive solved the problem for me. Now the chip kind of klicks in.
![Inserting Chip](pics/IMAG2406.jpg)
![Chip Inserted](pics/IMAG2407.jpg)
Four bolts guarantee the alignment of chip and PCB. I use broken drill/mill bits from my CNC. Magnets in the holder and on the backside of the PCB apply slight pressure to ensure a reliable contact.
![Mounting the Holder on the PCB](pics/IMAG2408.jpg)

When the chip is in place the bootloader is flashed.
![Mounted Holder](pics/IMAG2409.jpg)

Here is the flashed chip ready to be used in the next project!
![Removing Flashed Chip](pics/IMAG2411.jpg)