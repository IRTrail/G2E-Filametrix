
# G2E and Filametrix
## _Modifications for the G2E to have a Filametrix cutter and toolhead sensors._  
#### Thanks to sundee, jmaurin, jelliebean, gsx8829, CheeseFrog, and kinematicdigit for suggestions and feedback. Thanks to any of you who have come here and print these parts. You're what it's all about.  
#### Special thanks to JaredC01 and Sorted for their amazing designs.
I am on discord @ Silverback_Attack
This version is based on the released CAD from JaredC01. For any parts not included here, you'll need to go to that repository.  

I have depreciated the single and non-sensor versions since I have not heard of anyone using them. If you want them, the versions previously here and based on beta CAD are in the `Depreciated` branch of this repo. I have no plans to continue supporting the other versions.  

Also, because I want to be transparent with you my esteemed colleagues, I have an affiliate status with Amazon, and get a tiny kickback if you click and buy on the links. I'll only suggest stuff I have used and had success with though.  

#### Use at your own risk. It's not my fault your sister is ugly or your tongue hurts when you lick a 9V battery...or anything else. Just saying.  
<h1>The G2E-Filametrix "Twinsor" (Dual Sensor)</h1>

<p align="center">
	<img src="https://github.com/IRTrail/Voron-Stuff/assets/53546870/72df904c-5bd1-4afa-8aa7-244e5654a124" alt="Twinsor" width="354" height="722" />
</p>

### _All Licenses are carried over from their respective creators. Read them here:_
https://github.com/sorted01/Filametrix  
https://github.com/JaredC01/Galileo2  
If not otherwise licensed, the files herein are covered by GPL V3. See LICENSE in this directory.  
## Ok, so what do I need to print?  
You'll need to print:
---
[KinematicDigit's calibration cube](https://www.printables.com/model/570510-swiss-cheese-calibration-cube)  
Print this ***FIRST!*** If you can't make this work, tune your printer. Most of the issues with switch activation can be solved with a finely tuned printer. Unfortunately, there's no real good way to get around the 0.5mm activation range of the D2F switch. ***Your prints must be on point!***  
Furthermore, if you ask me why your switches don't work correctly, I'll likely ask to see some detailed photos of this cube and the ERCF calibration print.
---  
 - [ ] One front of the G2E extruder body.
 - [ ] One G2E extruder rear body. This is the same between all versions.
 - [ ] One arm of either version (See below)
	- The Stylized arm works with the printheads here.
	- The "wide" arm works with the original Filametrix printheads. It also works with the printheads here, but for either, you'll need a screw in the ADXL mount hole, just like the original Filametrix setup.
 - [ ] A front and back of your desired print head.
	- The rear is often the same between versions of the same hotend. I.E. The Rapido V1 rear will work for the Standard Rapido V1 and the Rapido V1 UHF.
 - [ ] The remaining parts from the main G2E repository linked above.
 - [ ] The remaining parts from Filametrix linked above (blade holder etc.)  
## Great, what else do I need?
Well, pretty much what is in the parent repos linked above.
- The G2E extruder bodies use all the same hardware as the original and the only change was to carve out some material for the arm and switches, and modify the filament path a bit so the switches actuate more reliably. Thus, it uses the same hardware.
- The Filametrix printheads I have adapted in this repository have a socket head screw instead of a countersink screw at the pivot. Not a big deal, and if you want to modify yours for the countersink, have at it. I just have way more socket head screws laying around than countersink.
- You'll need two D2F microswitches. I've been just taking the lever off and it seems to work well. I didn't design for the lever, so if you use it, that's your choice and let me know how it goes. I bought a pack of 30 from Amazon. (Affiliate link to the [ones I bought](https://amzn.to/3wfdvVp))
- You'll need two 5.5mm ball bearings. (Affiliate link to [the ones I bought](https://amzn.to/4bB7HpA) or [these work as well](https://amzn.to/3Vf1sli))  
## Right on. But, I'm a true badass and mangled the depressor. Got anything for me?
You bet'cha. Check out the `Beefy Depressor` folder. It should mount in the same location as the standard one, but hey, you don't know your own strength, so use washers on every M3 x 10 Socket head screw. It's important. Don't be like this guy:  
<p align="center">
	<img src="https://github.com/IRTrail/G2E-Filametrix/blob/main/Beefy%20Depressor/images/broken.jpg?raw=true" alt="busted depressor" width="400" height="301" />
</p>  
## The more boring stuff, but still important...kinda.
- Unless otherwise stated below, all the build notes from the G2E and Filametrix apply. If you look things over, you should get the idea.
#### There are two arm versions.  
- One is a wide version which uses the screw in the ADXL hole for a stop.  
The other is a stylized arm which has an integral stop which does not use the screw. However, it does obscure the ADXL hole somewhat.  
- I have been told it is a PITA to install with the spring and washers and all without the screw stop. (I didn't know there were supposed to be washers!)
- The easiest way I have found is with the front and back separated. You put the screw through the pivot point, then add a washer. Then the spring goes in the arm and you simultaneously slide the arm on the screw while guiding the other end of the spring into the recess. Then place the second washer on the screw. Now you can mate the front and back parts of the printhead fairly easily.

## Extruder and Hotend Measurements
These are taken from CAD and are just calculations for reference. I am not sure what nozzle you use, so just measure it with the stinger of your calipers and add that to these values where asked in the Happy-Hare software.
### Rapido 1:
<p align="center">
	<img src="https://github.com/IRTrail/G2E-Filametrix/assets/53546870/7c532d00-b54f-4a1f-99e9-4abc08bdaa8b" />
</p>
#### Here's what I have for the Rapido 2 standard flow hotend with the Twinsor. I have found them to be the same as the Rapido 1 standard flow.
- Note that these are taken from Happy Hare 2.5.0.
- Yours may be located in a different config file if you don't have the same version of Happy Hare.  
- Also, understand these are what work for me. You may have different values. But, hopefully these are a good starting point for you.  

From mmu_parameters.cfg:  
![mmu_parameters](https://github.com/IRTrail/G2E-Filametrix/assets/53546870/b694b0f2-8ff9-45dd-b704-69659f8a9ae5)
From mmu_macro_vars.cfg:   
![mmu_macro_vars](https://github.com/IRTrail/G2E-Filametrix/assets/53546870/60c23db7-0f1e-40f7-a741-d50ed480d1b3)

### Revo
<p align="center">
	<img src="https://github.com/IRTrail/G2E-Filametrix/assets/53546870/43c72d0e-b89d-4fb6-b7ae-fc93a39379fa" />
</p>  

<ins>_These are only measured from CAD and not tested._</ins>  

### Troubleshooting:
If your switches don't activate correctly:
- Go back and print the swiss cheese calibration block.
- Tune your printer using [Ellis' guide](https://ellis3dp.com/Print-Tuning-Guide/). Step through it one step at a time and DON'T SKIP ANY STEPS.
- Try a different switch. I have found that some of the Amazonium switches vary in their activation range. Chances are a different switch (even from the same box of 50 you bought) will work better. I bought [these (affilate link)](https://amzn.to/49HGtfB) and they are decent. I haven't had much issue with them, but most of the time, if a user's print is dialed in, a different switch will help.
### Input Shaper and Resonance Tuning
I have found that the balls tend to rattle around and make an extra hump in the frequency graph. So, because you've changed the mass of the toolhead and are going to redo input shaper (...right?) I would suggest just cutting off about a 15cm length of filament and pushing that throught the printhead to hold the balls steady, or just feed filament from the MMU down to the toolhead. Then run input shaper. That tends to make a more realistic graph since there will be filament in the printhead while printing.  
### A few words about the blade
I have found the #4 blades to be of poor to low quality through Amazon. [I got these](https://amzn.to/3PAReIw). The steel seems to be good, but the edge isn't honed well. I would suggest a few swipes across a sharpening stone to hone it to a keen edge.
### NOTES:  
I have included all the necessary parts in each folder...I think. Please let me know of you find something missing.  
They should be oriented to print with no issues.  
- If you don't see something, or it's oriented incorrectly, please let me know. This project kinda blew up in a hurry and I did my best.  

The necessary supports are included and should be discarded after printing.  
The standard Voron print settings should work quite well here.  
Some other print heads are available, and I am working through the others as I get requests for them. They're located in "Other Printheads".  
-- If you see something amiss in there, please let me know.
