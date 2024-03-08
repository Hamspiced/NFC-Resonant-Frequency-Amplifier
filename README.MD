# Project Repository for the Resonant Repeater Project




<details open>
<summary>Avaible For Purchase</summary>

|         Version         |                                                    Product Link                                                       |                  Gerber Files                    |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------ |
| V1 DIY Antenna Adapter  | [Tindie V1 DIY Antenna Adapter](https://www.tindie.com/products/hamspiced/rfid-antenna-adapter-for-tuning-antennas/)  | [V1 Gerber](https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Gerber%20Files/V1AntennaAdapter.zip)    |
| V1 Repeater             | [Tindie V1 Repeater](https://www.tindie.com/products/hamspiced/rfid-antenna-adapter-for-tuning-antennas/)             |     |
| V2.1 Repeater PCB       | [Tindie V2.1 Repeater PCB](https://www.tindie.com/products/hamspiced/1356mhz-nfc-amplifier-v2/)                       | [V2.1 Gerber](https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Gerber%20Files/V2-1Repeater.zip)  |
| V2.1s Small Repeater    | [Tindie V2.1s Small Repeater](https://www.tindie.com/products/hamspiced/rfid-antenna-adapter-for-tuning-antennas/)    | [V2.1s Gerber](https://www.github.com/hamspiced) |

</details>

# Goal
Create a low-cost adaptable device that can amplify 13.56Mhz frequencies for low power devices, implants, etc.  
Initial idea is to take already made tuned NFC Chips from Keyfobs, harvest the antenna from them, find out the resonant capacetence, introduce a capacitor and tune as needed.


# Proof of Concept

Magnet Wire coil with a capacitor to test.
Using online calculators i determined my .5mm magnet wire wrapped 5 times at 50mm width should be resonant at 13.56mhz.

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/v0-1%20antenna%20test.jpg" width="400">

Tuning was successfull

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/V0%20Antenna%20Tuning.jpg" width="400">


# V1.0 Antenna Adapter PCB
---
For the next step i wanted to take an already known Antenna design from a Keyfob that i knew operated at 13.56Mhz and make it easy to solder and add smd resistors.  Since the 0603 package is difficult to hand solder using a Hotplate to solder these components should save time and make it simple.  The initial PCB design should be relatively compact enough to fit in the Antenna void to keep thickness as low as possible.  Also printing on Flex PCB should make for super thin applications.

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/FR4%20Adapter.jpg" width="400"> <img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/%20Flex%20Adapter.jpg" width="400">

Next was to add the antenna from a working NFC fob.  

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/Raw%20NFC%20Chip.jpg" width="400">

The only issue was these are not tuned properly

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/Raw%20NFC%20Chip%20Tuning.jpg" width="400">


I soldered a 22pf Capacitor to the Tuning adapter, soldered one lead to the adapter and slowly unwound the copper from the antenna until tuning was exactly at 13.56Mhz and ended up with a completed V1 of the resonant repeater.

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/Soldered%20Antenna%20to%20adapter.jpg" width="400">

V1 Antenna Adapters for DIY are now available on my Tindie Store:
[Tindie V1 Antenna Adapter](https://www.tindie.com/products/hamspiced/rfid-antenna-adapter-for-tuning-antennas/) [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]


V1 Repeaters are now available on my Tindie Store:
[Tindie V1 Repeater](https://www.tindie.com/products/hamspiced/1356mhz-nfc-amplifier/)


Moving on to V2.0

The idea is to incorporate the designs into a printed PCB.  Using the traces as an antenna.

Overall design is almost complete.  awaiting prototypes for testing.



<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/V2prototype.png" width="400">


# V2.0/V2.1 PCB Integrated Antenna 
---
First Designs came back.  

I made a blunder in my first setup and had these assembled with a 22pf cap.  This was incorrect and tuning was better with a 30pf capacitor.  This got tuning in the same area.  I immediately ordered another batch in 30pf and will re-version this as V2.1

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/V2-1front.jpg" width="400">

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/V2-1back.jpg" width="400">

Testing with the proper capacitor yielded excellent results

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/V2-1test.jpg" width="400">


With this run of larger FR4 components reaching a satisfactory level i will start offering these on my Tindie store:

[Tindie V2.1 Repeater PCB](https://www.tindie.com/products/hamspiced/1356mhz-nfc-amplifier-v2/) [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]


# V2.1s PCB Integrated Antenna with Smaller Footprint
---
>Versioning will append an S to indicate smaller footprint but overall same design

With the success of the overall design at satisfactory levels we need to look at the possibility of a smaller circuit design.  Although the current state it works great the overall size is an issue for most applications.  Taking what we know of RFID circuits most nfc tags are about 1 inch in diameter.  So i wanted to redesign our board to fit within those confines.  

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/V2-1sprototype.jpg" width="400">

I checked my math and did a quick run condensing the turns of the circuit and using a 100pf capacitor.

<img src="https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Images/V2-1stest.jpg" width="400">

I dont think i could be more impressed.  Prototype was a success out of the gate.

Debating putting this footprint up on tindie.

# V3.01 PCB Integrated Antenna with Integrated capacitance on Flex

Design is going to begin testing on an integrated capacitance circuit using flex.  With the help of Satur9 i hope we can take his knowledge of integrated capacitance using copper plate layers and apply it to our project.  Flex runs in testing are going to be expensive.  I hope to reduce the number of prototype runs by incorporating "trial by error sheet runs"

Flex pcbs are charged based on the foot print used when cutting them in sheets. By utilizing a singular large sheet i can create 10-20 different designs within an uncut sheet to see how they test.  My idea is to take what i learn from Satur9 make 2-3 panels with the design repeated on an uncut panel with slight variations in the capacitence layers to find one that ideally works.

There are multiple levels of variation and theory involved with Satur9's capacitence design.  One of which that takes the resonant flux that is generated by the capacitence, transfers it to the edge of the pcb and allows the coil to take that flux and increase its ability to operate at a more efficient level.  a 45 minute discussion with an expert in this field humbled me in knowing how little i know still.

Updates will be forthcoming as i take on this next step.



[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

