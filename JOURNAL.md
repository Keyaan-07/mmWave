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

### time spent today: 10 mins