# KicadFormantVCO
Started as a Clone of http://sebholzapfel.com/modular-synth-vco-design-build/

# Rev C1 - New PCB


## Status - Rev C1 Produced - received - tested
### Errata

### Issues and Notes
 - Consider 10 pin Doepfer (will make routing easier)
 - Place SMD on backside to make better room for components and traces
 - Consider TL074/MC33079
 - 1N4148 footprint - reconsider
 - trimmers on back
 - add resistor to coarse freq trim
 - add swich on PCB for LFO
 - Replace jack connectors 
 - Silk screen is off..
### Alternative components
 - Next should not rely on the LM3046 BJT as its not easy to come by.
 - Next should not rely on the REF102/AD587 as its more expensive than most and not certain if its needed.
 - Consider NAND alternative in oscilator core (74LS00 used for test without problems)
 - consider 1nF cap for VCO core (now 470p)
 - Q4 and Q5 was 2N2222 for test
 - Q1,2,3 was S9013 for the test
 - Op amp was LM833 for the test
 - Mix of 1uF and 4u7 decoupling caps for the test
 - R12 = 390k for the test
 - RV8 = 500R for the test
 - RV7=RV9 = 50k for the test
 - R9 = 240R for the test
 - R18 = 18k for the test
 - R24 = 5k6 for the test
 - R28 = 330R for the test
 
## Physical Construction

## Features


# Rev B
## Old README.md For original PCB
# SMD Formant VCO Prototype
KiCAD files for eurorack-compatible formant-based VCO design. Mostly created just to learn KiCAD.

Video on construction/operation is here: https://www.youtube.com/watch?v=rq4ovZ2om6k

## ERRATA [V1A] (To be fixed in future revision)
- The TL071 op-amp in the CAD files is arbitrary, I actually used an LM358. Just use whatever 8-pin SOIC dual op-amp you like.
- Diodes (D1..) are incorrect footprint. Change this to suit.
- 10V reference chip, VCC is not connected to +V properly. This must be bridged.
- +/-15V designator actually should be +/-12V to match eurorack. Doesn't make any electrical difference, but it's what the schematic says.
- Be careful with tantalum capacitor orientation, check with schematic. Silkscreen 'line' is negative, not positive.
