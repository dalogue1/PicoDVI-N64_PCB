# PicoDVI-N64_PCB
Project to create a PCB to connect the [PicoDVI-N64](https://github.com/kbeckmann/PicoDVI-N64) project by Konrad Beckmann.



The current status of the board I have made is as follows.  I have created and checked the board many times.  I have ordered it and will be testing it when it arrives. I will post installation photos and instructions when possible.

It includes everything needed in a PCB that can be ordered from jlcpcb for $2 for five boards.  The remaining parts in the BOM from Mouser will be about $5 plus shipping.  The RPi Pico or Pico-W is a separate cost.  

## The features include: 

- Fits securely in the N64 using a no-cut 3D printed adapter from the [n64adv2_pcb](https://github.com/borti4938/n64adv2_pcb) open-source project by Peter Bartmann.  
- USB port works without disconnecting power from the N64. (useful for software updates)
- Works with the full or part flex cables from the n64adv2_pcb project
- Works with a $12 flex cable for N64Digital from [HISPEEDIDO](https://www.aliexpress.us/item/3256805571419579.html?spm=5261.ProductManageOnline.0.0.33212ddbdJ53Tz&gatewayAdapt=glo2usa4itemAdapt) on AliExpress.
- Both flex cable connections use FFC sockets
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

![image](https://github.com/dalogue1/PicoDVI-N64_PCB/assets/133064876/9315e3da-7bc9-433b-8e38-e10323c88f16)

![image](https://github.com/dalogue1/PicoDVI-N64_PCB/assets/133064876/763a6812-2a31-4b81-8f16-87e49d605c8b)

Test fit of an early version of the board

![N64_PCB_Fit](https://github.com/dalogue1/PicoDVI-N64_PCB/assets/133064876/a9b3f396-81b1-41a5-92eb-939396d21952)
