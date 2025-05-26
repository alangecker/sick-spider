# SICK Spider changelog

## unreleased
- replace expensive switch (200MDP3T1B1M6QE, 3-4€) by a much cheaper on (SK-23D07, ~10ct)

## Version 1.1c
- Fix misaligned traces at C16, C7 and C24
- Add missing Silkscreen value for C29
- Power switch 1mm further inside (sticks out quite a lot)
- more clearence for headphone jacks so that it is more difficult to bridge them to GND

## Version 1.1b
- Limit Microphone Gain (R36,R46)
- Battery fuse
- More room for soldering USB port
- Correct footprints for 0.1uF capacitors
- Correct footprints for 4.7k resistor

## Version 1.1
- replace MAX4062 with own preamplifier circuit in order to avoid difficult TSOP soldering
- Fix wrong footprints for 20-1655 headphone jacks
- thicker traces to reduce the chance of irreparable damage by ripping them off
- easier solderable USB-C port
- add linear regulator for stable 1.65V
- replace LM358 with rail-to-rail and 3.3V compatible OPA2310 op amp
- rounded corners
- Remove PJ359 footprints (won't use them anymore)
- label switch positions (BAT / USB) on the board

