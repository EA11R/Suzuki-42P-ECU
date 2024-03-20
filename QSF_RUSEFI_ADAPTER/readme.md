## RUSEFI UAEFI BASED SUZUKI EMS 
as rusefi expanded into making better and better ecus over the years , they've released the affordable verison of their lineup and that is way over what the cappuccino needs to run since it's a 6x6 ecu
therefore many of the outputs can be reutilized for other things and I took advantage over the fact to create a true "ULTRA AFFORDABLE CAPPUCCINO ECU" without going low on features 


## For people with bare stock cars
just plug the ecu and turn the key it will function as is and perform superior to stock

## for nerds 
you can get the adapter from me and solder the ecu board from RUSEFI yourself 
I recently changed my pin size to arduino (0.8MM) on adapter side due to 1.14MM pins being difficult to source and expensive 
would increase cost by 60$



## IMAGE OF BOARD


<img width="892" alt="Screen Shot 1445-09-10 at 5 29 34 AM" src="https://github.com/EA11R/Suzuki-42P-ECU/assets/82368250/2b30bd2f-559f-4a84-b4cf-ca94abe880a2">


![IMG_3487](https://github.com/EA11R/Suzuki-42P-ECU/assets/82368250/7be59731-5070-45e2-8bfc-03a098b46155)





## COP HARNESS EXPLAINED 
<img width="442" alt="Screen Shot 1445-09-10 at 4 02 22 AM" src="https://github.com/EA11R/Suzuki-42P-ECU/assets/82368250/1bf7319e-855b-4e43-8ece-d20ddba9131a">

each number goes to it's co-responding cylinder don't be afraid to mismatch because it can be managed in software 
for GND of coils it should be grounded somewhere in the engine , anywhere you wish as long as it's a good ground 
for tach signal I suggest some aftermarket cop tach adapters 
such as this if you're running "smart coils without a external ignitor" https://www.ebay.com/itm/142171581596 and one such as this https://www.autosportlabs.com/product/tach-adapter/ 

**IGN 1 = CLY 1** 

**IGN 2 = CLY 2**

**IGN 3 = CLY 3**

**if you're running dumb coils with a external ignitor , you simply connect the coil side of ignitor and not the ecu signal side**

![image](https://github.com/EA11R/Suzuki-42P-ECU/assets/82368250/929edff9-692a-4145-8b73-b0f902adcc7a)

then connect "TACH" to your orignal brown wire (coil ground) , please use orignal IG power to power ur coil pack harness instead of direct ecu feed 
don't use 12V on ecu extra plug to feed it with power as I only use them for testing

<img width="673" alt="Screen Shot 1445-09-10 at 4 16 22 AM" src="https://github.com/EA11R/Suzuki-42P-ECU/assets/82368250/bf37807e-5c40-4d36-a933-ce3c2d94ad91">


**make sure to cut jumper made here , and remove solder from the SMD jumper , the THT jumper is there if you somehow manage to ruin the SMD jumper however it's nice
to have both closed when running stock coil to insure it's getting a good signal** 

orignal harness side coil plug 
https://www.aliexpress.com/item/1005002422920931.html
needed to make a COP plug , source whatever coils u want ur self , and take care of the bracket


## WARNING 

if you don't cut IGN jumper or remove IGN#1 wire from ecu plug this before install of coil packs you can risk damage to your tach or ecu while installing tachometer adapter 
tach adapters have voltage spikes up to 60V and I don't suggest back feeding it into your ignition transistor as it shouldn't share the signal with IGN#1 
anymore

## AUX 1 (one of 3 AUX WIRES across the board)
it's a gauge input bundled with the COP plug you can use that to put any analog gauge u wish into ur ecu
if ur running a stock setup and want to have a full digital cluster I suggest using it for fuel level!

## Ask for help you're not superman!
again if you don't have knowledge in wiring don't be afraid to ask me or consult your local wiring/ecu speicalists 
just hand him this information and they will certianly understand why and how!


## CAS HARNESS EXPLAINED 


<img width="870" alt="Screen Shot 1445-09-10 at 4 33 57 AM" src="https://github.com/EA11R/Suzuki-42P-ECU/assets/82368250/2a79e0a2-564f-485d-a87c-3f107f8a3b6f">

as simple as it gets wire each one into it's counterpart in the CAS sensor on ur daewoo distributor 


![IMG_3406](https://github.com/EA11R/Suzuki-42P-ECU/assets/82368250/c956d462-cd5b-4579-b756-250ce87fd72c)

## KNOCK SENSOR (IN CAS HARNESS BECAUSE IT'S CLOSE TO THE BOTTOM OF THE ENGINE)
for knock sensor check the diagram of whatever sensor ur using 

wire signal to KNOCK_IN

wire ground to GNDA 

## CAN BUS HARNESS 

<img width="779" alt="Screen Shot 1445-09-10 at 4 42 30 AM" src="https://github.com/EA11R/Suzuki-42P-ECU/assets/82368250/d20bf8ee-e605-4a4a-b164-6d5e169b3a8e">


CAN + , CAN - can be used to wire a external wideband such as AEM Series X , you can certianly use the onboard wideband if you don't want/need a gauge

BTN2 (ORIGNALLY USED FOR A/C) (can be reutilized for race cars) , BTN3,BTN1 can be used as a clutch switch or any kind of button to activate anything 

**BUTTONS (GROUND BASED SWITCH OR BUTTON ONLY)**

## E-Throttle + TPS information 
<img width="454" alt="Screen Shot 1445-09-10 at 4 57 29 AM" src="https://github.com/EA11R/Suzuki-42P-ECU/assets/82368250/7798119e-9dee-4af6-b402-721d7201eaff">

| PIN | FUNCTION |
| ------ | ------ |
| DC1 +  | Throttle motor + |
| DC1 - | Throttle motor -  |
| TPS1  | TPS SIGNAL|
| TPS2  | TPS SIGNAL(only E throttle uses two tps)|
| GNDA | I think ground O_0 but for sensor (use for tps) |
| 5V | I think FIVE VOLTS use for tps power |
| fun fact | TPS 5V being connected with any 12v wire will kill ur ecu |

| PIN | FUNCTION |
| ------ | ------ |
| PPS1  |Primary pedal output|
| PPS2 | secondary pedal output|


| EXTRA PIN | FUNCTION |
| ------ | ------ |
| LSW1  |LOW SIDE OUT (can used for fan relay)|
| BTN1 | BUTTON OR SWITCH INPUT (GROUND BASED ONLY) |


<img width="773" alt="Screen Shot 1445-09-10 at 5 16 13 AM" src="https://github.com/EA11R/Suzuki-42P-ECU/assets/82368250/0ee943a7-5879-44ff-b85e-510c02273fbb">

| EXTRA PIN | FUNCTION |
| ------ | ------ |
| IGN5 (TACH)  |TACHOMETER OR WHATEVER OUTPUT U WANT|
| AUX3 | ANALOG GAUGE INPUT (0-5V) |

**IF YOU EVER WANTED STEPPER IDLE**

| DC PIN | FUNCTION |
| ------ | ------ |
| DC2+  |STEPPER +|
| DC2- | STEPPER- |

## NEW ECU PINOUT AND EXTRAS 

<img width="189" alt="Screen Shot 1445-09-10 at 5 20 59 AM" src="https://github.com/EA11R/Suzuki-42P-ECU/assets/82368250/eea53de8-b5e6-4639-b523-63bf72b680fe">

the unused pins in the harness are now INJ3 (For sequential use) and FLEX (Flex fuel sensor) 
EL1 , EL2 are dropped from harness (unconnected) 
EGR No longer used (always off) 


## supported Triggers 

| TRIGGER | RECOMMENDED |
| ------ | ------ |
| EA11R STOCK 3 TOOTH |works but very low res (single coil only) |
| Daewoo Distributor | recommended for single coil and COPs|

## for nerds read: 


| Distributor_wheel |[Directory](https://github.com/EA11R/Suzuki-42P-ECU/blob/main/Distributor_Modification/readme.md)|
| ------ | ------ |





