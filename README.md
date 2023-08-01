# PicoDVI-N64_PCB
Project to create a PCB to connect the [PicoDVI-N64](https://github.com/kbeckmann/PicoDVI-N64) project by Konrad Beckmann.



The current status of the board I have made is as follows.  I have created and checked the board many times.  I have ordered it and will be testing it when it arrives. I will post installation photos and instructions when possible.

It includes everything needed in a PCB that can be ordered from jlcpcb for $2 for five boards.  The remaining parts in the BOM from Mouser will be about $5 plus shipping.  The RPi Pico or Pico-W is a separate cost.  

## The features include: 

- Fits securely in the N64 using a no-cut 3D printed adapter from the [n64adv2_pcb](https://github.com/borti4938/n64adv2_pcb) open-source project by Peter Bartmann.  
- USB port works without disconnecting power from the N64. (useful for software updates)
- Works with the full or part flex cables from the n64adv2_pcb project
- Works with a $12 flex cable for N64Digital from [HISPEEDIDO](https://www.aliexpress.us/item/3256805571419579.html?spm=5261.ProductManageOnline.0.0.33212ddbdJ53Tz&gatewayAdapt=glo2usa4itemAdapt) on AliExpress.
- Both flex cable connections use FFC sockets  (Important note: the flex cable connectors need to have top contacts not bottom.)
- Connects PIF Control and Reset signals to gpio pins 20 and 21
  - directly for the n64adv2 flex cable
  - via 47 ohm in-line resistors for the HISPEEDIDO flex cable
- Connects the HDMI CEC signal to gpio pin 22 via a 0k resistor
- To connect HDMI, the PCB implements the equivalent of the [Pico-DVI-Sock](https://github.com/Wren6991/Pico-DVI-Sock) by Luke Wren.
- Passes 5V power to the HDMI port via a 0k resistor
- Adds 2.2k pull-up resistors to 5V for HDMI SCL and SDA signals
- All resistors and resistor networks are large enough for hand-soldering by DIYers

## Additional information: 

This project is created in KiCad 6.0.11 and the project files are included. The zip for the Gerber Files is provided as well.

After some initial testing, it appears as if the termination resistors on the part flex or on the HISPEEDIDO flex need to be replaced with 0 ohm resistors.  More investigation will be done to determine why because without the resistors the n64adv2 flex would be incompatible with the N64 RGB Mod.  Possibly 33 ohm resistor packs may work.  Further testing will be made to determine what are the best resistor packs to put on the flex cable.

Modifications have been made to the PCB to attempt to allow it to fit in varying N64 versions without cutting.  If anyone has difficulty with the PCB not fitting please let me know in the PicoDVI-N64 Discord chat or in a PM to @dalogue in Discord.

![PicoDVI-N64_PCB-Front](https://github.com/dalogue1/PicoDVI-N64_PCB/assets/133064876/febf28a8-e9df-4b44-a28a-578e1b2b2d29)

![PicoDVI-N64_PCB-Back](https://github.com/dalogue1/PicoDVI-N64_PCB/assets/133064876/be7cd166-1c3c-4c83-8c34-6b221039ceb5)

Test fit of an early version of the board.  The new version of the board has much smaller overlap to work with other versions of the N64 motherboard with wider screw mounts.  Also, the flex cable needed additional space.  The board should be connected to the case with a piece of the 3M double stick tape. (same method used by the HISPEEDIDO adapter)

![N64_PCB_Fit](https://github.com/dalogue1/PicoDVI-N64_PCB/assets/133064876/a9b3f396-81b1-41a5-92eb-939396d21952)
