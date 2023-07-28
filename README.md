# USB-C Cable Tester

[![CI](https://github.com/Qeteshpony/USB-C-Cable-Tester/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Qeteshpony/USB-C-Cable-Tester/actions/workflows/ci.yml)

![3D Render](https://qeteshpony.github.io/USB-C-Cable-Tester/3D/USB-Cable-Tester-3D_top.png)

[Hardware Documentation](https://qeteshpony.github.io/USB-C-Cable-Tester)

Small passive device for determining the capabilities of a USB-C Cable

This helps when you have a USB-C cable and don't know which USB-Version and other features it supports. 

The tester can of course not check for any active circuitry in the cable and might not work at all with active cables but in most cases it should give you a good overview.

| LED       | Meaning   |
|:----------|:----------|
| VBUS 1-4  | One LED for each VBUS connection in the cable. Can give a hint on power capabilities |
| VGND 1-4  | One LED for each Ground connection |
| Shield    | Shows if the shielding is connected on both ends |
| USB 2.0   | Lights up when the USB2 differential pair is connected |
| USB 3.x   | One LED for each set of TX/RX pairs in the cable. If only one is lit, USB3.2 will not work |
| CC        | One of these must be connected, the other should not be. A dim LED *can* be a hint for an active cable |
| SBU       | SideBand Use (See [USB Type-C Spec R2.0, chapter 4.3](https://www.usb.org/sites/default/files/USB%20Type-C%20Spec%20R2.0%20-%20August%202019.pdf)) - Used for alternate modes like audio and video connections |

The PCB is designed with production by JLCPCB in mind and all parts but the USB-Connectors are from their basic parts library. I strongly suggest getting these assembled since soldering the USB connectors by hand is not easy. 
