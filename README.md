# Shaurya-AGV-Embedded-PCB-nPM110-

This project involves the design and layout of a high-efficiency Power Management Module based on the Nordic nPM1100 PMIC. The board is engineered to provide a robust 3V logic rail at a nominal 200ma charging rate.
The PCB follows a 2-Layer approach where Copper Pour(Ground) has been done on both planes with a primary focus on maintaining a solid, contiguous Ground Plane on the bottom layer. By minimizing signal routing on the bottom a low-impedance return path for the high-frequency switching currents is ensured 
The Designs prioritises Power integrety , a effort has been made into ensuring minimum SW- trace and keeping the decoupling capacitors as close as possible with multiple ground vias attached to them
Various LED for power CHG and ERR are placed , MCU is exposed to multiple pins including CHG ERR Mode SHPACT and a battery charge monitering system has been introduced.
A switch has also been connected to SHPLD to turn on the IC manually.
Values of various Pins like VSET and resistance like R_ICHG are tune to ensure a 200ma nominal charging current and a max 4.2VBAT with the data from the datasheet.
In the battery monitering system the MCU is given controll through Q1 and Q2 on when to measure the battery voltage, to reduce power loss .
