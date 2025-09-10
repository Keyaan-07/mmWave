# August 10 2025

Starting with the journaling of this project!

found an amazing guide for the IC(IWRL6432), here it us https://www.ti.com/tool/TIDEP-01033#design-products

It is amazing and i started with the schematic too, i have plans that i will order BGA from LCSC and assemble myself home, but let's see what happens. 

# august 20 2025

i am in school today and will start with the schematic  


did most of the schematic work today itself, and now i will do final changes and then start with PCB..  

it is gonna be great  
oh wait, here is an image:  
![main sch](/images/aug20/main.png)

oh wait, i just forgot that i would have to make the 1.8v voltage regulator :pf:

# August 22 2025

Gonna do a lot of work today, i will try to finish the 1.8v circuit, and start with the layout, i will route RF at the last because it is the hardest

umm i did some work today, it was idk what, mostly assigning stuff and trying to see what option would fit the best for me for reducing costs.

i have two options for making the PCB, 
- Either i can go for a single sided baord(not ideal for BGA
- I can do dual sided board(not ideal for costs as setup fee is 18 USD alone)

but a dual sided board is almost necessary as the components are BGA, and i would need decoupling caps all around it. 

so now basically i have to get 2 sided board made by myself, because i will only get JLCPCBA for 1 side, so i have kept all the back sided components(almost all are 0603) to handsolder pad size(that will be okay for me as i have handsoldered 0402😎). but i will still need to take care. 

![sch](/images/aug22/sch.png)  
only added this much of the circuit cuz i was finding the proper IC which is basic component in PCBA, and i was trying to understand it's circuit but i didn't understand it properly, will try tomorrow.  

This much PCB work is done:
![pcb](/images/aug22/pcb.png)  

i will try to complete schematic and placement by tomorrow...


### Time Spent today: about 1 hour

# august 23 2025
I am currently in school. gotta start working on the buck convertor, the 1.8v regulator

nvm, i am just changing the buck convertor to the tps62850 instead of the tps5430, because it has very low ripple output and it is recommeneded.

i changed my oscillator to [this](https://www.lcsc.com/product-detail/C5261245.html), and it required 10 pF locad cap so i will use the 15pFx2 capacitors, i already have them at my home.

### Time Spent today: about 25 mins

# august 24 2025

today, i am feeling very very happy as i figured out how i would mae the PCB for cheap as a 6 layer board and still have PCBA. i feel great thinking about it!

might route today..

didn't do any significant work today, just completed the 1.8v buck reg, and i still feel happy. will update with the photos tomorrow cuz too tired.  
Images:  
Buck Convertor:  
![buck convertor](/images/aug24/buck.png)  
efficient way and make PCBs cheaper:  
![BGA pads](/images/aug24/bga.png)  

### time spent today: 30 mins

# august 25 2025
i am in school today, uploaded the photos for yesterday, now i will find 2 inductors and assign footprints and finally start with final routing

started with the PCB layout, will update soon

just completed with the layout, almost, probably, antennas remaining ofcourse  

![layout](/images/aug25/layout.png)  

did this, done that, now time for the harder part, RF.

well i have no experience making microstrip patch antennas and their feedlines but why not try making them. i'll be starting now

i am done, i think my patch antenna is ready

so basically, there are two popular types of feed lines in a patch, inset feedline and quarter-wave transformer feedline.  

Inset Feedline:  
![inset feedline](https://www.antenna-theory.com/antennas/patches/patch4.jpg)  
Quarter-wave Transformer feedline:  
![q-wave transformer](https://www.antenna-theory.com/antennas/patches/patch5.jpg)

and um after mind-storming, i figured out that i would use inset feedline(it is simpler to make lol). and I made it too!  

Here is something i made:  
![my patch yayyy](/images/aug25/patch.png)

it operates at 60GHz so the dimensions are pretty small. L=1.15mm and W=1.51mm

i felt so happy when it turned out great

### time spent today: 2 hours 30 mins

# August 26 2025

I am in school, made the RX antenna part completely, the array consists of 3 antennas at lambda/2 length

![RX array](/images/aug26/RX_ant.png)

now, i have to make a custom ANT symbol.  
did just make it in 5 mins  


finally, i think all the antennas are ready, with all the final touches done too, and i removed the wires coming out of the antennas, because they were causing problems. here is the current look:  
### RX:  
![current RX antenna](/images/aug26/current_RX.png)  
### TX:  
![current TX antenna](/images/aug26/current_TX.png)

well well well, my layout is done, feel super good!  
![layout done](/images/aug26/layout_done.png)

### time spent today: 1 hour 10 mins

# August 28

Started with PCB layout in school.


I have made a decision to remove the JTAG pins, i think that those are unnecessary, because i am confident that i build great circuits, and thus there is no need for debugging(BPS Space reference). 

oh my god, my PCB is almost complete, just two Antenna connections remaining!

i guess the PCB is done, some final touches remaining:  
![pcb doneee](/images/aug28/pcb_done_prolly.png)
(i am at 64 vias rn let's see how many i add)
### Time Spent Today: 4 hours

# August 29 2025
today, idk how but i forgot to journal, and i have added so many damn vias, i am a crazy crazy person, they were like 64 yesterday, now they are like 200 something, all ground vias, atp i am just making jlc suffer, and i spent an hour trying my best to squeeze as many vias as i can :skull:

### Time spent today: 1 hour

# August 30 2025

i am done. THE PCB IS FINALLY READY  

![final PCB](/images/aug30/final_pcb.png)  
![final PCB](/images/aug30/final_pcb_poured.png)  
![3d render image 1](/images/aug30/3d1.png)
![3d render image 2](/images/aug30/3d2.png)
### time spent today: 20 mins  

# August 31 2025
grounded ends today, and i have to submit this proj, so i am gonna do that today itself!

# sept 6 2025
Grounded ends 20 sept!! i have started routing again, will update later on!! Worked on it, and i think i am done with the board again.

for proper routing, i changed the pin config many many times, and thus i have arrived to what i have today, ladies and gentlemen.  

Schematic:  
![schematic](/images/sept6/schematic.png)  
PCB:  
![PCB1](/images/sept6/pcb1.png)  
![PCB2](/images/sept6/pcb2.png)  
3d:  
![3d1](/images/sept6/3d1.png)  
![3d2](/images/sept6/3d2.png)  
I wrote a bit of the readme too!
### Time spent today: 2.5 hours

# sept 10 2025
i have sat on 13th, so i'm working less these days, anyways, i'll update production files today

oh shoot, i discovered a problem with the footprint assignment too, gotta fix that rn.