Project Repository for the Resonant Repeater Project

Goal:
Create a low-cost adaptable device that can amplify 13.56Mhz frequencies for low power devices, implants, etc.  
Initial idea is to take already made tuned NFC Chips from Keyfobs, harvest the antenna from them, find out the resonant capacetence, introduce a capacitor and tune as needed.


Proof of concept.

Magnet Wire coil with a capacitor to test.
Using online calculators i determined my .5mm magnet wire wrapped 5 times at 50mm width should be resonant at 13.56mhz.

![V0.1](/Images/v0-1%20antenna%20test.jpg)

Tuning was successfull
![V0.1 Tuned](/Images/Raw%20NFC%20Chip%20Tuning.jpg)


V1.0 Antenna Adapter PCB
For the next step i wanted to take an already known Antenna design from a Keyfob that i knew operated at 13.56Mhz and make it easy to solder and add smd resistors.  Since the 0603 package is difficult to hand solder using a Hotplate to solder these components should save time and make it simple.  The initial PCB design should be relatively compact enough to fit in the Antenna void to keep thickness as low as possible.  Also printing on Flex PCB should make for super thin applications.

![FR4 Adapter](/Images/FR4%20Adapter.jpg) 
![Flex Adapter](https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/%20Flex%20Adapter.jpg?raw=true "Flex Adapter")
![Employees-Burnout-Analysis-and-Prediction](Images/%20Flex%20Adapter.jpg?raw=true)
