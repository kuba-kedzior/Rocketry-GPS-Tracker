Project Description:

This is a 30mm by 50mm radio tracker, 
It can be powered via a 7.4V or 9V battery. 
It can act either as a base station or Flight computer

Upon CAN Connection to a 
seprate device with compatible firmware, 
it will exchange and transmit data.

Primary Project goals:
Implement a FreeRTOS codebase.
Gain more familiarity with the STM32 ecosystem
Implement a working CAN bus

Secondary Project goals:
Developed compatibility with the LEEP Nexus
Report GPS Error Ellipse, not just position
HIL Verification
Implement DMA
Impelment Voting in clustered modules
Monitor System Voltage with STM32 PVD


Key design decisions:

STM32F103C8T6 was chosen due to its inclusion in the JLCPCB Basic component catalogue.

An integrated LoRa module was chosen over a barebones RF module because of lack of RF design knowledge.
The LoRa1268F30-Mini-433 was chosen due to its high gain (27.4Db at 3.3V), along with it's Simple Interface.

LE80RE GPS Module Is used for cost effectiveness, datasheet readability, and Compact form factor.

Terminal blocks are used for most external connections to make integration possibilities as low-cost as possible.

No resistor is added to the CAN bus, allowing for more than 2 trackers on a single bus.

USB power support allows for use a s a groundstation via USB

Data budget can be found in [this spreadsheet](https://docs.google.com/spreadsheets/d/102A4YWSmNOC4Mrc8TIuKeTcN84fMUZAXphBgqFSV5SE/edit?gid=0#gid=0)
