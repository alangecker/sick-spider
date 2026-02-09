# Part 1: soldering "SMD" components

_SMD_ stands for _surface mounted devices_ and means all (usually quite small) components which don't have legs going through the board.

this requires some soldering skills and you should not do this as your first soldering lesson. rather get help for this part, learn with the through-hole parts and help than the next person with the SMD soldering :)

### Required Tools
- **Soldering iron**
- **Sharp metal tweezers** for holding the components
- **Solder** 
- **Solder wick** for removing excess solder
- **Cotton swab / Q-tips** and
- **Isopropanol** for cleaning up
- **Microscope** if available or Camera with good enough zoom

<!-- 
### How to solder SMD components with solder paste & air gun
There are pleanty of tutorials to find on the internet. If you do it for the first time, maybe watch one first :)
- https://youtube.com/watch?v=rgcupYOnvBo
 -->

### Steps

##### 1.1 PAM8406 Power Amplifier (U7)
1. apply some solder to one corner pad
2. place component onto the place
    * make sure that the dot on the component (= Pin 1) matches the arrow on the board
3. with the soldering iron solder this corner pad
4. with the placement being correct, solder the opposite corner pad
5. with the placement still being correct, solder all other pads 
6. verify, that there are no bridges between contacts, if so
    * add some flux
    * work with the soldering iron and potentially the solder wick to remove the excess solder
7. clean everything with isopropanol
    * there might be tiny solder balls which could short something else
8. under the microscope check every pin, whether it is probably soldered

##### 1.2 OPA2310 Operational Amplifier (U4, U5, U6)
1. repeat process for all 3 op-amps as with the PAM8406

##### 1.3 NCV8114 Linear Regulator for 1.65V (U1)
now with increased soldering skills you can approch the much smaller components!
1. repeat process as with the PAM8406

##### 1.4 AP63203 Step Down Converter for 3.3V (U2)
1. repeat process as with the PAM8406


##### 1.5 Capacitors and coil
1. Solder C6, C16, C26 (22 uF capacitor)
2. Solder C2 (0.1 uF Capacitor)
3. Solder L1 (square coil/inductance)
4. Solder Fuse F1 (250mA)

<!-- ##### 1.6 USB port (J17)
1. place the USB port into the corresponding place
2. solder one leg
3. make sure, that the tiny pins on the back align
4. solder the other legs
5. solder the pins
6. verify, that there are no bridges between contacts, if so
    * add some flux
    * work with the soldering iron and potentially the solder wick to remove the excess solder
7. clean everything with isopropanol
    * there might be tiny solder balls which could short something else
8. under the microscope check every pin, whether it is probably soldered

 -->
##### 1.6 Verify connections
With such tiny components, it is quite easy to get a bad solder joint. Verify them but measuring following values.

1. Wait until board cooled down
2. Put Multimeter into _diode mode_ ![](https://pad.kanthaus.online/uploads/29473d7e-92cf-4de4-a4e4-7073a18f5cd6.png =50x)
3. Red multimeter probe onto GND
4. With black probe go through all the points on the picture and ensure that the values match
    * if some value does not match, check the solder joints connected to the point

![](https://pad.kanthaus.online/uploads/5b8ea4c4-59a7-4dfd-8df3-bcce6fd7ac30.png)


##### 1.7 clean up
1. Clean up once more everything with isopropanol
