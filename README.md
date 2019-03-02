# KicadFormantVCO
Started as a Clone of http://sebholzapfel.com/modular-synth-vco-design-build/

# Rev C1 - New PCB


## Status - Rev C1 Produced - received - tested
### Errata

### Issues and Notes
 - Next should not rely on the LM3046 BJT as its not easy to come by.
 - Next should not rely on the REF102/AD587 as its more expensive than most and not certain if its needed.
 - Consider 10 pin Doepfer (will make routing easier)
 - Place SMD on backside to make better room for components and traces
 - Consider NAND alternative in oscilator core (74LS00 used for test without problems)
 - Consider TL074/MC33079
 - 1N4148 footprint - reconsider
 - trimmers on back
 - add resistor to coarse freq trim
 - consider 1nF cap for VCO core (now 470p)

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
