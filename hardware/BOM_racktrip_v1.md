# BOM for RackTrip

Using [O&C BOM](https://ornament-and-cri.me/build-it/) and [Terminal Tedium BOM](https://github.com/mxmxmx/terminal_tedium/wiki) as reference(s).



## Capacitors 0603
note: use 25v or better

| value | # | note | mouser # |
| --- | ---: | --- | --- |
| 18p | 8x | 0603 / NP0/C0G | 80-C0603C180J5G |
| 20pF | 2x | 0805 / NP0/C0G | 80-C0805C200J5G (change to 0603 later) |
| 10n | 5x | 0603 / NP0/C0G | 80-C0603C103J3G |
| 100n | 16x | 0603 / MLCC | 80-C0603C104K3R7081 |
| 470n | 3x | 0603 / MLCC | 80-C0603C474K3R |
| 1uF | 1x | 0805 / MLCC | 80-C0805C105K3R |
| 10uF | 2x | 0805 / MLCC | 80-C0805C106K3P or 963-TMK212BBJ106KG-T |

## Resistors 0603
| value | # | note | mouser # |
| --- | ---: | --- | --- |
| 200R | 1x | | 603-RC0603FR-07200RL |
| 220R | 4x | non-ferrite bead | 603-RC0603FR-07220RL |
| 220R | 4x | ferrite bead; buffer btwn wm8731 and rpi | 81-BLM18BB221SN1D |
| 510R | 2x | | 603-RC0603FR-07510RL |
| 1k | 2x | | 603-RC0603FR-071KL |
| 4k7 | 2x | | 603-RC0603FR-074K7L |
| 5k6 | 2x | | 603-RC0603FR-075K6L |
| 10k | 4x | | 603-RC0603FR-0710KL |
| 11k8 | 1x | | 603-RC0603FR-0711K8L |
| 12k4 | 0x (or 4x) | | 603-RC0603FR-0712K4L |
| 24k9 | 8x (or 4x) | | 603-RC0603FR-0724K9L |
| 27k | 2x | | 603-RC0603FR-0727KL |
| 33k | 1x | | 603-RC0603FR-0733KL |
| 47k | 6x | | 603-RC0603FR-0747KL |
| 100k | 12x | | 603-AC0603DR-07100KL |


## Electrolytic Caps, SMD

| value | # | note | mouser # |
| --- | ---: | --- | --- |
| 10uF | 5x | 16V or better; diameter < 5.3mm | 647-UUQ1E100MCL1GB |
| 33uF | 2x | 25V or better; diameter < 8mm | 140-VE330M1HTR0607|

## ICs/semis/etc:

| what | # | desc | package | mouser # |
| --- | ---: | --- | --- | --- |
| WM8731 | 1x | stereo codec | TSSOP-28 | 238-WM8731SEDS/V |
| AD5592R | 1x | DAC/ADC for CV | TSSOP-16 | 584-AD5592RBRUZ |
| MCP6004 | 1x | CV input op-amp | SOIC-14 | 579-MCP6004T-I/SL |
| OPA4172 | 1x | CV output op-amp | SOIC-14 | 595-OPA4172IDR |
| OPA1678 | 2x | Audio I/O op-amp | SOIC-8 | 595-OPA1678IDR |
| ADP150 | 1x | 3v3 regulator | TSOT | 584-ADP150AUJZ-3.3R7 |
| SM5817PL-TP | 2x | diodes for power | SOD-123FL | 833-SM5817PL-TP |
| LM4040-10v | 1x | 10v for ?? | SOT-23 | 926-LM4040DIM3100NPB |
| LM4040-2v5 | 1x | 2v5 for 2V bias circuit (CV output) | SOT-23 | 998-LM4040CYM3-2.5TR or  522-LM4040C25FTA |
| 5V DC converter | 1x | R-785.0-0.5 (or 1.0) | t-h | 919-R-785.0-0.5 |


## Through-Hole Parts:
| what | # | ref | where | note |
| --- | ---: | --- | --- | --- |
| Mono jacks | 12x | Thonkiconn PJ398SM | Thonk | |
| Rotary encoder | 1x | PEC11R | Mouser # 652-PEC11R-4220F-S24  | |
| tactile switch | 1x | mecs 5ETH935 | mouser # 642-5GTH935 or [sos electronics](https://www.soselectronic.com/products/mec/5gth935-102165) | |
| 12.288 MHz Crystal | 1x | 20pF | Mouser # 559-FOXS128-20-LF | HC-49/S, low-profile |
| inductance, 10uH | 1x | - | mouser # 542-78F100-RC | - |
| electrolytic capacitor, 10uF | 2x | 2.5mm / 16V+ (for DC block / audio output) | mouser # 647-UFG1H100MDM |

## Etc
| what | # | ref | where |
| --- | ---: | --- | --- |
| Knurled / Hex Nuts for jacks | 12x | | Thonk |
| Washers for jacks | 12x | | Thonk |
| 1.3" OLED display | 1x | SH1106 or SSD1306 / 128x64 / 4 Pins or I2C | Amazon |
| Encoder Knobs | 1x | Small Encoder BLACK (D Shaft) Rogan | Thonk |
| Switch bezel or cap | 1x | | mouser # 642-1SS09-09.5 or 642-1US09 |
| 1x4 Socket for OLED | 1x | "2.54mm, low profile but not “machined” sockets with round holes for the pins" | Mouser # 517-929870-01-04-RA |
| raspberry GPIO socket, 2x20 | 1x | RM2.54, extra-tall female socket for RPI (†) | mouser # 485-2222 |
| 2x5 male pins for power socket | 1x | | mouser # 649-67996-410HLF |
| 1x2 female pin for 5V jumper | 1x | | mouser # 517-929870-01-02-RA  |