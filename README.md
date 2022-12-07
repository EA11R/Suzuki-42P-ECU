# Suzuki-42P-ECU
The #1 source of Suzuki mask MPU information and resources 
 ## image of board 
 ![alt text](https://gcdnb.pbrd.co/images/1ydCnrPaT7p2.jpg)
 
 
 
 the board utilzes a 8-bit cpu which is masked it's believed to be close 
 
 > the pinout has been previously figured out by (rhinopower) 
 www.rhinopower.org/ECUs/RomReader/Romreader.html
 
 ## pinout of the cpu 
  ![alt text](https://gcdnb.pbrd.co/images/Y1y29Iqc7OYW.jpg?o=1)

> this is a pinout of the ecu pulled over by a scope and some testing 
I took the neccesary pins of it to work and left over things such as temp sensors 
it can be pulled out of the ecu but I honestly can't tell how to turn that digital signal into numbers without further testing
the IC before it however has a gradiant signal of voltage via the variant resistance of the temp thermos 
I have took the neccesary pins to hook the ECU alongsite a daughter card that uses speeduino 

## Currently Known PNPs
https://www.keisport.us/pnp/
## Current Daugtercards on sale
   MTR40BB : https://buyee.jp/item/yahoo/auction/u1052820291
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

  ![alt text](https://gcdnb.pbrd.co/images/rOFZfakCF07A.jpg?o=1)
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

## PDF Resources & Notes

| ECU | PDF/DIR  |
| ------ | ------ |
| HKS F-CON IS Pinout |[Click Here](HKS_F_CONV + IS/F-conIS.jpg) |
| HKS F-CON IS Installion Notes |[Click Here](HKS_F_CONV + IS/installation%20notes.md) |
| E-Manage (TRUST) |[Directory](E-manage/) |
| MCU & EPPROM's   |[Directory](Datasheet/)

So lets see where this project goes and the documentation with it shall we 






**Qatif Speed Factory , Saleh.M**

