---
title: Hacking vehicles and drones
linkTitle: Hacking
type: docs
description: Deckers vs riggers
date: 2021-03-25
weight: 700
---

## Hacking autopilots

Any vehicle or drone that has an autopilot can be attacked from the Matrix.

### Sleaze hacking autopilots

A successful [sleaze hack]({{< relref "../matrix/hacking.md" >}}) against an autopilot is sufficient to issue it one command of about one or two sentences length *or* to Jump In to it. If you issue a command, that command can be superseded by the vehicle's or drone's owners or occupants when they notice, of course. If you Jump In, the drone or vehicle is yours to command unless/until you are overridden (see "control hierarchy" below) or somebody crashes your connection.

As usual, if the drone or vehicle is networked in a PAN, WAN, or s-PAN, that has to be dealt with (sleaze or cybercombat hacked) first.

### Cybercombat hacking autopilots

If a vehicle or drone's autopilot is crashed in cybercombat, then the autopilot and navigation is disrupted, but the occupants can still use manual controls to take over. Even if they don't, then a backup failsafe system will attempt to bring it to a safe halt. (It might fail though, they're quite basic.)

### DoS attacking drones

Drones are not smart and are easily confused by messing with their Matrix traffic. Deckers attempting DoS attacks against them take +2 on their rolls.

### Stealing cars

A single successful sleaze hack roll is enough to get a parked vehicle to unlock itself, disable the autopilot, and then activate manual controls. It can then be stolen. However, this comes with some severe caveats that kick in as soon as the theft is noticed:

* Multiple broadcast tags hidden around the body of the car will begin to broadcast prominent AR holos proclaiming the car as stolen, as well as uploading the car's location to the owner and the authorities. Finding and deactivating all the tags is extremely time-consuming (this has already been done to hot cars bought with Logistic Points.) 
	* About the only thing the thieves can do once the tags have been set off is use a [Matrix jammer]({{< relref "sprawlrunners/gear/electronics.md#wideband-wireless-matrix-jammer" >}}) to block the signals and drive like Hell.
* Gridguide will constantly issue commands to the autopilot to disable the vehicle and park up safely. The thieves have to disable it entirely and drive manually, or keep fighting for control (by re-rolling periodic Hacking tests).
	* Gridguide will also use other vehicles it controls to form rolling blockades, traffic jams, etc to impede the thieves. This complicates the "drive like Hell" strategy mentioned above.

### Throwback vehicles

Some vehicles are *throwbacks* and lack any sort of autopilot. They cannot be hacked. They can be stolen and hotwired with the Thievery skill. 

A small number of prestige throwback vehicles have been retrofitted with rigger interfaces, however. They still cannot be hacked, and a direct cable connection is required in order to Jump In to thm.

## Control hierarchy

If multiple entites are competing to control a given vehicle or drone at the same time, there's a hierarchy which determines who wins:

1. Jumped In control via a direct cable connection
2. Manual controls inside a vehicle (whether physical or via an AR interface surface) 
3. Jumped In control via a wireless connection
3. Autopilot

Hence, hacking an autopilot and issuing it commands can be overridden by anyone inside the vehicle who can access the physical controls. A rigger can jump into the vehicle remotely, but a competing rigger inside the vehicle can usurp them with a direct cable connection.


