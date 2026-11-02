# Amphenol 73725-0110BLF Altium addition

Search: 73725-0110BLF
Symbol: Dlib.SchLib
Footprint: USB_A_UPRIGHT_73725-0110BLF in Dlib.PcbLib
USB 2.0 Type-A receptacle, upright right-angle, through-hole, white housing,
without sensor contact, hold-down style A, 2.29 mm contact tails.

Pins 1=VBUS, 2=D-, 3=D+, 4=GND. S1-S4 are library-assigned shield stake labels.
All eight terminals are passive. Four shell stakes are electrically common in
hardware; connect the shield terminals consistently in the schematic.

Dimensions are from Amphenol drawing 73725, Rev AL1, sheet 2:
- Signal holes: 0.92 mm diameter, 2.00 mm pitch; 1.50 mm copper pads.
- Shell holes: 1.35 mm diameter; grid 5.44 x 7.00 mm; 2.10 mm copper pads.
- All eight holes plated. Use drawing hole tolerances in fabrication requirements.
- Origin is center between front shell stakes; pin 1 is at (0, +0.73) mm.
- Mating face is Y=-11.76 mm; body extends to Y=+7.94 mm.
- Body shell envelope is 5.76 x 19.70 mm. PCB thickness 1.00-1.60 mm.
- Top silkscreen avoids pad openings; Mechanical 1 body, Mechanical 15 courtyard.
- Mechanical 13 marks the mating face and outward cable direction. This is NOT
  a board cut or an enforced PCB edge; choose board/panel edge position for your enclosure.
- Solder-mask expansion 0.05 mm. No paste openings for through-hole assembly.
- Copper pad diameters and courtyard clearances are library design choices;
  manufacturer-specified hole geometry and pitch are maintained.

Source:
https://www.amphenol-cs.com/product/737250110blf.html
https://cdn.amphenol-cs.com/media/wysiwyg/files/drawing/73725.pdf
The manufacturer's drawing was read from the distributor-hosted copy:
https://s3.us-west-2.amazonaws.com/catsy.925/73725.pdf

Embedded manufacturer STEP model included (73725-0110BLF-aligned.step).
Press 3 in the PCB/PCB Library editor to view it. For a previously placed
footprint, update it from this library first. No external STEP path is needed.

Manufacturer original: 73725-0110blfc.stp, FCI ELX, 2009-06-04.
Downloaded archive: https://s3.us-west-2.amazonaws.com/catsy.925/s73725-0110blf.zip
The aligned copy preserves shape, with coordinates in mm:
X = original Z - 0.384; Y = original Y + 1.373; Z = 2.080 - original X.
PCB top is Z=0; four signal contact axes match the pads exactly. The original
CAD is older than the current drawing: its mating face is Y=-11.79 mm versus
-11.76 mm in the drawing. Use the current drawing for fabrication dimensions.
Original and aligned STEP files are retained in 3D/Amphenol_USB73725.
Native Altium 3D display, embedded STEP bytes, and contact axes were checked.

Similar appearance does not establish compatibility with
the connector in the supplied photos. Verify actual part number/lead pattern.

The existing Dlib libraries were updated in the library repository and its
lib_altium.IntLib rebuilt. Source libraries in this archive retain the previous
DRV8825PWPR, 0R2 and MSMBJ8.0CAE3 additions. User schematic/PCB was not modified.
See verification.json and compile-log.txt for checks and existing project issues.
