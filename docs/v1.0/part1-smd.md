# Part 1: soldering "SMD" components
_only valid for SICK Spider version 1.0_

_SMD_ stands for _surface mounted devices_ and means all (usually quite small) components which don't have legs going through the board.

this requires some soldering skills and you should not do this as your first soldering lesson. rather get help for this part, learn with the through-hole parts and help than the next person with the SMD soldering :)

### Required Tools
- **Hot air rework station**
- **Soldering iron**
- **Sharp metal tweezers** for holding the components
- **Solder paste**
- **Solder wick** for removing excess solder
- **soldering flux** 
- **Cotton swab / Q-tips** and
- **Isopropanol** for cleaning up
- **Microscope** if available or Camera with good enough zoom

### How to solder SMD components with solder paste & air gun
There are pleanty of tutorials to find on the internet. If you do it for the first time, maybe watch one first :)
- https://youtube.com/watch?v=rgcupYOnvBo

### Steps

##### 1.1 PAM8406 Power Amplifier (U7)
1. apply solder paste on all pads (like in the video)
2. place component onto the pad
    * make sure that the dot on the component (= Pin 1) matches the arrow on the board
3. use hot air gun to melt the solder. thanks to the surface tension the component will move in place as soon as the solder is liquid enough
4. verify, that there are no bridges between contacts, if so
    * add some flux
    * work with the soldering iron and potentially the solder wick to remove the excess solder
5. clean everything with isopropanol
    * there might be tiny solder balls which could short something else
7. under the microscope check every pin, whether it is probably soldered


##### 1.2 AP63203 Step Down Converter (U2)
1. repeat process as with the PAM8406


##### 1.3 Capacitors and coil
1. Solder C6, C16, C26 (22 uF capacitor)
2. Solder C2 (0.1 uF Capacitor)
3. Solder L1 (square coil/inductance)

##### 1.4 MAX4062 Pre-Amplifier (U5, U6)
now with increased soldering skills you can approch the final enemy, the MAX4062, which is in a really tiny form.

1. U5, U6: repeat process as with the PAM8406
2. check the pins with a microscope

##### 1.5 Verify connections
With such tiny components, it is quite easy to get a bad solder joint. Verify them but measuring following values.

1. Wait until board cooled down
2. Put Multimeter into _diode mode_ ![](https://pad.kanthaus.online/uploads/29473d7e-92cf-4de4-a4e4-7073a18f5cd6.png =50x)
3. Red multimeter probe onto GND
4. With black probe go through all the points on the picture and ensure that the values match
    * if some value does not match, check the solder joints connected to the point

![](https://pad.kanthaus.online/uploads/dc49981d-4ab2-4325-a5af-7b57c5bcf03b.png)


##### 1.6 clean up
1. Clean up once more everything with isopropanol
