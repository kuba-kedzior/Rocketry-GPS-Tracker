Project Description:

this is a 40mm by 40mm radio tracker, 
it can be powered via a 7.4V or 9V battery. 
it can act either as a base station or 
Flight computer

Upon CAN Connection to a 
seprate Device with Compatible firmware, 
it will exchange and transmit data.

Project goals:
Implement a FreeRTOS codebase.
gain more familiarity with the STM32 ecosystem
Implement a Working CAN bus

Compatibility will be developed for the LEEP Nexus

Key design decisions:

STM32F103C8T6 was chosen due to its inclusion in the JLCPCB Basic component catalogue.

C1200 Radio module was chosen due to its use in the Telemetrum flight computer (expect similar radio performance)

LE80RE GPS Module Is used for cost effectiveness, datasheet readability, and Compact form factor.

Terminal blocks are used for most Wire connections to make connection possibilities as versitile as possible.

No resistor is added to the CAN bus, allowing for more than 2 trackers on a single bus.

USB power support allows for use a s a groundstation via USB
