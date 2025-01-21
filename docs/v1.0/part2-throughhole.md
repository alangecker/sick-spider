# Part 2: soldering "trough hole" components
_only valid for SICK Spider version 1.0_

## generally
- always make sure that the components are as close as possible on the board
- cut off the component legs on the bottom side (<5mm)
- when removing components, never use force, since it is quite easy to rip off pads and traces from the board. if something sticks too strong, the solder is probably still not liquid enough!

## 2.1 Power supply section
1. Solder 5.1k Ohm resistors (R23, R24)
2. Solder 15 Ohm resistor (R34)
3. Battery clip: pull the cable through the upper hole (see picture) and solder it on (red +; black -)
4. Use a cable tie to secure/relief the battery cable (see picture)
5. Solder USB Port (P1)
    * make sure port sits as close as possible on the board
    * solder 4 bigger legs first
    * solder then the smaller pins 
6. Solder Power Switch (SW4)
8. Solder reverse polarity transistor BS170 (Q1) 
    * ensure correct orientation
10. Solder 220uF capacitor (C30)
    * ensure correct orientation
11. go through the following debugging steps (see Debugging)
    * DBG-1
    * DBG-2.1
    * DBG-2.2
    * DBG-2.5
12. If 3.3V is present, create a solder bridge at JP1
13. Do test DBG-2.6


#### battery connector
![](https://pad.kanthaus.online/uploads/c0d7a9ab-cd5a-4a28-bafe-833e2b10808a.jpeg =300x) ![](https://pad.kanthaus.online/uploads/bc88aa51-bffd-4512-a903-dd0977efba91.jpeg  =300x)


## 2.2 Status LED section
1. solder 6.2V diode (D2)
2. solder 47k resistor (R19,R20)
3. solder 1k resistor (R27, R2, R25)
4. solder transistor BC547 (Q2, Q3)
    * ensure correct orientation
6. solder yellow LED (D1)
    * short leg goes into the rectangular pad
    * TODO: led distance to board
7. solder red/green battery LED (D5)
8. do tests
    * DBG-2.3
    * DBG-2.4


## 2.2b _(only with Version 1.0)_ Headphone sockets
Due to wrong hole sizes, the headphone sockets ("20-1655") don't fit, must be modified and require good access to be soldered. We rather do it now, before more components are on the board
1. Solder all 14 headphone sockets
    * they need to be as close as possible to the board
    * make sure, that there is a proper solder joint on the cut pins

## 2.3 Preamplifier section
1. solder 4.7k Ohm resistor (R36, R37, R31, R32)
2. solder 0.1uF capacitor (C24, C3, C1, C21, C29, C13, C14, C9, C10)
3. solder 220pF electrolytic capacitor (C12, C8)
4. solder 270k Ohm resistor (R29, R28)
5. solder 220 Ohm resistor (R40, R39)
6. solder potentiometers (RV1, RV2)
7. solder sockets (J2,J1)
8. do tests: DBG-3

## 2.4 Power amplifier section
1. solder black ferrit beads (FB1-4)
2. solder 220pF capacitor (C15, C18, C11, C5)
3. solder 1uF capacitor (C20, C23, C4)
4. solder 220uF electrolytic capacitor (C19)
    * ensure correct orientation
5. do tests DBG-4

## 2.5 Headphone sockets
1. solder 15 Ohm resistor for floor headphones (R16)
2. solder all 15 Ohm resistors in the headphone section
3. ~~solder all headphone sockets~~
    * they need to be as close as possible to the board
    * it is quite difficult to solder with only 2 hands, feel free to ask others for support :)
4. check, whether all pins of all headphone sockets are soldered
5. test all headphone sockets

## 2.6 Spider chain section
1. solder 220 ohm resistor (R6, R10, R21, R22)
2. solder 100k ohm resistor (R33)
3. solder 47k ohm resistor (R43, R44, R30, R17, R18)
4. solder LM358 (U4)
    * ensure correct orientation
5. solder 220pF capacitor (C17, C22)
6. solder 0.1uF capacitor (C7)
7. Solder 1u capacitator (C28) 
8. solder headphone sockets (J10, J6)
9. do tests DBG-5

## 2.7 finishing up
1. clean up all flux with isopropanol
2. have a second look on all solder joints