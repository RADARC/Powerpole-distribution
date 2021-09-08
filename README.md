# Powerpole-distribution
Anderson Powerpole distribution board with reverse polarity and over voltage protection.
Designed primarily for amateur radio use.

* 4 outputs rated at 30A with a combined 30A rating.
* TVS diodes to dissipate any transient voltage spikes.
* SCR based crowbar circuit for over voltage protection.
* Latching relay to disconnect supply if the crowbar cuircuit triggers as the input fuse may take time to blow depending on the available current from the supply.
* Diode protection around the relay and enable switch to stop the output from being enabled if the polarity is reversed.
* Input fuse for added protection.
* Output fuses to protect devices which may be rated at lower currents.

# Versions
V1.1 has the powerpole silkscreen updated to indicate the true outline of the socket. The pad and holes for sw1 have been enlarged.
# Current status
Final version of the PCB (V1.1) is complete.
Trip voltage is between 15.5V and 15.9V depending on how fast the input voltage seems to rise.
# Current and voltage meter
The circuit is designed to support the use of an ammeter in order to have a voltage and current display in the same case with the board.
A suitable meter would be https://www.aliexpress.com/item/33010218601.html. There are many sellers selling similar meters. I would suggest getting
at the very least a 50A rated one and ideally 100A as the voltage drop across the current shunt will be less.
Take note that the current shunt is wired between the netative of the input and outputs. If the power supply has a grounded negative connection then
return current can flow through ground instead of the negative causing an incorrect current reading. It is undesirable for this to happen anyway
so an incorrect current reading in this case is probably a good indication that there is something wrong anyway.
# 3D case
A case is currently being designed to hold the PCB and the meter.