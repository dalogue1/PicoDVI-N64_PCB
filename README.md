# PicoDVI-N64_PCB
Project to create a PCB to connect the PicoDVI-N64 project by Konrad Beckmann.



The current status of the board I have made is as follows.  I have created and checked the board many times.  I have ordered it and will be testing it when it arrives. 

It includes everything I know in a board that can be ordered from jlcpcb for $2 for 5.  The remaining parts in the BOM from Mouser will be about $5 plus shipping.  

The features include: 

    Fits within the N64 without cutting using a no-cut 3D printed adapter from the n64adv2 project
    
    USB port works without disconnecting power from the N64. (useful for software updates)
    
    Works with the full or part flex cables from the n64adv2 open-source project
  
    Works with a flex cable from HISPEEDIDO on AliExpress (link below).
  
    Connects PIF and Reset signals to gpio pins 20 and 21 directly for the n64adv2 flex cable
    
    Connects PIF and Reset signals to gpio pins 20 and 21 via 47 ohm in-line resistors for the HISPEEDIDO flex cable
    
    Connects HDMI CEC signal to gpio pin 22 via a 0k resistor
  
    Passes 5V power to the HDMI port via a 0k resistor

    Added 2.2k pull-up resistors to 5V are added for HDMI SCL and SDA signals
  
    All resistors and resistor networks are large enough for hand-soldering by DIYers

The HISPEEDIDO flex cable is available for $12 (free shipping) at  
https://www.aliexpress.us/item/3256805571419579.html?spm=5261.ProductManageOnline.0.0.33212ddbdJ53Tz&gatewayAdapt=glo2usa4itemAdapt 

  
This is created in KiCad 6.0.11 and the project files are included.

![PicoDVI-N64_PCB-Front](https://github.com/dalogue1/PicoDVI-N64_PCB/assets/133064876/229bf70d-1fcd-4e96-a488-81059325d73f)

![PicoDVI-N64_PCB-Back](https://github.com/dalogue1/PicoDVI-N64_PCB/assets/133064876/9ae8b330-6932-4652-8f9d-c9026ffff4cd)

![N64_PCB_Fit](https://github.com/dalogue1/PicoDVI-N64_PCB/assets/133064876/a9b3f396-81b1-41a5-92eb-939396d21952)
