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
# Assembly tips
* When soldering the powerpole sockets asemble them and insert the pins and then solder to the PCB. The shells are fine with the high temperatures
during soldering. Also it helps to plug something into them when soldering the first contact to check that they are perfectly vertical. Otherwise it is not easy
to tell and you may not realise they are at an angle until something is plugged in.
* When soldering the relay, powerpole contacts and the fuse holders use plenty of heat and fine solder and try to get the solder to flow right through to the top surface.
Both surfaces are used for carrying the large currents so it's important to have a good contact between the pins and both surfaces and not rely on the small amount of
copper in the plated through hole to conduct both sides.
* The electrolytic capacitor (C3) is a bit too tall as it would require the top of the case to be quite high making removing the fuses difficult or a hole put in the lid
for the capacitor to poke though. Therefore either lie it down or just solder it to the reverse of the board as there is plenty of space under the PCB as the height
of the case is governed by the ampmeter and the cables which plug in underneath.
* A 50W soldering iron was fine for soldering all the contacts even onto the large ground planes. The only joint which was problematic was the relay contact furthest away
from the input fuse which is probably connected to the armature and sucked away a lot of the heat.
# 3D case
A case has been designed for the PCB and the current shunt and meter mentioned above.
I have made the designs public in Tinkercad so people can modify it to fit different meters or remove the option if desired.
All screws are M3 and I made made use of metal threaded inserts.  
Base - https://www.tinkercad.com/things/e5ViJ67TmCy  
Top - https://www.tinkercad.com/things/gQ1BUrXmc8q

![Image of completed unit](https://github.com/RADARC/Powerpole-distribution/blob/main/Completed%20Unit.jpg?raw=true)