# Printing and Assembly Notes

## Printing

- Import STL files in millimeters at 100% scale.
- SLA/MSLA/DLP resin printing is recommended because the holder has small screw, contact, and locking features.
- Use tough resin, ABS-like resin, or another engineering resin with good impact resistance.
- Start with 0.03-0.05 mm resin layer height.
- Orient parts to protect the camera-facing surfaces, avoid suction cups, and keep supports away from critical contact slots where possible.

After printing, test the parts together before soldering any electronics. Lightly deburr the edges that contact the camera battery bay.

## Assembly

1. Dry-fit the main body and locking base.
2. Test the M2.5 and M1.2 hardware in the printed parts.
3. Shape the copper/brass/nickel strip contacts and confirm they sit flat in the printed retainers.
4. Place two matched 3.7 V lithium cells in the holder without pinching, bending, or rubbing either cell.
5. Connect the cells in series as a 2S pack and mount the 2S charge/boost board where the USB-C port and wiring remain accessible.
6. Wire the pack, protection/charging connections, and output leads according to the documentation and markings for the exact module being used.
7. Connect the regulated output to the camera-facing contacts.
8. Use a multimeter to check pack voltage, regulated output voltage, polarity, continuity, and absence of shorts.
9. Insulate exposed solder joints and sharp metal edges.
10. Install the holder into the camera only after the electrical checks pass.

## Reference Views

![Front cross section](../images/assembly-cross-section-front.png)

![Body/base perspective](../images/body-base-perspective.png)

![Locking base top view](../images/locking-base-top-view.png)

![Body bottom view](../images/body-bottom-view.png)

## Safety

Lithium cells can be damaged by puncture, crushing, over-discharge, over-charge, imbalance, or short circuits. Do not mix cell models, capacities, ages, or states of charge in the 2S pack. If either cell becomes hot, swollen, punctured, or smells unusual, stop using the pack immediately and dispose of it according to local battery rules.
