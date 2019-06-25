# L2SI-Vacuum-Lib
The vacuum library implements the required functionality and interlocks for all devices in the architecture document. Encapsulation of data
and logic is implemented for each device thus keeping local functionality, variables and IOs well hidden and safe from external 
modification.

The library is made up of multiple modules, i.e devices. Each vacuum device has its own function block. Each function block defines the 
interfaces, I/Os and includes all the pv/data for this particular device. All protection/run logic is implemented within the function block.

All necessary data variables are already tagged with pyTMC pragmas. Thus resulting in minimal programming to implement a device for a 
specific beamline or endstation, hence, reducing development time.

| Device | Function Block |Description |
| --- | --- |--- |
| Gauges |  | |
| --- | --- |--- |
| MKS 422| FB_MKS422| This function is for the Cold Cathode MKS 422 connected to a 937A/B. This function provides Interlock and Set Point Protection for the Cold Cathode. |
| --- | --- |--- |
| MKS 317| FB_MKS317| This function is for the Cold Cathode MKS 422 connected to a 937A/B. This function block is used to provide protection and automatic turn on of ion gauges, it also manages the turn on of the AT_VAC boolean, and checks to make sure the pressure is good  |
| --- | --- |--- |
| MKS 500| FB_MKS500| This function is for the Cold Cathode MKS 500 connected to Beckhoff EL terminals. This function provides Interlock and Set Point Protection for the Cold Cathode. |
| MKS 500| FB_MKS500_EP| This function is for the Cold Cathode MKS 500 connected to Beckhoff EP Boxes. This function provides Interlock and Set Point Protection for the Cold Cathode. |
| --- | --- |--- |
| MKS 275| FB_MKS275| This function block is used to provide protection and automatic turn on of ion gauges,
 it also manages the turn on of the AT_VAC boolean, and checks to make sure the pressure is good. |
