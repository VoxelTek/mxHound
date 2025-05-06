# mxHound
### A Wii RTC-RVL ("MX chip") relocation flex

![image](https://github.com/user-attachments/assets/7c52fef8-ef87-4117-a8a2-910158b5dbc4)


This flexible PCB aims to simplify the relocation of the Wii MX chip, to make creating portables that utilise it as easy as possible.

Due to the overlapping of the via used for the U10, I decided to also relocate it onto here. I also added a solder pad if U10 emulation (like what's featured on the RVL-PMS line) is used, or if U10 is located elsewhere. 

Additional pads were added for soft shutdown and the EXI bus, primarily for the RVL-DD.

This flex primarily reuses the original components found on the Wii motherboard, with the reference designators for the passive components matching the corresponding components from the Wii.

- R60 = 1kΩ, 0402 (1005 metric)
- D31 = 0603 (1608 metric) package, unknown specs
- C101, C102 = 5pF, 0402 (1005 metric)
- C98 = 100nF, 0402 (1005 metric)

To reduce space, the crystal has been swapped for a smaller one. Any crystal with a frequency of 32.768 kHz and a load capacitance of 4pF in a 2mm x 1.2mm package should work fine.

Some suitable replacements:

- ABS06-107-32.768KHZ-T ([Digikey](https://www.digikey.com.au/en/products/detail/abracon-llc/ABS06-107-32-768KHZ-T/4291565) | [Mouser](https://mou.sr/3IUZvTK))
- ECS-.327-CDX-1082 ([Digikey](https://www.digikey.com.au/en/products/detail/ecs-inc/ECS-327-CDX-1082/5875549) | [Mouser](https://mou.sr/3VA6LMf))
