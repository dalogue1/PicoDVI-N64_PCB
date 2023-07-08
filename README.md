# PicoDVI-N64_PCB
Project creating a PCB to connect to the PicoDVI-N64 project.



The current status of the board I have made is as follows.  I have created and checked the board many times.  I have ordered it and will be testing it when it arrives. 

It includes everything I know in a board that can be ordered from jlcpcb for $2 for 5.  The remaining parts in the BOM from Mouser will be about $5 plus shipping.  

The features include: 

    fits within the N64 without cutting using the 3-d printed adapter
    
    usb port works without disconnecting power from the N64. (useful for software updates)
    
    works with the full or part flex cables from the n64adv2 open-source project
  
    works with a flex cable from HISPEEDIDO on Ali Express ( https://www.aliexpress.us/item/3256805571419579.html?spm=5261.ProductManageOnline.0.0.33212ddbdJ53Tz&gatewayAdapt=glo2usa4itemAdapt )
  
    passes PIF and Reset and hdmi CEC signals to gpio pins via in-line resistors
  
    passes 5V power to the HDMI port and pullup resistors to 5V are added for SCL and SDA
  
    all resistors and resistor networks are large enough for hand-soldering by DIYers
  
  
This is created in KiCad 6.0.11 and the project files are included.

![PicoDVI-N64_PCB-Front](https://github.com/dalogue1/PicoDVI-N64_PCB/assets/133064876/229bf70d-1fcd-4e96-a488-81059325d73f)

![PicoDVI-N64_PCB-Back](https://github.com/dalogue1/PicoDVI-N64_PCB/assets/133064876/9ae8b330-6932-4652-8f9d-c9026ffff4cd)

![N64_PCB_Fit](https://github.com/dalogue1/PicoDVI-N64_PCB/assets/133064876/a9b3f396-81b1-41a5-92eb-939396d21952)
