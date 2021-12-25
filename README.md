# OpenUMR(?): Open and Universal Mobile Robot Mother Board

The _OpenUMR_ is a PCB for making your own mobile robot.
The goals of the projects are (in no particular order):

- Design a board for containing the main electronics (electronic drives, sensors, connectors, power stage) for building your own mobile robot.
- As compatible as possible with SBCs and other computing boards, such as: RPi, Xilinx SoCs- Ultra96v2 or Kria SoM-, Adafruit Feather form factor or Arduino.
- As cheap as possible.
- Containing interfaces for connecting high data-throughput sensors, such as cameras and Lidars.
- Mobile robot for working with ROS2.
- Combining with FPGA-SOCs , able to perform HW acceleration at the edge.
- Due to component shortage, standard components for easy part number replacing.
- PMOD connectors and GPIO expansors for additional sensor attachment.
- Compatible with regular hobbyist motors.

### Interface wish-list

Ideally, this are the interfaces the board should contain.

|  |   |   |
---|---|---
**Interface**|**Connector**|**Amount**
Ethernet   | RJ45         | 1/2
USB3       | USB3 type A  | 1
MicroSD    | MicroSD Slot | 1
GPIOs      | PMOD-style   | 1
I2C        | PMOD-style   | 1
SPI        | PMOD-style   | 1
UART       | PMOD-style   | 1
Lipo Power | ?            | 1
CAN        | ?            | 1
Motor      | ?            | 1
12v out    | ?            | 1
Bluetooth  | -            | 1 chip
