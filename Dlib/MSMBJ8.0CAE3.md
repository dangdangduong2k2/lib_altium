# MSMBJ8.0CAE3 Altium library addition

Search name: MSMBJ8.0CAE3
Symbol library: Dlib.SchLib
Footprint library: Dlib.PcbLib
Footprint: MICROCHIP_SMBJ_DO214AA_BIDIR

Microchip bidirectional TVS, 8 V working standoff, 8.89-9.83 V breakdown at 1 mA,
13.6 V maximum clamp at 44.1 A, 600 W peak for a 10/1000 us pulse (not continuous).
Two passive interchangeable terminals, mapped 1-to-1 to pads 1 and 2.
SMB / DO-214AA J-bend land pattern: two 2.16 x 2.79 mm pads at X = +/-2.22 mm.
Recommended Microchip overall pad span: 6.60 mm. Mask expansion 0.05 mm;
paste expansion 0 mm. Mechanical 1 body envelope, Mechanical 15 courtyard.
No 3D model included for this new part.

Source: Microchip DS00005167A, electrical page 6, package page 11, pads page 12.
https://ww1.microchip.com/downloads/aemDocuments/documents/HRDS/ProductDocuments/DataSheets/RF01000%2B(3).pdf

APPLICATION LIMIT: This 8 V part is NOT a suitable replacement for the protection
of a general RS-232 input that can reach +/-12 V. It can conduct during valid data.
Check signal amplitude, TVS capacitance and protection coordination before use.
The user schematic has not been modified.

The included Dlib files also retain the previously added DRV8825PWPR and 0R2 resistor.
Install the rebuilt lib_altium.IntLib from the existing library project's Project Outputs,
or use these source libraries. Existing unrelated compiler issues are documented in
that project's VALIDATION.md; see verification.json for this component's checks.
