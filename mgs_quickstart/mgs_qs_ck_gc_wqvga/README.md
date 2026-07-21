# MGS Quickstart Demo for PIC32CK GC Curiosity Ultra Board

---

**MPLAB Harmony Graphics Quickstart** | PIC32CK GC Curiosity Ultra | WQVGA Display

---

## Description

This application demonstrates basic graphics rendering using the Microchip Graphics Suite (MGS) on the PIC32CK GC microcontroller. It serves as a starting point for developing graphical user interfaces with MPLAB Harmony 3.

The demo uses the Microchip LCC (Low Cost Controller-less) driver to drive a 4.3" WQVGA (480x272) LCD via a 16-bit RGB565 interface. The LCC driver generates display timing signals directly from the MCU, eliminating the need for an external display controller.

The application displays a simple screen to verify that the graphics stack, display driver, and hardware connections are working correctly.

## Hardware Requirements

- **Development Board:** [EV44P93A – PIC32CK GC Curiosity Ultra Board](https://www.microchip.com/en-us/development-tool/ev44p93a)
- **Display Module:** [AC320005-4 – WQVGA Display](https://www.microchip.com/en-us/development-tool/AC320005-4)
- **Display Adapter:** [AC320212 - 565 LCD Adapter Graphics Card](https://www.microchip.com/en-us/development-tool/ac320212)

## Project Structure

| Folder/File                               | Description                                              |
|-------------------------------------------|----------------------------------------------------------|
| curiosity_wqvga/                          | Project root for PIC32CK GC Curiosity Ultra board        |
| src/                                      | Application source and event logic                       |
| mcc_generated_files/                      | MCC auto-generated peripheral/device files               |
| build/, out/                              | Build results and binary outputs                         |
| .vscode/                                  | VSCode workspace configs and settings                    |
| .vscode/mgs_qs_ck_gc_wqvga.mplab.json     | MPLAB project settings (do not delete)                   |
| README.md                                 | This project information file                            |

## Build Instructions

1. Open this folder in Visual Studio Code with MPLAB Extension.
2. Install and set up MCC plugin, MPLAB Harmony Graphics Suite, and toolchain.
3. Use MCC to configure peripherals and display. Regenerate code if settings change.
4. Build the project
5. Program the device and connect the display as described in hardware user guides.

## References and Links

- [EV44P93A – PIC32CK GC Curiosity Ultra Board](https://www.microchip.com/en-us/development-tool/ev44p93a)
- [AC320005-4 – WQVGA Display](https://www.microchip.com/en-us/development-tool/AC320005-4)
- [AC320212 - 565 LCD Adapter Graphics Card](https://www.microchip.com/en-us/development-tool/ac320212)
- [Microchip MPLAB Harmony Graphics Suite](https://developerhelp.microchip.com/xwiki/bin/view/software-tools/mgs/mgs-harmony-guide/)

## Notes

- Edit application logic in `src/`. Do NOT modify `mcc_generated_files` by hand.
- For wiring and setup details, refer to Microchip’s official user guides.
