# L2SI-Vacuum-Lib
The vacuum library implements the required functionality and interlocks for all devices in the architecture document. Encapsulation of data
and logic is implemented for each device thus keeping local functionality, variables and IOs well hidden and safe from external 
modification.

The library is made up of multiple modules, i.e devices. Each vacuum device has its own function block. Each function block defines the 
interfaces, I/Os and includes all the pv/data for this particular device. All protection/run logic is implemented within the function block.

All necessary data variables are already tagged with pyTMC pragmas. Thus resulting in minimal programming to implement a device for a 
specific beamline or endstation, hence, reducing development time.

