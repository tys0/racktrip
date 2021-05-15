# RackTrip
RackTrip is an open-source Eurorack module that sends audio and control voltage signals over the internet. Using Raspberry Pi Zero (W) and Pure Data, RackTrip virtually and remotely patches two modular synthesizers together at low-latency.

![RackTrip prototype image](https://ccrma.stanford.edu/~tsadlier/img/racktrip_img_MMF.jpg)

RackTrip's hardware has:
* 4 CV inputs
* 4 CV outputs
* 2 audio inputs
* 2 audio outputs
* USB-C port for wired internet connections through Ethernet over USB
* GUI Controls:
    * 1.3" OLED display (I2C)
    * Rotary encoder w/ push detent
    * Tactile push button

RackTrip's custom PCB is based on "Terminal Tedium," an open-source module for audio I/O, gate I/O, and CV input to Raspberry Pi. RackTrip utilizes a modified version of Miller Puckette's "Quacktrip" Pd patch to send uncompressed audio and control rate signals between peers at low latency. Once two RackTrip modules are connected via Internet, inputs to one module are mirrored on the respective outputs of the other.

**Note:** some WIP software has not yet made it onto this repo. Build / software setup instructions to follow. Stay tuned!

## License
Software: [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) \
Hardware: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

RackTrip's Pure Data patches use a modified version of Miller Puckette's 
[Quacktrip](http://msp.ucsd.edu/tools/quacktrip/) Pure Data patch. RackTrip's software, including its Pure Data patches and C++ programs, are licensed under an MIT license.

RackTrip's hardware design is influenced by mxmxmx's terminal tedium Raspberry Pi module ([github](https://github.com/mxmxmx/terminal_tedium)) and ornament & crime module ([github](https://github.com/mxmxmx/O_C), [website](https://ornament-and-cri.me)). As a derivative work, RackTrip's hardware, including schematic and PCB files, are licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa] (CC BY-NC-SA 4.0).

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg