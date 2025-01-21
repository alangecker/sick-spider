# Debugging issues
_only valid for SICK Spider version 1.0_

## Required Tools
- something outputting a sinus signal on a 2-pin 6.3mm Jack cable, either
    * Smartphone or Laptop with
        - a 2-Pin ("TS") 3.5mm -> 6.3mm Jack cable (e.g. https://www.thomann.de/intl/the_sssnake_adapter_cable_6_3_3.5_mm.htm)
        - https://draemm.li/various/tonegen/
        - with set to full volume the spider could already distort, maybe rather put it to 50%
    * Signal generator
        - 440 Hz
        - 1V (signal should not distort until 1.3V)
- XLR -> TRS Jack cable
- USB-C Power supply
- 9V Battery (full)
- Multimeter
- Oscilloscope

## DBG-1 Short circuits
Set Switch to "USB" (to the left / away from the usb port) and measure resistance between following points, all values should be >10 kOhm. You can find the points next to the USB Port.
1. GND and Vin (TP3)
1. GND and 3.3V (TP1)
1. GND and 3.3VA (TP4)

## DBG-2 Power supply
1. Plug in USB, set switch to USB (left) and measure voltage between GND and V_in (TP3). it should around 5V. If not
   * check the USB power supply
   * check solder joints on P1, SW4
2. Plug in a Battery, set switch to Battery (right) and measure voltage between GND and V_in (TP3). it should be between 5V and 9V (depending on the battery state) if not
   * check battery voltage
   * check orientation of the battery connector BT1 (red should go to +)
   * check orientation of MOSFET Q1
3. The ON-LED (D1) should light up. if not
   * check solder joints on D1, R2
   * check orientation of LED (D1)
4. With a battery the battery status LED (D5) should light up. if not
   * check all solder joints in the status LED section
   * check orientation of LED (D5), diode (D2) and transistors (Q2,Q3)
5. Verify with a battery 3.3V between GND and TP1 if not
   * check orientation of U2
   * check all solder joints of the SMD components in the power supply section
   * it still not working, U2 might be broken and needs to be replaced
6. Check with a battery for 3.3V at TP4 (3.3VA)
   * check solder bridge JP1
   * check solder joints of R34

## DBG-3 Preamp
1. Floor input (left): Set volume potentiometer as low as possible, plug in a sinus signal (see "Required tools"). With an oscilloscope confirm a sinus signal between R29 (at the arrow) and GND, if not
  * check all solder joints at U6, potentially bridged between two pins
  * check all solder joints in that area
  * check for 3.3V on C21
2. Sinus wave on oscilloscope should in-/decrease with raising/lowering the volume potentiometer, if not
  * check all solder joints on potentiometer
  * check the two most right solder joints on U6
3. Repeat the same for the interpreter input (right) on R28
  * check all solder joints on potentiometer
  * check the two most right solder joints on U5

## DBG-4 Power Amplifier
1. Disconnect any input and measure the DC voltage at every ferrit bread (FB1-4) against GND. it should be 1.6-1.8V, if not
    * check all solder joints on U7 and ferrit breads
    * replace U70 
2. Connect a sinus signal to the floor input (left) and measure the DC voltage across FB3 ↔ FB4. it should be <30mV, if not
    * // TODO
3. Measure AC voltage across FB3 and FB4. it should be >0.3V and in-/decrease with the volume potentiometer
    * // TODO
4. Repeat step 2 with interpreter input and DC voltage across FB1 ↔ FB2
5. Repeat step 3 with interpreter input and AC voltage across FB1 ↔ FB2


## DBG-5 spider chain

:::info

**TODO**
:::