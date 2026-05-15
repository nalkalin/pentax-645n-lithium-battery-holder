# Printing and Assembly Notes

## Printing

- Import STL files in millimeters at 100% scale.
- PETG, ABS, or ASA is recommended for a functional holder. PLA+ is useful for quick test prints but can deform in hot storage.
- Start with 0.16-0.20 mm layer height, at least 3 walls, and 30-40% infill.
- Use supports where needed for internal ledges and the locking-base geometry.
- Print the small retainers slowly so the screw/contact features stay crisp.

After printing, test the parts together before soldering any electronics. Lightly deburr the edges that contact the camera battery bay.

## Assembly

1. Dry-fit the main body and locking base.
2. Test the M2.5 and M1.2 hardware in the printed parts.
3. Shape the copper/brass/nickel strip contacts and confirm they sit flat in the printed retainers.
4. Place the LiPo cell in the holder without pinching or bending the pouch.
5. Mount the charge/boost board where the USB-C port and wiring remain accessible.
6. Solder the battery leads to `B+` and `B-`.
7. Solder the output leads from `VO+` and `VO-` to the camera-facing contacts.
8. Use a multimeter to check output voltage, polarity, and continuity.
9. Insulate exposed solder joints and sharp metal edges.
10. Install the holder into the camera only after the electrical checks pass.

## Reference Views

![Front cross section](../images/assembly-cross-section-front.png)

![Body/base perspective](../images/body-base-perspective.png)

![Locking base top view](../images/locking-base-top-view.png)

![Body bottom view](../images/body-bottom-view.png)

## Safety

LiPo cells can be damaged by puncture, crushing, over-discharge, over-charge, or short circuits. If the cell becomes hot, swollen, punctured, or smells unusual, stop using it immediately and dispose of it according to local battery rules.
