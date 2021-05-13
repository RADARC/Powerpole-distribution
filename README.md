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
First prototype pcb's have arrived and the circuit has been tested and works.
Trip voltage is between 15.5V and 15.9V depending on how fast the input voltage seems to rise.

