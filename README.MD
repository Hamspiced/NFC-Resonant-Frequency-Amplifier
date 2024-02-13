Project Repository for the Resonant Repeater Project

Goal:
Create a low-cost adaptable device that can amplify 13.56Mhz frequencies for low power devices, implants, etc.  
Initial idea is to take already made tuned NFC Chips from Keyfobs, harvest the antenna from them, find out the resonant capacetence, introduce a capacitor and tune as needed.


Proof of concept.

Magnet Wire coil with a capacitor to test.
Using online calculators i determined my .5mm magnet wire wrapped 5 times at 50mm width should be resonant at 13.56mhz.

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/v0-1%20antenna%20test.jpg" width="400">

Tuning was successfull
<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/V0%20Antenna%20Tuning.jpg" width="400">


V1.0 Antenna Adapter PCB
For the next step i wanted to take an already known Antenna design from a Keyfob that i knew operated at 13.56Mhz and make it easy to solder and add smd resistors.  Since the 0603 package is difficult to hand solder using a Hotplate to solder these components should save time and make it simple.  The initial PCB design should be relatively compact enough to fit in the Antenna void to keep thickness as low as possible.  Also printing on Flex PCB should make for super thin applications.

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/FR4%20Adapter.jpg" width="400">
<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/Flex%20Adapter.jpg" width="400">

Next was to add the antenna from a working NFC fob.  

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/Raw%20NFC%20Chip.jpg" width="400">

The only issue was these are not tuned properly

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/Raw%20NFC%20Chip%20Tuning.jpg" width="400">


I soldered a 22pf Capacitor to the Tuning adapter, soldered one lead to the adapter and slowly unwound the copper from the antenna until tuning was exactly at 13.56Mhz and ended up with a completed V1 of the resonant repeater.
<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/Soldered%20Antenna%20to%20adapter.jpg" width="400">


