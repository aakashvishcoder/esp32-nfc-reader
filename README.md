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
<img width="311" height="595" alt="Screenshot 2025-11-30 002322" src="https://github.com/user-attachments/assets/a23eaea0-3d0e-4660-864a-02fcb65eb087" />
<img width="315" height="604" alt="Screenshot 2025-11-30 002317" src="https://github.com/user-attachments/assets/ac182631-f975-4009-b49d-b56192b7ba57" />
<img width="441" height="833" alt="Screenshot 2025-11-30 002309" src="https://github.com/user-attachments/assets/a25a5959-d3ae-4063-b6d0-ba8cb55c8eaa" />
<img width="1160" height="801" alt="Screenshot 2025-11-30 002255" src="https://github.com/user-attachments/assets/b453d46d-b063-4df9-aa4d-9c81cd1daf79" />

# BOM
| Reference        | Qty | Value     | DNP | Exclude from BOM | Exclude from Board | Footprint                                                                 | Datasheet                                                                 |
|------------------|-----|-----------|-----|------------------|--------------------|---------------------------------------------------------------------------|---------------------------------------------------------------------------|
| AE1              | 1   | Antenna   |     |                  |                    | Connector_PinSocket_2.54mm:PinSocket_1x01_P2.54mm_Vertical                | ~                                                                         |
| BZ1              | 1   | Buzzer    |     |                  |                    | Buzzer_Beeper:Buzzer_15x7.5RM7.6                                          | ~                                                                         |
| C1,C4,C6,C11     | 4   | 0.1uF     |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         |
| C2               | 1   | 47uF      |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         |
| C3,C7,C12        | 3   | 1uF       |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         |
| C5               | 1   | 4.7uF     |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         |
| C8               | 1   | 220pF     |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         |
| C9               | 1   | 100pF     |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         |
| C10              | 1   | 10uF      |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         |
| C13              | 1   | 100nF     |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         |
| C14,C15          | 2   | 15pF      |     |                  |                    | Capacitor_SMD:C_0402_1005Metric                                           | ~                                                                         |
| D1               | 1   | D_Schottky|     |                  |                    | Diode_SMD:D_0402_1005Metric                                               | ~                                                                         |
| D2               | 1   | D         |     |                  |                    | Diode_SMD:D_0402_1005Metric                                               | ~                                                                         |
| D3               | 1   | WS2812B   |     |                  |                    | LED_SMD:LED_WS2812B_PLCC4_5.0x5.0mm_P3.2mm                                | [WS2812B Datasheet](https://cdn-shop.adafruit.com/datasheets/WS2812B.pdf) |
| D4               | 1   | D_TVS     |     |                  |                    | Diode_SMD:D_SMA                                                           | ~                                                                         |
| FB1              | 1   | FerriteBead_Small| |                |                    | Inductor_SMD:L_0402_1005Metric                                            | ~                                                                         |
| J1               | 1   | USB_C_Receptacle_USB2.0_16P | |      |                    | Connector_USB:USB_C_Receptacle_GCT_USB4105-xx-A_16P_TopMnt_Horizontal     | [USB Type-C Spec](https://www.usb.org/sites/default/files/documents/usb_type-c.zip) |
| J2               | 1   | Conn_01x02_Pin | |                  |                    | Connector_PinHeader_1.00mm:PinHeader_1x02_P1.00mm_Vertical                | ~                                                                         |
| J3               | 1   | Conn_01x08 | |                    |                    | Connector_PinHeader_1.00mm:PinHeader_1x08_P1.00mm_Vertical                | ~                                                                         |
| K1               | 1   | Relay_SPDT|     |                  |                    | Relay_THT:Relay_SPDT_Finder_34.51_Vertical                                | ~                                                                         |
| L1               | 1   | 4.7uH     |     |                  |                    | Inductor_SMD:L_0402_1005Metric                                            | ~                                                                         |
| Q1               | 1   | PMOS      |     |                  |                    | Package_TO_SOT_SMD:SOT-23                                                 | [MOSFET Models](https://ngspice.sourceforge.io/docs/ngspice-html-manual/manual.xhtml#cha_MOSFETs) |
| Q2               | 1   | Q_NMOS    |     |                  |                    | Package_TO_SOT_SMD:SOT-23                                                 | ~                                                                         |
| R1,R2            | 2   | 5.1k      |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         |
| R3,R8,R10,R11,R12| 5   | 10k       |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         |
| R4,R6,R7         | 3   | 100k      |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         |
| R5               | 1   | 56k       |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         |
| R9               | 1   | 1.8k      |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         |
| R13              | 1   | 330       |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         |
| R14              | 1   | 220       |     |                  |                    | Resistor_SMD:R_0402_1005Metric                                            | ~                                                                         |
| SW1              | 1   | RESET     |     |                  |                    | Button_Switch_SMD:SW_Tactile_SPST_NO_Straight_CK_PTS636Sx25SMTRLFS        | ~                                                                         |
| SW2              | 1   | BOOT      |     |                  |                    | Button_Switch_SMD:SW_Tactile_SPST_NO_Straight_CK_PTS636Sx25SMTRLFS        | ~                                                                         |
| SW3              | 1   | USER_INPUT|     |                  |                    | Button_Switch_SMD:SW_Tactile_SPST_NO_Straight_CK_PTS636Sx25SMTRLFS        | ~                                                                         |
| U1               | 1   | ESP32-S3-WROOM-1 | |                |                    | RF_Module:ESP32-S3-WROOM-1                                                | [ESP32-S3 Datasheet](https://www.espressif.com/sites/default/files/documentation/esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf) |
| U2               | 1   | AP63203WU |     |                  |                    | Package_TO_SOT_SMD:TSOT-23-6                                              | [AP63203WU Datasheet](https://www.diodes.com/assets/Datasheets/AP63200-AP63201-AP63203-AP63205.pdf) |
| U3               | 1   | PN5321A3HN_C1xx | |                |                    | Package_DFN_QFN:HVQFN-40-1EP_6x6mm_P0.5mm_EP4.1x4.1mm                      | [PN532 Datasheet](https://www.nxp.com/docs/en/nxp/data-sheets/PN532_C1.pdf) |
| Y1               | 1   | 27.12MHz  |     |                  |                    | Crystal:Crystal_HC49-U-3Pin_Vertical                                      | ~                                                                         |
