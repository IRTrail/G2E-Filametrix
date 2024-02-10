# G2E and Filametrix
## _Modifications for the G2E to have a Filametrix cutter...and a filament sensor option...or two._  
#### Thanks to sundee, jmaurin, jelliebean, gsx8829, CheeseFrog, and kinematicdigit for suggestions and feedback. Thanks to any of you who have come here and print these parts. You're what it's all about.  
I am on discord @ Silverback_Attack#1187  
Understand there is no CAD released for the G2 stuff. Reverse engineering it is a total PITA. Ergo, there will likely be some slicer complaints because the stls aren't "watertight". I have done my best. If you want the reverse engineered files I used to start these mods, they're in the aptly named folder. They are not perfect clones because of some intricacies in the CAD process that are difficult to overcome. But they're likely indistinguishable when printed.  
#### Use at your own risk. It's not my fault your sister is ugly or your tongue hurts when you lick a 9V battery...or anything else. Just saying.  

### Non-sensor Config:  
![Filametrix for G2E - Baseline](https://github.com/IRTrail/Voron-Stuff/assets/53546870/971e3992-9a19-41cd-ba88-7a4262078c5e)   
![Filametrix for G2E - Baseline_2](https://github.com/IRTrail/Voron-Stuff/assets/53546870/f2b1baad-611c-4490-8393-d75df3c98c23)  

### Single Sensor Config:  
![Filametrix for G2E - Single Sensor](https://github.com/IRTrail/Voron-Stuff/assets/53546870/d396f91a-6356-4e1e-9b5f-fdacacf5937b)  

### Twin Sensor (Twinsor) Config:  
![Filametrix for G2E - Twinsor - Hex](https://github.com/IRTrail/Voron-Stuff/assets/53546870/72df904c-5bd1-4afa-8aa7-244e5654a124)  

### _All Licenses are carried over from their respective creators. Read them here:_
https://github.com/sorted01/Filametrix  
https://github.com/JaredC01/Galileo2  
If not otherwise licensed, the files herein are covered by GPL V3. See LICENSE in this directory.  
## Ok, so what do I need to print?  
You'll need to print:  
- One front of the G2E extruder body. No sensor, single sensor, or Twinsor. (See below)
- One G2E extruder rear body. This is the same between all versions.
- One arm of either version (See below)
	- The Stylized arm works with the printheads here.
	- The "wide" arm works with the original Filametrix printheads. It also works with the printheads here, but for either, you'll need a screw in the ADXL mount hole, just like the original Filametrix setup.
- A front and back of your desired print head.
	- The rear is often the same between versions of the same hotend. I.E. The Rapido V1 rear will work for the Standart Rapido V1 and the Rapido V1 UHF.
- The remaining parts from the main G2E repository linked above.
- The remaining parts from Filametrix linked above (blade holder etc.)  
## Great, what else do I need?
Well, pretty much what is in the parent repos linked above.
- The G2E extruder bodies use all the same hardware as the original and the only change was to carve out some material for the arm and switches, and modify the filament path a bit so the switches actuate more reliably. Thus, it uses the same hardware.
- The Filametrix printheads I have adapted in this repository have a socket head screw instead of a countersink screw at the pivot. Not a big deal, and if you want to modify yours for the countersink, have at it. I just have way more socket head screws laying around than countersink.
- You'll need two D2F microswitches. I've been just taking the lever off and it seems to work well. I didn't design for the lever, so if you use it, that's your choice and let me know how it goes. I bought a pack of 30 from Amazon. (Affiliate link to the ones I bought: https://amzn.to/3wfdvVp)
- You'll need two 5.5mm ball bearings. (Affiliate link to the ones I bought: https://amzn.to/4bB7HpA)
## The more boring stuff, but still important...kinda.
#### There are now three versions. One is non-sensored, one has a single sensor, the other has two sensors. See the respective folders for CAD, 3MF, and STL files.
- Unless otherwise stated below, all the build notes from the G2E and Filametrix apply. If you look things over, you should get the idea.
#### There are two arm versions.  
- One is a wide version which uses the screw in the ADXL hole for a stop.  
The other is a stylized arm which has an integral stop which does not use the screw. However, it does obscure the ADXL hole somewhat.  
- I have been told it is a PITA to install with the spring and washers and all without the screw stop. (I didn't know there were supposed to be washers!)
- The easiest way I have found is with the front and back separated. You put the screw through the pivot point, then add a washer. Then the spring goes in the arm and you simultaneously slide the arm on the screw while guiding the other end of the spring into the recess. Then place the second washer on the screw. Now you can mate the front and back parts of the printhead fairly easily.

#### These are measurements for the Rapido 1 with the Twinsor.  
Other versions use the same measurements, I.E. the Single Sensor has the same measurement, just not the other switch. Other hotends will vary with the length of the hotend.  
These are taken from CAD and are just calculations for reference. I am not sure what nozzle you use, so just measure it with the stinger of your calipers and add that to these values where asked in the Happy-Hare software. 
![Rapido Twinsor Lengths](https://github.com/IRTrail/Voron-Stuff/assets/53546870/a821cf6b-4c67-44a2-a548-0bc05bf0c026)
### NOTES:  
I have included all the necessary parts in each folder...I think. Please let me know of you find something missing.  
They should be oriented to print with no issues.  
- If you don't see something, or it's oriented incorrectly, please let me know. This project kinda blew up in a hurry and I did my best.  

The necessary supports are included, and should be discarded after printing.  
The standard Voron print settings should work quite well here.  
Some other print heads are available, and I am working through the others as I get requests for them. They're located in "Other Printheads".  
-- If you see something amiss in there, please let me know.
