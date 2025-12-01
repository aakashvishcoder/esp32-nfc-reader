# ESP32 NFC Reader

My very own prototype of an NFC Reader using an ESP32 microcontroller.

# Features:
- ESP32 microcontroller
- NFC transceiver chip
- PCB antenna
- Power management
- Interfaces
- Firmware support
- Form factor

# How to Use
Plug in a USB cable into the receptacle! Install the ESP32IDE for configuration of the firmware.

# Images

<img width="299" height="552" alt="Screenshot 2025-11-30 204253" src="https://github.com/user-attachments/assets/e0dee442-2709-4721-a8d0-28f23494c02d" />
<img width="291" height="567" alt="Screenshot 2025-11-30 204249" src="https://github.com/user-attachments/assets/ff8627b0-b299-40c2-93af-86cb28b76f20" />
<img width="445" height="840" alt="Screenshot 2025-11-30 204234" src="https://github.com/user-attachments/assets/ff2b791b-b9da-4f78-973b-078361ccc2d9" />
<img width="1149" height="797" alt="Screenshot 2025-11-30 204221" src="https://github.com/user-attachments/assets/87c449f0-16c2-4bc1-9d86-435da8c773c0" />

# BOM
| Reference        | Qty | Value     | DNP | Exclude from BOM | Exclude from Board | Footprint                                                                 | Datasheet                                                                 | Price (USD ea.) | Total (USD) |
|------------------|-----|-----------|-----|------------------|--------------------|---------------------------------------------------------------------------|---------------------------------------------------------------------------|-----------------|-------------|
| AE2              | 1   | Antenna   |     |                  |                    | RF_Antenna:Coilcraft_MA5532-AE_RFID                                       | ~                                                                         | 0.80            | 0.80        |
| BZ1              | 1   | Buzzer    |     |                  |                    | Buzzer_Beeper:Buzzer_15x7.5RM7.6                                          | ~                                                                         | 1.20            | 1.20        |
| C1,C4,C6,C11     | 4   | 0.1uF     |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         | 0.10            | 0.40        |
| C2               | 1   | 47uF      |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         | 0.50            | 0.50        |
| C3,C7,C12        | 3   | 1uF       |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         | 0.04            | 0.12        |
| C5               | 1   | 4.7uF     |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         | 0.20            | 0.20        |
| C8               | 1   | 220pF     |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         | 0.08            | 0.08        |
| C9               | 1   | 100pF     |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         | 0.08            | 0.08        |
| C10              | 1   | 10uF      |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         | 0.36            | 0.36        |
| C13              | 1   | 100nF     |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         | 0.10            | 0.10        |
| C14,C15          | 2   | 15pF      |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         | 0.08            | 0.16        |
| D1               | 1   | D_Schottky|     |                  |                    | Diode_SMD:D_0402_1005Metric                                               | ~                                                                         | 0.12            | 0.12        |
| D2               | 1   | D         |     |                  |                    | Diode_SMD:D_0402_1005Metric                                               | ~                                                                         | 0.10            | 0.10        |
| D3               | 1   | WS2812B   |     |                  |                    | LED_SMD:LED_WS2812B_PLCC4_5.0x5.0mm_P3.2mm                                | [WS2812B Datasheet](https://cdn-shop.adafruit.com/datasheets/WS2812B.pdf) | 0.30            | 0.30        |
| D4               | 1   | D_TVS     |     |                  |                    | Diode_SMD:D_SMA                                                           | ~                                                                         | 0.20            | 0.20        |
| FB1              | 1   | FerriteBead_Small| |                |                    | Inductor_SMD:L_0402_1005Metric                                            | ~                                                                         | 0.20            | 0.20        |
| J1               | 1   | USB_C_Receptacle_USB2.0_16P | |      |                    | Connector_USB:USB_C_Receptacle_GCT_USB4105-xx-A_16P_TopMnt_Horizontal     | [USB Type-C Spec](https://www.usb.org/sites/default/files/documents/usb_type-c.zip) | 1.50            | 1.50        |
| J2               | 1   | Conn_01x02_Pin | |                  |                    | Connector_PinHeader_1.00mm:PinHeader_1x02_P1.00mm_Vertical                | ~                                                                         | 0.05            | 0.05        |
| J3               | 1   | Conn_01x08 | |                    | Connector_PinHeader_1.00mm:PinHeader_1x08_P1.00mm_Vertical                | ~                                                                         | 0.20            | 0.20        |
| K1               | 1   | Relay_SPDT|     |                  |                    | Relay_THT:Relay_SPDT_Finder_34.51_Vertical                                | ~                                                                         | 2.50            | 2.50        |
| L1               | 1   | 4.7uH     |     |                  |                    | Inductor_SMD:L_0402_1005Metric                                            | ~                                                                         | 0.20            | 0.20        |
| Q1               | 1   | PMOS      |     |                  |                    | Package_TO_SOT_SMD:SOT-23                                                 | [MOSFET Models](https://ngspice.sourceforge.io/docs/ngspice-html-manual/manual.xhtml#cha_MOSFETs) | 0.15            | 0.15        |
| Q2               | 1   | Q_NMOS    |     |                  |                    | Package_TO_SOT_SMD:SOT-23                                                 | ~                                                                         | 0.15            | 0.15        |
| R1,R2            | 2   | 5.1k      |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         | 0.02            | 0.04        |
| R3,R8,R10,R11,R12| 5   | 10k       |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         | 0.11            | 0.55        |
| R4,R6,R7         | 3   | 100k      |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         | 0.12            | 0.36        |
| R5               | 1   | 56k       |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         | 0.12            | 0.12        |
| R9               | 1   | 1.8k      |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         | 0.10            | 0.10        |
| R13              | 1   | 330       |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         | 0.07            | 0.07        |
| R14              | 1   | 220       |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         | 0.07            | 0.07        |
| SW1              | 1   | RESET     |     |                  |                    | Button_Switch_SMD:SW_Tactile_SPST_NO_Straight_CK_PTS636Sx25SMTRLFS        | ~                                                                         | 0.24            | 0.24        |
| SW2              | 1   | BOOT      |     |                  |                    | Button_Switch_SMD:SW_Tactile_SPST_NO_Straight_CK_PTS636Sx25SMTRLFS        | ~                                                                         | 0.24            | 0.24        |
| SW3              | 1   | USER_INPUT|     |                  |                    | Button_Switch_SMD:SW_Tactile_SPST_NO_Straight_CK_PTS636Sx25SMTRLFS        | ~                                                                         | 0.24            | 0.24        |
| U1               | 1   | ESP32-S3-WROOM-1 | |                |                    | RF_Module:ESP32-S3-WROOM-1                                                | [ESP32-S3 Datasheet](https://www.espressif.com/sites/default/files/documentation/esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf) | 4.50            |
