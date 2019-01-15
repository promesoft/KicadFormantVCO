# KicadFormantVCO
Started as a Clone of http://sebholzapfel.com/modular-synth-vco-design-build/

# Rev C1 - New PCB


## Status - Rev A Produced 3 of 5 sections working
### Errata

### Issues and Notes
 - The two ESP12 modules are difficult to program

 - The Wemos D1 mini section should not be used for 230V but works nevertheless.

 - The rest is fine.

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
