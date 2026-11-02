# KCD1-104B / KCD117

Added to Dlib.SchLib as KCD1-104B: a generic 4-pin DPST ON/OFF rocker.
Contacts 1-2 and 3-4 are mechanically linked. Pin numbers are library assigned;
check continuity on the actual OEM switch before using the wiring.

The symbol links to KCD1_104B_4PIN_RA_VISUAL_REF in Dlib.PcbLib.
The footprint includes an embedded, original simplified STEP model resembling
the user's photographed right-angle black rocker. It is not manufacturer CAD.
No external STEP path is needed. Press 3 in the PCB library to see it.
The user requested a similar shape and did not require footprint matching.
The 10 x 5 mm pad grid and 21 x 15 mm bezel are reference dimensions only;
this footprint is not validated for fabrication or mechanical interchangeability.

Reference product and drawing:
- https://www.thegioiic.com/kcd1-104b-kcd117-cong-tac-bap-benh-on-off-mau-den-4-chan-cong-6a
- https://file.thegioiic.com/upload/large/9421.jpg

Existing DC jack, left unchanged:
- Symbol: Jack DC 5.5*2.1, in RD Intergrated Lib schematic/Connector.SchLib
- Footprint: JACK_DC 5.5 mm, in RD Intergrated Lib pcb/Connector.PcbLib
- Embedded 3D: Jack DC.STEP

The existing KCD1 XL601-101 KA-15-3 symbol is a different 3-pin switch and
was preserved. All other Dlib symbols, footprints and embedded models remain.
