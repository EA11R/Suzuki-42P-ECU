## Details about my Daughtercard for the F6AT ecu (K1)

<img width="740" alt="Screen Shot 1444-07-10 at 12 42 44 PM" src="https://user-images.githubusercontent.com/82368250/216007766-0e2ea58b-51f4-4361-a6ea-929bace56371.png">

Since the simplcity of the stock ecu Throttle switch I've decided to link it using a 5v signal from the actual ecu pinout so only WOT would effect the signal however if you wish to cancel this and add a virable nissan TPS you could unsolder the JP2 and connect it to the TPS pin shown within this photo
this should allow the tps to be utilized to be used for accel enrichment 


the map sensor can be connected via ADC chip but the better choice is to use the internal map sensor to control fueling in the system

#R504 can be connected to IG1 (**H1** on the board) to control the Ignition Advance however deleting the fuel cut is what is needed to add more boost 


there's extra circuit that could be built under the MPU to add a third injection channel to fully sequentially control the fuel on the engine 
so it becomes a single injection channel for each injector instead of the paired wire #20 on the oem harness 

-------------- **FEATURES** -------------------

1- On Board boost control ( requires a external solenoid) 
Ran via PWM signal 
2- Wideband support over the same wire (OX signal) 
3- Third Injection Channel 
4- Usage of full range TPS for accel enrichment 
5- External tach RPM wire (12v)

------------------------------------------------
**Third Injection channel**
A Twin wire harness can be wired straight from the board to the injector #3 
This modification will convert the injection system to fully sequential 
------------------------------------------------
** Ignition Advance control **
However it's very limted and not actually that useful but it's still possible 
I strongly advise just sticking to moving the distrubutor to adjust the timing or
buying viarable cam wheels however adjusting small increments on higher boost could be done
over computer 
