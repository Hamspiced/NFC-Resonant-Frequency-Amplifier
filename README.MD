# Project Repository for the Resonant Repeater Project [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

#New Website Launch

All of my designs are now available at the new MidwestGadgets.org website!!

# Support
If you are interested in my projects and would like to support me or buy me a coffee: http://paypal.me/hamspiced

For Licensing, Bulk or Custom orders feel free to contact me at: Hamspiced@gmail.com

For a video review by Deviant Ollam: https://youtu.be/64x2NtmRFpE?si=17tjNadDkAVzWNMu


<details open>
<summary>Avaible For Purchase</summary>

|         Version         |                                                    Product Link                                                       |                  Gerber Files                    |                  Amazon Link                    |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------ | ------------------------------------------------ |
| V1 DIY Antenna Adapter  | [Tindie V1 DIY Antenna Adapter](https://www.tindie.com/products/hamspiced/rfid-antenna-adapter-for-tuning-antennas/)  | [V1 Gerber](https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Gerber%20Files/V1AntennaAdapter.zip)    | ------------------------------------------------ |
| V1 Repeater             | [Tindie V1 Repeater](https://www.tindie.com/products/hamspiced/rfid-antenna-adapter-for-tuning-antennas/)             |     | ------------------------------------------------ |
| V2.1L Repeater PCB       | [Tindie V2.1 Repeater PCB](https://www.tindie.com/products/hamspiced/1356mhz-nfc-amplifier-v2/)                       | [V2.1 Gerber](https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Gerber%20Files/V2-1Repeater.zip)  | [Amazon US V3L Repeater](https://www.amazon.com/dp/B0D8WMCYDH) |
| V2.1s Small Repeater    | [Tindie V2.1s Small Repeater](https://www.tindie.com/products/hamspiced/1356mhz-nfc-amplifierrepeater-small-v21s/)    | [V2.1s Gerber](https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Gerber%20Files/V2-1SRepeater.zip) | ------------------------------------------------ |
| V3 Flex Repeater    | [Tindie V3 Flex Repeater](https://www.tindie.com/products/hamspiced/flex-nfc-repeaters-1356mhz-range-extenders/)    | Not Released to Creative Commons | ------------------------------------------------ |
| Field Detectors    | [Tindie V2.1 Field Detector](https://www.tindie.com/products/hamspiced/1356mhz-field-detectersrepeater-locator/)    | [V2.1s Gerber](https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Gerber%20Files/V2-1SRepeater.zip) Replaced 100pf Capacitor with smd 0603 LED | ------------------------------------------------ |

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

The debate is over.  I updated the design and identified an issue.  Since this repeater uses a 100pf capacitor choosing capacitors with a +/-10% tolerence isnt feasable.  When building ensure you are using a +/- 1%-5% capacitor to ensure it works properly.

Gerbers for this design are now available here

[V2.1s Gerber](https://github.com/Hamspiced/NFC-Resonant-Frequency-Amplifier/blob/main/Gerber%20Files/V2-1SRepeater.zip)

and Available for purchase here

[Tindie V2.1S Repeater PCB](https://www.tindie.com/products/hamspiced/1356mhz-nfc-amplifierrepeater-small-v21s/) [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

# V3.01 PCB Integrated Antenna with Integrated capacitance on Flex

Design is going to begin testing on an integrated capacitance circuit using flex.  With the help of Satur9 i hope we can take his knowledge of integrated capacitance using copper plate layers and apply it to our project.  Flex runs in testing are going to be expensive.  I hope to reduce the number of prototype runs by incorporating "trial by error sheet runs"

Flex pcbs are charged based on the foot print used when cutting them in sheets. By utilizing a singular large sheet i can create 10-20 different designs within an uncut sheet to see how they test.  My idea is to take what i learn from Satur9 make 2-3 panels with the design repeated on an uncut panel with slight variations in the capacitence layers to find one that ideally works.

There are multiple levels of variation and theory involved with Satur9's capacitence design.  One of which that takes the resonant flux that is generated by the capacitence, transfers it to the edge of the pcb and allows the coil to take that flux and increase its ability to operate at a more efficient level.  a 45 minute discussion with an expert in this field humbled me in knowing how little i know still.

Updates will be forthcoming as i take on this next step.


# Flex Prototypes

I received the first run of prototypes and was incredibly suprised by my math and how far it was off.  I took the documentation provided by a trusted expert in the field, Satur9, and layered the antenna from the V2.1s on the top and bottom layers of the flex pcb.  So basically i cut the coil in half and through vias layered it over itself.

In Satur9's design he incorporated a really aesthetically pleasing hump that helps to better make the transition to the next coil wind.  However i just cannot seem to replicate this due to my likely poor understanding of kicad software.  Its okay though, i am happy with the spiral design and will just overlap it.  I also think it may work out in my favor because i worry that the traces directly overlapping one another may cause some unknown capacetence within the antenna.  His design uses 3 winds at an unknown trace width and distance from one another.  My design is slightly different at 4 winds on each layer.

As far as getting the math correct and zeroing in on the correct capacetive plate size.  I used the documentation that Satur9 put together.

C = ε0 * εr * (A/d)
ε0 (vacuum permittivity) = 8.8541878128⋅10−12 F/m
εr (relative permittivity): relative permittivity polyimide = 3.4
A (area of plates): ?
d (distance between plates): 
0.025mm for 0.26mm FPC thickness
0.012mm for 0.1mm FPC thickness


So, for a capacitance of 100 pF, the area of the plates would be approximately 8.934mm^2 for an FPC thickness of 0.26 mm and approximately 2.968mm^2 for an FPC thickness of 0.1 mm.  So, for an FPC thickness of 0.26 mm, the radius would need to be approximately 0.1181 inches, and for an FPC thickness of 0.1 mm, the radius would need to be approximately 0.0763 inches to achieve the specified areas.  Since i was using an FPC thickness of .1mm i went with .0763 capacitive plate radius as my middle point.  

I designed a 200x100mm test flex panel With different plate sizes with .0763 as the base radius for the capacitive plates.  I didnt know how much capacetence would be introduced by increasing or decreasing the area.  so i made .0763 as a focal point.  

Each row would correspond to a different set variance that i would have in incrementally increaseing or decreasing the capacetive Plate Area.

Row 1 would increase by .0020mm
Row 2 and 3 would increase by .0050
Row 4 would increase by 10.

I sent this design off to the fab house and then second guessed everything.  I got in my own head that it is unlikely an area this small would effectively create the resistance i need.  So i assumed my calculations were off.  I re-made the same array but disregarded the math.  I created the plates at decreasing intervals from .2524 to .1369 and my thought was, i likely wont get what i need from the first revision.  But i can take the measured data from both, and estimate the needed area if it can graph out parabolically.

And this is what worked.

Below are my readings.

| Radius       | Frequency |
|--------------|-----------|
| 0.2524       | 8.3       |
| 0.2485111111 | 8.2       |
| 0.2446222222 | 8.1       |
| 0.2407333333 | 8.2       |
| 0.2368444444 | 8.3       |
| 0.2329555556 | 8.2       |
| 0.2290666667 | 8.2       |
| 0.2251777778 | 8.3       |
| 0.2212888889 | 8.3       |
| 0.2174       | 8.4       |
| 0.2135111111 | 8.4       |
| 0.2096222222 | 8.4       |
| 0.2057333333 | 8.6       |
| 0.2028       | 8.6       |
| 0.2018444444 | 8.6       |
| 0.1989111111 | 8.6       |
| 0.1950222222 | 8.65      |
| 0.1911333333 | 8.8       |
| 0.1872444444 | 8.9       |
| 0.1833555556 | 8.9       |
| 0.1794666667 | 9         |
| 0.1755777778 | 9.1       |
| 0.1716888889 | 9.2       |
| 0.1678       | 9.4       |
| 0.1639111111 | 9.4       |
| 0.1600222222 | 9.5       |
| 0.1561333333 | 9.7       |
| 0.1522444444 | 9.9       |
| 0.1483555556 | 9.9       |
| 0.1444666667 | 9.9       |
| 0.1405777778 | 10.1      |
| 0.1366888889 | 10.2      |
| 0.1328       | 10.4      |
| 0.1172444444 | 11        |
| 0.105        | 11.6      |
| 0.1          | 11.8      |
| 0.0762       | 13.4      |
| 0.0712       | 13.68     |
| 0.0692       | 13.72     |
| 0.0682       | 13.74     |
| 0.0672       | 13.76     |
| 0.0662       | 13.84     |
| 0.0652       | 13.92     |
| 0.0642       | 14.04     |
| 0.0632       | 14.16     |
| 0.0622       | 14.34     |
| 0.0612       | 14.52     |

Using this data i was able to create an additional test board zeroing in on around the .0712 radius.

5/24/2024
The test board came back and i found Exact tuning at specifically 0.0716in radius capacitive plates.  This design is going forward to fabrication and i will report back the findings.

8/13/2024
The first run of Flex V3 repeaters were a huge success.  After careful thought i am going to hold on to this design for a little while.  I would like to see what others can do in this same space and i feel that if i release the files for these repeaters that creativity will end here with this finished product.  For the capacitive plate design i have opened the doors i believe for a lot of other applications and i would like to see more NFC antenna designs using what i have documented here.  If anyone has any questions on this design please dont hesitate to reach out.  

I have created a tester board with different capacitive plate dimensions to cover a variety of capacetences.  If you are developing a project that can use this please feel free to reach out to me.

I have released production units of my flex design to tindie, as well as created Field detectors using the 2.1S design (You replace the 100pf capacitor with any smd 0603 LED).  Those are also on tindie.  I have also redesigned the 2.1L to a V3L using the capacitive plate design and it is also available on both Tindie as well as Amazon with the links above.


[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

