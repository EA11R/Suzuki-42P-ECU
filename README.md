# Suzuki-42P-ECU
The #1 source of Suzuki mask MPU information and resources 
 ## image of board 
 
 ![i-img1200x903-1666231880i3cpzc833943](https://user-images.githubusercontent.com/82368250/230820564-450ab1d6-fdd1-4f6e-8afe-afcb6894f376.jpg)

 
 
 the board utilzes a 8-bit cpu which is masked it's believed to be close 
 
 > the pinout has been previously figured out by (rhinopower) 
 www.rhinopower.org/ECUs/RomReader/Romreader.html
 
 ## pinout of the cpu 
  ![IMG_0691_result](https://user-images.githubusercontent.com/82368250/230824265-55904e76-d08a-4f00-839f-5ac02835fae6.png)


## about [*IC101*]
the raw sensor input connects to IC101 before being converted to digital signals 
and sent to CPU on the Right side of the IC the raw inputs could be sniffed as a 0-5v
analog signal.


> this is a pinout of the ecu pulled over by a scope and some testing 
I took the neccesary pins of it to work and left over things such as temp sensors 
it can be pulled out of the ecu but I honestly can't tell how to turn that digital signal into numbers without further testing
the IC before it however has a gradiant signal of voltage via the variant resistance of the temp thermos 
I have took the neccesary pins to hook the ECU alongsite a daughter card that uses speeduino 

## Currently Known PNPs
https://www.keisport.us/pnp/
## Current Daugtercards on sale
   MTR40BB : https://buyee.jp/item/yahoo/auction/u1052820291
   
   QSF313_F6A : https://github.com/EA11R/Suzuki-42P-ECU/tree/main/QSF_ADD_ON_BOARD

## Possible piggy-back ECU's
- E-manage (TRUST)

- HKS F-con (ALL)

- Speeduino ( can be standalone with some changes)

- any ECU that can get a squarewave signal and a choice of cylinders.
Current ("Free of charge") project

- an open source ECU adapter for speeduino boards & harness how to and links to purchace parts 

- Adapter PCBS for popular ecus with an added pip373 slot for distrubtor ignition!

- Modren Daughtercard using oem CPU + speeduino (atmega 2560) , for better ignition timing , full fuel control

> Prepare for Piggyback install : 
![IMG_8498](https://user-images.githubusercontent.com/82368250/230824334-06d7a9eb-bb7e-4e37-abc9-e3ff67b28280.jpg)

 
 - 1 Cut the resistor where I have the solder joint from the middle so you can Undo if you wish. 
     then pass the wires trough the case holes
  
 -  2 Solder the wire onto the remaining of the resistor leg. & lift it up to keep space * this will be your "out wire" from stock to aftermarket
 
  - 3 shrink tube the resistor is a good countermeasure just incase the resistor vibrates back into place , any insulator is fine.
 
 -  4 solder a IN wire in the remaining of the other side. ( connect the wire coming from aftermarket to your stock ecu)
  
  >  the rest of the information will be on each independant ecu catagory with it's own install guide.
  

## Repair 
- As far as repair goes within the suzuki ecu
if you manage to burn the cpu or the IC101 you need another suzuki ecu as a donor to fix that 
otherwise all other parts can be found off shelf 
the similar ICs are AD chips.

## My PNP Card Design 
converts the OEM stock ECU into a tuneable 
ECU and adds a Addtional injection channel 
to convert fueling into fully sequential

Features:

-Internal MAP option 

-wideband support 

-Ignition control (optional)

-Bluetooth 

-Data logging (bluetooth or usb)



![IMG_9346](https://user-images.githubusercontent.com/82368250/219488621-e23a3fb9-1fba-4b5f-b295-8bf397ed1a99.jpg)


## PDF Resources & Notes

| ECU | PDF/DIR  |
| ------ | ------ |
| QSF_F6A   |[Directory](QSF_ADD_ON_BOARD/readme.md)
| HKS F-CON IS Pinout |[Click Here](HKS_F_CONV_&_IS/F-conIS.jpg) |
| HKS F-CON IS Installion Notes |[Click Here](HKS_F_CONV_&_IS/installation%20notes.md) |
| E-Manage (TRUST) |[Directory](E-manage/) |
| MCU & EPPROM's   |[Directory](Datasheet/)
| MTR40BB   |[Directory](MTR40BB%20INFORMATION/)
| Speeduino   |[Directory](speeduino/)
| Distributor_wheel   |[Directory](Distributor_Modification/readme.md)
                


So lets see where this project goes and the documentation with it shall we 






**Qatif Speed Factory , Saleh.M**

