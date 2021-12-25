# KRIA SoM Design Notes

### Power Rails Requirements

| Power Rail Name | Voltage Range | Max I | Description |
|---|---|---|---|
| _Vcc\_SoM_ | 5v(50mV vpp) | 4A | Main power IN |
| _VCC\_BAT_ | 1.2-1.5V | 150-3650nA | External RTC IN  |
| _VCCO\_HPA_ | 1-1.8V | 1A | HPIO B66|
| _VCCO\_HPB_ | 1-1.8V | 1A | HPIO B65|
| _VCCO\_HPC_ | 1-1.8V | 1A | HPIO B64|
| _VCCO\_HDA_ | 1-1.8V | 1A | HDIO B45|
| _VCCO\_HDB_ | 1-1.8V | 1A | HDIO B43|
| _VCCO\_HDC_ | 1-1.8V | 1A | HDIO B44|

I/O tolerance: +3/-2%

### Power On Sequence

1. VCC_SOM
2. Carrier card deasserts _POWER\_OFF\_C2M\_L_
3. KRIA SOM asserts _VCCOEN\_PS\_M2C_ => turn on PS peripheral power rails
4. KRIA SOM asserts _VCCOEN\_PL\_M2C_ => turn on PL peripheral power rails and VCCO rails.


Source: https://www.xilinx.com/support/documentation/data_sheets/ds987-k26-som.pdf
