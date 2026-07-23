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
| 2 | Matched 3.7 V lithium cells | Use the same model, capacity, age, and state of charge. Connect in series as a 2S pack (7.4 V nominal, 8.4 V fully charged). The 103450 image is a size reference only; verify that two selected cells fit safely. |
| 1 | 2S lithium charge/boost board, USB-C input | Must support charging/protection for the selected 2S pack. Follow the exact board's documentation and confirm the regulated output voltage before connecting the camera. |
| As needed | Flexible silicone wire | Use appropriate gauge for the current draw. |
| As needed | Heat-shrink, Kapton tape, or other insulation | Cover every exposed solder joint and metal edge near the LiPo cell. |

![Lithium cell size reference](../images/103450-lipo-cell.png)

![2S lithium charge/boost board](../images/2s-lithium-charge-boost-board.png)

## Hardware

| Quantity | Part | Notes |
| ---: | --- | --- |
| 1 or more | M2.5 x 6 mm brass thumb screw | Used for the locking/contact hardware shown in the reference image. |
| 1 or more | M2.5 brass hex nut | Match the M2.5 screw. |
| 1 or more | M1.2 x 3 mm brass slotted screw | Small retaining screw. |
| As needed | Copper, brass, or nickel strip | For making the camera-facing electrical contacts. |

![Hardware reference](../images/hardware-screws-and-nuts.jpg)

## Electrical Checklist

- Confirm that the two cells are matched and connected as a 2S pack.
- Confirm that the protection/charging arrangement is intended for 2S operation.
- Confirm the boost board output voltage matches the camera's expected battery input.
- Confirm the final contact polarity before installing the holder.
- Check for shorts between positive and negative contacts.
- Do not let metal contacts rub into either lithium cell.
- Do not charge unattended.
