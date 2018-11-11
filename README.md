# MK-312BT V1.3

Documentation at : http://tinyurl.com/mk312bt-info

Forum (for questions/discussion): https://metafetish.club ([Estim
Specific Category Here](https://metafetish.club/c/estim), but may not
include all estim messages)

## Board ordering instructions

Preferred board house is https://jlcpcb.com

You'll need 2 gerber zip files from the gerbers directory (click links below to download):

- [MK-312 V1.2 Front Panel](https://github.com/buttshock/mk312-bt/blob/master/gerbers/ZIP%20FILES/MK-312BT%20Front%20Panel%20V1.2%20Gerber.zip?raw=true)
- [MK-312 V1.3 Main Board](https://github.com/buttshock/mk312-bt/blob/master/gerbers/ZIP%20FILES/MK-312BT%20Main%20Boards%20V1.3%20Gerber.zip?raw=true)

**NOTE:** Order Front Panel and Main Board as seperate items (but they
can be in the same cart), due to difference in "Different Design"
setting. See below.

- 2 Layer PCB and Dimensions should be detected when you upload the
  zip with the gerbers
- Quantity: No requirement, choose whatever you like
- Thickness: 1.6
- PCB Color: No requirement, choose whatever you like
- Surface finish: HASL
- Copper weight: 1oz
- Gold fingers: No
- Material: Standard FR4
- Panel by jlcpcb: No
- Different Design 
   - 2 for main boards
   - 1 for front panel

## Board Assembly Instructions - IMPORTANT

1. Trim Potentiometer knobs to correct length if desired
2. Use black permanent marker to black out front panel hole walls if
   desired
3. Cut the tabs off of the base of the pots so the board sits flush
   with the display facade if desired
4. To correctly fit LCD - solder header to LCD board first. Next
   insert LCD panel into front panel daughter board. Then put screws
   on front panel facade and finger tighten M2.5 screws first. Adjust
   positions as needed so everything lines up and sits well. Finally
   solder LCD header to front panel daughter board.
5. Make sure Pin 32 (LED2) on the HC-05 module is actually soldered
   and making connection to the ZS-040 break out board or "Radio" LED
   may not function on the front panel
6. Be very careful not to bridge pins when soldering the LM 2941
   (U14). Apply heat to 1 pad only and carefully apply solder. If a
   bridge occurs - remove the IC, clean the pads throughly with flux
   and solder wick and then retry. Pins 2 and 3 can be bridged because
   they are both ground. Ensure that no other pins are bridged. Check
   with multimeter continuity tester for bridges before power on!
7. Make sure to check the orientation of all electrolytic caps. (+)
   indicates the positive and a solid white "|" indicates the negative.
8. MAKE SURE YOUR POWER PLUG IS CENTER POSITIVE OR THINGS WILL GO
   BADLY. If you fuck up and plug in a reversed polarity supply -
   replace electrolytic caps C1 and C4.
9. Please remember to adjust the LCD contrast potentiometer - if
   incorrectly set the unit and backlight will power on but the
   interface will not be displayed.
10. Place transformers with P facing the output jacks (yes we are
    using the transformers "backwards" if you follow orientation given
    in the transformer datasheet )
11. Trim pins of 4066 IC (U3) Socket on the front panel board flush
    before soldering so buttons can clear. If the buttons still
    interfere, carefully disassemble the button and cut off the bit of
    the plastic housing that interferes with the 4066 IC socket pins.
12. Using side cutters cut off the screw boss/screw mount on the case
    that touches/interferes with the ribbon cable socket on the
    display board.
13. The LCD display has metal retention tabs that may short the
    soldered leads of C43. When installing the display board ensure
    that this does not happen (shorten the capacitor leads and bend
    the offending metal tab out of the way if necessary
14. If Error 20 is encountered on first boot:
   - Check that all FETs and Transformers are turned in the correct direction
   - Check that resistors R35 and R46 these should be 200k
   - [See this thread on the message board](https://metafetish.club/t/mk-312bt-failure-20/)
