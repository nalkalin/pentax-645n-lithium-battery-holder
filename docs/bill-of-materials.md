# Bill of Materials

This list is based on the reference material images included in this repository. Equivalent parts may work if they match the electrical requirements and fit inside the printed holder.

## Printed Parts

| Quantity | File | Notes |
| ---: | --- | --- |
| 1 | `models/pentax-645n-lithium-holder-body.stl` | Main holder body. |
| 1 | `models/pentax-645n-lithium-holder-locking-base.stl` | Bottom locking/base part. |
| 1 | `models/pentax-645n-lithium-holder-top-contact-retainer.stl` | Small upper contact/retainer part. |
| 1 | `models/pentax-645n-lithium-holder-lower-contact-spacer.stl` | Small lower spacer/contact support. |
| 1 | `models/pentax-645n-lithium-holder-bottom-contact-retainer.stl` | Small lower contact/retainer part. |

## Electronics

| Quantity | Part | Notes |
| ---: | --- | --- |
| 1 | 103450 LiPo pouch cell, 3.7 V, about 2000 mAh | The reference image shows a 103450 cell. Use a protected cell or a module with cell protection. |
| 1 | Lithium charge/boost board, USB-C input | The reference board has `B+`, `B-`, `VO+`, and `VO-` pads. Confirm the regulated output voltage before connecting to the camera. |
| As needed | Flexible silicone wire | Use appropriate gauge for the current draw. |
| As needed | Heat-shrink, Kapton tape, or other insulation | Cover every exposed solder joint and metal edge near the LiPo cell. |

![103450 LiPo cell](../images/103450-lipo-cell.png)

![Lithium charge/boost board](../images/lithium-charge-boost-board.jpg)

## Hardware

| Quantity | Part | Notes |
| ---: | --- | --- |
| 1 or more | M2.5 x 6 mm brass thumb screw | Used for the locking/contact hardware shown in the reference image. |
| 1 or more | M2.5 brass hex nut | Match the M2.5 screw. |
| 1 or more | M1.2 x 3 mm brass slotted screw | Small retaining screw. |
| As needed | Copper, brass, or nickel strip | For making the camera-facing electrical contacts. |

![Hardware reference](../images/hardware-screws-and-nuts.jpg)

## Electrical Checklist

- Confirm the boost board output voltage matches the camera's expected battery input.
- Confirm the final contact polarity before installing the holder.
- Check for shorts between positive and negative contacts.
- Do not let metal contacts rub into the LiPo pouch.
- Do not charge unattended.
