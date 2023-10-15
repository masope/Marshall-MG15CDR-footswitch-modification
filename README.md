# Marshall-MG15CD-footswitch-modification-board

This Repository contains PCB design files from KiCAD and source code for modifying Marshall MG15CDR combo guitar amplifier.


## About

Old combo guitar amplifier; Marshall MG15CD, MG15CDR, MG15DFX has 2 Channel; Clean and OD (Overdrive). The amplifier doesn't have footswitch functionality for Channel or Reverb unlike it's bigger and pricier counterparts.   
   
To give little more life to this good old amplifier, I've designed add-on modification boards using ATtiny4 MCU. It can handle diverse types of switch just by changing firmware source code and upload it to MCU.   


## controller-board
![Alt text](./controller-board/controller-board-3d-image.png)

The board for channel switching. The board has power (Dual 15V and GND) and external footswitch Connector. The board is powered from the **_power-board_**.     

After remove the old channel switch, the board can be installed to amplifier using [DW-01-09-T-S-450](https://www.samtec.com/products/dw-01-09-t-s-450) Board Stacking Headers (adjust post height to 10.5mm).

The MCU can be programmed through [DF40B-10DS-0.4V(58)](https://www.hirose.com/en/product/p/CL0684-4038-8-58) Board-to-Board Connector. If you find mating connector's adaptor board, look [my other repository](https://github.com/masope/DF40C-10DP-0.4V-adaptor).


## power-board
![Alt Text](./power-board/power-board-3d-image.png)

The Dual 15V Power can be tapped-off from the amplifier's main board.

After remove the Z2, Z3 from the amplifier, install this board.