# E3D lite6 clogging maintenance guide

**Clogging**. Clogging is the obstruction of the hotend due to

* damage to the PTFE liner
* buildup of impurities inside the nozzle
* filament plug between the nozzle and the heatsink or PTFE tube (due to improper assembly)

## Detecting clogging in the hotend

When a hotend starts to clog:

* Plastic flow coming out of the noozle decreases.
* More force is needed to push the filament through the nozzle.

Parts printed with a clogged hotend show signs of insufficient plastic flow: weakness, surfaces with small voids, incomplete or weak support, incomplete or weak infill, falling top layers... The flow decreases as the layers grow and sometimes the hotend may be completedly blocked before the print is finished.

[images of printed parts]

### Free flow hotend test

If the clog is already severe, it can be detected by extruding a given length of filament from the extruder. When the hotend is clogged:

* The extruded filament will be thinner than normal
* Extruder motor may lose steps

Results from the free flow test will be apparent only when the hotend is already severly clogged.

## Other causes extrusion jams

There are other causes of hotend/extruder jamming different of hotend clogging, such as:

* extruder malfunction
* filament grind
* filament tangle
* filament plug inside the hotend
* ...

**Extrusion jams not caused by hotend clogging are not to be fixed using this guide.**


## Clogged E3D lite6 maintenance tutorial

### Objectives

Hotend substitution and maintenance is performed to assure the printers 

* minimize printer down time
* get the hotend back to work with the minimun time/money spent

### Tools

* 

### Part replacement

* Always replace PTFE tube (consumable).
	* PTFE is damaged from exposure to high temperatures (from about 230-250º).
	* A damaged PTFE liner presents all or some of the following signs:
		* Sticky, thick texture
		* "Plastic" smell
		* Deformation
		* Leaked filament on the outer surface of the tube.
	* Removal of the PTFE liner with pliers deforms the tube so it cannot be used again in a production machine.
* Replace nozzle (consumable) if the hotend is clogged but the PTFE is OK.
	* If the PTFE tube is not damaged the next most likely cause of clogging is an obstructed nozzle.
* Replace silicone sock (consumable) if damage may affect hotend reliability or performance.
* Replace any other part as you see fit if damage may affect hotend reliability or performance.

### Removing hotend from the machine

1. Remove clogged hotend from the machine.
2. Install a new hotend in the printer and put aside the clogged hotend indicating that it is clogged.

### Steps

1. Dissasembly
	* Remove silicone sock.
	* Remove fan shroud with your hands.
	* Remove PTFE with pliers.
	* Unscrew nozzle with 7mm wrench, while holding the heater block with a 23mm wrench, variable wrench or bench vise.
	* Unscrew heatsink using your hands.
2. Fan cleaning
	* Remove fan screws with pozidriv screwdriver (PZ1 size).
	* Clean fan shroud with alcohol.
	* Clean fan blades as much as possible with pliers and/or alcohol.
	* Assemble fan back again.
3. Heatsink cleaning
	* Remove dust and hairspray residue from the heatsink with alcohol
	* If the inner bore has leaked plastic use the 4mm drill bit with care to remove the residue.
		* Don't use this technique if not necessary, that is, if the PTFE tube already fits well in the hotend bore and there is not leaked plastic.
		* Only use the drill bit in PTFE lined hotends, never in all metal hotend because it could damage the polished channel.	
4. PTFE replacement. Always replace PTFE liner.
	* Cut a new PTFE liner with the cutter.
		* PTFE liner is 66mm long for the E3D lite6 + E3D Titan combination.
		* You can use the sample to measure the liner to the correct length.
		* PTFE liner must have both ends cut at 90º. This is critical in the hot end of the liner to avoid leakages.
	* Insert the new PTFE liner in the heatsink.
5. Nozzle replacement. Only replace nozzle if the hotend was clogged but the PTFE liner was not damaged.
6. Heater block.
7. Hotend cold tightening. Hot tightening is not necessary if cold tightening is performed correctly.
	* Hold the heater block with a wrench or vise. Keep up the side of the heater block with three holes on it, where the nozzle is to be screwed into.
	* Screw in the nozzle all the way into the heater block by hand. 
	* Unscrew the nozzle by 1/2 of a turn.
	* Screw the heasink by hand while holding the nozzle in the position from the previous step.
	* Tighten the nozzle with the 7mm wrench. Recommended torque is 3Nm (this is about as much pressure as you can apply with one finger on a small spanner). Overtorquing will result in nozzle breaking, undertorquing may result in molten plastic leaking.


### Additional resources

* E3D lite6 documentation: https://e3d-online.dozuki.com/c/LIte6
* https://www.youtube.com/watch?v=OzRAVkXjw3I



