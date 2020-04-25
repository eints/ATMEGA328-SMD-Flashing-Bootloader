# ATMEGA328 SMD Bootloader Flashing

![Uno Flashing Shield](pics/IMAG2413.jpg)

This is a little project I built to be able to flash my ATMEGA328 SMD chips with an Arduino bootloader.
There are professional solutions like here https://www.youtube.com/watch?v=GFyr9tVEHzQ. 
But for the 5 to 10 Chips I need to flash from time to time I couldn't justify to buy such a thing. 
I wanted to have something cheap and easy to use. Thus I built my own simple board.

I always use the [Optiloader](https://github.com/WestfW/OptiLoader). 
To flash it to an out-of-factory chip you need to connect the RESET, MISO, MOSI & SCK pins. 
Additionally a crystal and +5V are required. I designed this simple shield for an Uno with the mentioned connections.

<img src="pics/PCB_Kicad.png" width="250"> 

The used components are just a 10k pull-up resistor for the RESET pin, a 16MHz crystal with two 22pF capacitors and a few pin headers.

I milled the PCB on my desktop CNC with a 60° V-bit. The resulting PCB looks like this:
| PCB Front      | PCB Back with magnet  |
|------------|-------------|
| <img src="pics/IMAG2404.jpg" width="250">  | <img src="pics/IMAG2414.jpg" width="250">  | 


To press the chip onto the PCB the 3D printed chip holder is used.

<img src="pics/IMAG2405.jpg" width="350">

The chip should fit perfectly in the recess. At first the recess was slightly to large. 
I could have reprinted the holder with a smaller recess but roughing the inner walls of the recess with a knives solved the problem for me. 
Now the chip kind of clicks in.
The hole in one corner of the holder marks the chip orientation. It is aligned with the marking impression on the top side of the chip.

| Inserting Chip      | Chip Inserted  |
|------------|-------------|
| <img src="pics/IMAG2406.jpg" width="250">  | <img src="pics/IMAG2407.jpg" width="250">  | 

Four bolts guarantee the alignment of chip and PCB. I use broken drill/mill bits from my CNC. 
Magnets in the holder and on the backside of the PCB apply slight pressure to ensure a reliable contact.

<img src="pics/IMAG2408.jpg" width="350">

When the chip is in place the bootloader is flashed.

<img src="pics/IMAG2409.jpg" width="350">

Here is the flashed chip ready to be used in the next project! 

<img src="pics/IMAG2411.jpg" width="350">


