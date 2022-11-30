Welcome!

First: Shoutout to HDR. His work was extremely vital in completing this project. Take a look at his github and check out some of the cool projects he has worked on!

https://github.com/HDR

Second: You do this entire transfer at your own risk. I am not responsible for anything that happens to your game as a result of taking on this project. This is not a beginner task, and should definitely not be taken on as a first-time solder project.  I am not affiliated with any of the companies mentioned here. I do not do this for profit. This is just a neat little thing I decided to work on. 

This project is open source. Users may use this work to iterate, or improve upon it. In doing so, please make sure you follow the Creative Common License linked below below. Out of respect for HDR. Do not be a bad actor. your compliance is expected, and appreciated. DMG-KGDU-10 is an original Nintendo PCB design. I take no credit for that. 

https://creativecommons.org/licenses/by-nc-sa/4.0/

What is this project about?


In simple terms - This project is an upgraded replacement circuit board for games like Pokémon Gold, Silver, and Crystal. This board utilizes FRAM instead of SRAM so you can save your games without the need for a battery. The battery is still required for the real time clock (RTC) to function. But the good news is you will not lose any save data when the battery does die. More will be explained later. This board was designed with the United States version of the games in mind. I created this board for a few reasons. 

1. SRAM is annoying and I hate that my save data was at the mercy of a simple coin cell battery. This fixes that and allows for a very clean and professional looking mod without wires running all over the place.

2. I see tons of reddit posts of people posting their Pokemon Gold, Silver, or Crystal games in less than stellar condition. Sure, you can use jumper wires, and if you like that, it's all you. Some are beyond repair due to corrosion, broken traces, or just problems that aren't solvable. If the ROM IC, and MBC3 mapper are in good shape. This board will definitely save your game. Your games are not broken if your circuit board is in bad shape!

3. To learn.


How can I get my hands on these boards?

In order to get your hands on these boards, you will need to download this project zip, or clone it using GIT. One of the files labeled DMG-KGDU-10+_Gerber.zip Is the completed output of the circuit board. There are a few websites you can upload this to in order to get these boards made. they are not that expensive. These are the ones I use often. But feel free to use another if you’re comfortable with them. 




Note: PLEASE ORDER THESE BOARDS WITH THE FOLLOWING SPECIFICATIONS. IF YOU DO NOT ORDER THEM CORRECTLY, THEY WILL NOT WORK, OR WILL NOT FIT!

* Thickness: 0.8mm
* Color: Your choice! Have fun!
* Surface Finish: (ENIG or Immersion Gold. They’re the same thing) , or Hard Gold (expensive). DO NOT USE ANY OTHER OPTION. 
* Castellated Holes: No
* Copper Weight: 1oz is fine. 2oz is nice but not needed.
* Golden Fingers: Yes 
* 45° finger chamfered

1. JLCPCB: https://jlcpcb.com/

o This company is based in China, and has very good pricing on boards so long as you choose either green or purple. I find the best bang for your buck to be 10 boards as it's not that much more expensive than 5.

2. Elecrow: https://www.elecrow.com/

o This company is based in China, the pricing is great, and pricing is similar to JLCPCB and seems consistent across all colors. So I love these guys quite a bit. 

o Note: If using Elecrow, you will need to send them an email to specify that you want Golden Fingers, and beveled 45° finger chamfered. Just give them your order number after you place it. 


3. Osh Park: https://oshpark.com/

o Osh Park is a USA based company. Their online gerber viewer and order process is very easy. But your options are very limited. You can only get your boards in their signature deep purple color, which are quite nice. They’re also the most expensive. Their quality is good. You get less PCB’s for your money, and I noticed that it could still take a while for them to come in.

o When you order, choose the option that says: 2 oz copper, 0.8mm thickness and you should be all set. Their ordering process is more streamlined. 







**BOM:**

| Reference | Part | Description | Type |
|-|-|-|-|


BILL OF MATERIALS

You will need the following materials to complete this build. Feel free to source these from wherever you’d like. I’ll throw in some recommendations though. 

Reference | Part | Description | Type


U1 | Original ROM | The lower Right chip. This is the chip that holds your game and is needed from the original board. | 44 Pins 
U2
MBC3
Memory Bank Controller. You can only get this from an original Cartridge
LQFP-32
U3
FM18W08
256kbit FRAM
SOIC-28
U4
BA6129AF
Battery Reset IC. Get From Original Cartridge or AliExpress
SOIC-8
U5
74LVC1G32GV,125
2-input OR Gate
TSOP-5
C1, C2, C3, C6, C7
CL10B104KO8NNNC
100nF Capacitor
0603
C4, C5
CL10C150JB8NNNC
15pF Capacitor
0603
R1
RC0603FR-07330KL
330K ? Resistor
0603
R2
RC0603FR-0710KL
10K ? Resistor
0603
R3
RC0603FR-071KL
1K ? Resistor
0603
R4
RMCF0603ZT0R00
0K ? Resistor
0603
X1
R26-32.768-12.5-10PPM 20PPM seems to work fine as well.	
32.768 kHz Crystal. Buy or get from original Cartridge
RTC Crystal
Batt 2025
BK-6219-TR
CR2025 Battery Retainer
Battery Retainer


Some Tips

1). This should not be your first major solder project. Do not attempt to do this without any practice, or you risk ruining your game. 

2). Everything is pretty straight forward. Make sure you’re good with working on small components. Capacitors and resistors are not easy to solder if you’re new to this. Solder paste and hot air can help you out a lot with that process. 

3). The battery cell sometimes may not make amazing contact with the large circle pad. This is because it is ever so slightly recessed into the board. This can be fixed in a variety of ways. 

My way of solving this issue is cutting out a thin piece of nickel strip (I try to make it circular in shape, and a bit smaller than the edges of the circle pad. And I lay it down flat and solder it in place before installing the BK-6219-TR retainer. Make sure you solder in the retainer so you can place the battery in from the top side of the board. If you do it upside down, getting the battery in will be annoying because the ROM IC gets in the way. 

Another way, if you don’t want to cover the pad with solder is Makhos way. Makho uses a piece of copper tape on the circle pad, rather than soldering in the nickel strip that I use. It’s nice if you don’t want to get solder on the circle pad. I personally don’t mind but the choice is yours. 


Good luck! Be sure to post your successes, and feel free to ask me any questions!


