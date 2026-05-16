# TurtleBoard
The TurtleBoard is a development board based on the RP2040 chip. It features 43 pins, including most standard GPIO pins, an onboard potentiometer, and LED.<br>
I made this board to learn PCB design and to understand the inner workings of dev boards. This was hell to figure out for the first time, but insanely rewarding and probably more educational than anything I ever did at school. 
Front:
<img width="934" height="422" alt="image" src="https://github.com/user-attachments/assets/639630f2-dc61-4a3e-936c-c133c592c471" />
Back:
<img width="764" height="423" alt="image" src="https://github.com/user-attachments/assets/887b2742-a852-49e5-8eda-a4909ff98ee0" />
Sadly, the back has no silly drawing, which is because my KiCad kept crashing whenever I tried doing anything with it, so I left it alone out of fear of corrupting the design file or something.

# Schematic
<img width="1138" height="793" alt="image" src="https://github.com/user-attachments/assets/0638877d-36c0-4981-8f9f-4761e8b03fcd" />

# PCB
<img width="358" height="796" alt="pcb" src="https://github.com/user-attachments/assets/cd88917f-540c-4484-bfef-03e173227217" />
<img width="413" height="812" alt="image" src="https://github.com/user-attachments/assets/0da9d649-74d9-4b9c-b905-a5009ee7c017" />


# BOM
|Reference                      |Quantity|Comment                    |Total Cost|Part #|Exclude from Board|Footprint                                                 |Datasheet                                                                        |
|-------------------------------|--------|---------------------------|---|----------------|------------------|----------------------------------------------------------|---------------------------------------------------------------------------------|
|C1,C10                         |2       |1uF                        |$0.04|CL05A105KA5NQNC|                  |Capacitor_SMD:C_0402_1005Metric                           |~                                                                                |
|C2,C3,C4,C5,C6,C7,C8,C9,C11,C12|10      |0.1uF                      |$0.0825|CL05B104KO5NNNC|                  |Capacitor_SMD:C_0402_1005Metric                           |~                                                                                |
|C13,C14                        |2       |10uF                       |$0.102|CL10A106KP8NNNC|                  |Capacitor_SMD:C_0603_1608Metric                           |~                                                                                |
|C15,C16                        |2       |33pF                       |$0.013|0402CG330J500NT|                  |Capacitor_SMD:C_0402_1005Metric                           |~                                                                                |
|C17                            |1       |0.1uF                       |   |CL05B104KO5NNNC|                  |Capacitor_SMD:C_0402_1005Metric                           |~                                                                                |
|D1                             |1       |LED                        |$0.332|16-213SDRC/S530-A3/TR8|                  |LED_SMD:LED_0402_1005Metric                               |~                                                                                |
|J1                             |1       |USB_C_Receptacle_USB2.0_14P|$0.918|TYPE-C-31-M-12|                  |Connector_USB:USB_C_Receptacle_HRO_TYPE-C-31-M-12         |https://www.usb.org/sites/default/files/documents/usb_type-c.zip                 |
|J2,J3                          |2       |Conn_01x20                 |   |2.54-1*20P直针|                  |Connector_PinHeader_2.54mm:PinHeader_1x20_P2.54mm_Vertical|~                                                                                |
|J4                             |1       |Conn_01x03                 |   |1.27-1*3P针|                  |Connector_PinHeader_2.54mm:PinHeader_1x03_P2.54mm_Vertical|~                                                                                |
|R1,R2                          |2       |5.1K                       |$0.009|0402WGF5101TCE|                  |Resistor_SMD:R_0402_1005Metric                            |~                                                                                |
|R3,R4                          |2       |27                         |$0.0176|0402WGF270JTCE|                  |Resistor_SMD:R_0402_1005Metric                            |~                                                                                |
|R5,R7                          |2       |1K                         |$0.01|0402WGF1001TCE|                  |Resistor_SMD:R_0402_1005Metric                            |~                                                                                |
|R6                             |1       |10K                        |$0.0065|0402WGF1002TCE|                  |Resistor_SMD:R_0402_1005Metric                            |~                                                                                |
|R9                             |1       |220                        |$0.0045|0402WGF2200TCE|                  |Resistor_SMD:R_0402_1005Metric                            |~                                                                                |
|RV1                            |1       |R_Potentiometer            |   |3214J-1-503E|                  |Potentiometer_SMD:Potentiometer_Bourns_3214J_Horizontal   |~                                                                                |
|SW1                            |1       |SW_Push                    |$0.028|TS-1088-AR02016|                  |Button_Switch_SMD:SW_Push_SPST_NO_Alps_SKRK               |~                                                                                |
|U1                             |1       |RP2040                     |$4.8940|RP2040|                  |Package_DFN_QFN:QFN-56-1EP_7x7mm_P0.4mm_EP3.2x3.2mm       |https://datasheets.raspberrypi.com/rp2040/rp2040-datasheet.pdf                   |
|U2                             |1       |MCP1700x-330xxTT           |$2.398|MCP1700T-3302E/TT|                  |Package_TO_SOT_SMD:SOT-23                                 |http://ww1.microchip.com/downloads/en/DeviceDoc/20001826D.pdf                    |
|U3                             |1       |W25Q16JVZPIQ TR            |$8.0815|W25Q16JVUXIQ|                  |Package_SON:Winbond_USON-8-1EP_3x2mm_P0.5mm_EP0.2x1.6mm   |https://www.winbond.com/resource-files/w25q128jv_dtr%20revc%2003272018%20plus.pdf|
|Y1                             |1       |12MHz                      |$0.368|X322512MSB4SI|                  |Crystal:Crystal_SMD_3225-4Pin_3.2x2.5mm                   |~                                                                                |
JLCPCB's estimated cost is $53.58
