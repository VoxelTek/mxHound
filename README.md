# mxHound
### A Wii RTC-RVL (MX) relocation flex

![image](https://github.com/VoxelTek/mxHound/assets/53562267/43dbdc7d-d280-472a-bd83-501044c6b0d7)


This flexible PCB aims to simplify the relocation of the Wii MX chip, to make creating portables that utilise it as easy as possible.

Due to the overlapping of the via used for the U10, I decided to also relocate it onto here. I also added a solder pad if U10 emulation (like what's featured on the RVL-PMS line) is used, or if U10 is located elsewhere. 

This flex primarily reuses the original components found on the Wii motherboard, with the alignments as follows:

- R1 = R60 (1kΩ, 0402 (1005 metric))
- D1 = D31 (0603 (1608 metric) package, unknown specs)
- C1 = C101 (5pF, 0402 (1005 metric))
- C2 = C102 (5pF, 0402 (1005 metric))
- C3 = C98 (100nF, 0402 (1005 metric))

To reduce space, the crystal has been swapped for a smaller one. Any crystal with a frequency of 32.768 kHz and a load capacitance of 4pF in a 2mm x 1.2mm package should work fine.

Some suitable replacements:

- ABS06-107-32.768KHZ-T ([Digikey](https://www.digikey.com.au/en/products/detail/abracon-llc/ABS06-107-32-768KHZ-T/4291565) | [Mouser](https://mou.sr/3IUZvTK))
- ECS-.327-CDX-1082 ([Digikey](https://www.digikey.com.au/en/products/detail/ecs-inc/ECS-327-CDX-1082/5875549) | [Mouser](https://mou.sr/3VA6LMf))
