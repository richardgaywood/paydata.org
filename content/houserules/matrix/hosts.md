---
title: Hosts & devices
linkTitle: Hosts & devices
type: docs
date: 2020-07-19
weight: 60
description: Hosts, common devices, and IC
---


## Device ratings

* Local hosts (rating 3-8), cloud hosts (rating 6-12)
	* A/S = (Host Rating)
	* D/F = (Host Rating)+2
* Commlinks (rating 1-7)
	* A/S = 0
	* D/F = (Device Rating)
* Other devices (1-6)
	* A/S = 0
	* D/F = (Device Rating)/2

Typical device ratings:

1. Vending machines
2. Public terminals, entertainment machines
3. Standard personal electronics
4. Basic/alpha cyberware, basic vehicles
5. Beta/delta cyberware, expensive vehicles
6. (and up) Milspec 

Devices from rating 4 up might run additional protection software that grants a further +2 to +4 to its Firewall stat.

Unattended vehicles with active GridLink subscriptions automatically connect to a GridLink firewall service, giving them +2 to Firewall.

{{% alert title="Notes" %}}
*This is intended to make parked cars less of a trivial target. Otherwise every script kiddie with a hacking dongle would be causing routine chaos.*
{{% /alert %}}

### Pre-calculated defence pools and bought hits

|       	|   Naked device  	|   Vehicle  	|   Commlink/PAN  	|   Host    	|
|-------	|-----------------	|------------	|-----------------	|-----------	|
|   1   	|   2 / 0         	|            	|   2 / 0         	|           	|
|   2   	|   3 / 0         	|            	|   4 / 1         	|           	|
|   3   	|   5 / 1         	|   7 / 1    	|   6 / 1         	|   8 / 2   	|
|   4   	|   6 / 1         	|   8 / 2    	|   8 / 2         	|   10 / 2  	|
|   5   	|   8 / 2         	|   10 / 2   	|   10 / 2        	|   12 / 3  	|
|   6   	|   9 / 2         	|            	|   12 / 3        	|   14 / 3  	|
|   7   	|                 	|            	|   14 / 3        	|   16 / 4  	|
|   8   	|                 	|            	|                 	|   18 / 4  	|
|   9   	|                 	|            	|                 	|   20 / 5  	|
|   10  	|                 	|            	|                 	|   22 / 5  	|
|   11  	|                 	|            	|                 	|   24 / 6  	|
|   12  	|                 	|            	|                 	|   26 / 6  	|

First number is the dice pool, second number the bought hits.

## Hosts

### Host types

* Cloud hosts are planet-scale servers attached directly to the backbone. They can be accessed from anywhere on the planet. They are close to unhackable, not only because of their own defences, but also because of the security on uplink nodes and the backbone itself prevents hacking traffic from ever reaching them.
* Local hosts are hosts that only work in the context of the local mesh. Most corp facilities will have a local host that runs the office, provides security to wageslave's devices, and keeps all their files and work. Corporate local hosts are often combined with RF-blocking buildings to further reduce their range to inside an office. Local hosts can connect to cloud hosts for backup etc, either via the backbone or via dark fibre.
* Rumours abound of secret, powerful, arcane Foundation hosts, that are somehow tied to the mysterious force of power used by Technomancers and somehow function without any connection to the backbone at all. But 'runners are sometimes overly fond of tall tales about the dangers they faced. Who can tell if there's any truth in this...?

For more information, see [Matrix fundamentals]({{< relref "fundamentals.md#hosts" >}}).

### Local vs cloud hosts

Why don't the corps put all their valuable secrets on impregnable cloud hosts, outside of the grasp of shadowrunners? Sadly for the corps, it's not that easy.

* Highly rated cloud hosts are staggeringly expensive, and department directors and VPs are forever looking for ways to make themselves look good by cutting budget items. They're too short-sighted to realise they are leaving themselves vulnerable to espionage until too late.
* Cloud hosts are very powerful, but they still don't have enough data processing capability to run vast chunks of a megacorp's infrastructure. 
* Cloud hosts cannot form WANs, as the latency becomes too great. So corp facilities always require local hosts to run their physical security infrastructure (locks, cameras, drones, guards with guns), as well as less exciting stuff like the building's AC and the egghead's research terminals.
* The corps do not completely trust GOD, and GOD has complete dominion over traffic on the backbone. Megacorps worry their rivals will have demi-GODs in their pocket, stealing their secrets. Smaller corps worry the megacorps will steal everything. So for the most valuable secrets, the most important R&D data, the darkest paydata, there is still a need for guarded data storage in anonymous facilities and data couriers with wetware storage to move it around.

### Subsystems    

Many larger local hosts are internally divided into different subsystems. Each subsystem has a different purpose and different access levels.

For example, a corp R&D facility might have:

* general host: the lowest security level, and the first subsystem users attach to when they log in. Low-security users like admin staff might never go deeper than this.
* industrial control: runs all the obscure tech junk the eggheads are using to do their jobs
* secure file storage: where the eggheads keep their juicy data 
* security: runs the cameras, doorlocks, turrets, etc. Also runs the WAN that hosts the security personnel's guns and gear.

In game terms, each subsystem is treated as a separate host in terms of hacking rolls. Access levels are per-subsystem. Completing a hack on the general host doesn't give access to the security subsystem, and so the invading decker needs to complete a second round of hacking. However, for the purposes of Overwatch Score accumulation, the entire host is tracked as one value. For example, if a decker has Admin access to the secure file storage subsystem and User access to the general host, it's still only +2 OS per turn.

Note that there is no "map" of these hosts; the internal architecture is flat. Any user can see all the subsystems at once and move between them with ease.

{{% alert title="Notes" %}}
*The introduction of host subsystems is intended to give GMs some flexibility around the importance of a hacking target, and correspondingly, how long it'll take to resolve. Incidental hacks can be kept small and fast. Larger hacks - that provide spotlight moments for deckers - can be made more challenging. However, I have not kept host maps. I find them to be overly fussy.*
{{% /alert %}} 

### IC

When most hosts are not in an alert state, they are only running patrol IC (see below.)

Once a host is in an alert state (same conditions as tracking OS - a failed sleaze action or any attempted attack action), it starts deploying attack IC:

* Host launches 1 IC of its choosing (or randomly selected) per combat turn (at top of turn).
* The host can have (host rating) IC running at once, but can only run one copy of a given IC.
* If IC take full Matrix damage, they crash, but can be re-loaded as usual by the host.

IC stats:

* Each IC has its own Matrix damage track.
* Each IC gets one Complex action on each action phase, and all IC actions are Complex ones.
* Each IC rolls ((host rating) * 2) + 4d6 for initiative, and for ease of tracking this is usually one roll (although it can be one per IC program).
* All IC rolls (host rating) * 2 \[Attack\] to carry out its actions against a persona. For most hosts, Attack is (host rating).

#### IC types

* Patrol - see below.
* Degrader - targets the persona's weakest ASDF stat.
	* Persona resists with Willpower + the targeted stat.
	* The persona stat is reduced by the number of net hits.
	* If the stat hits zero, it prevents the deck from carrying out any actions that use that stat as a limit.
	* Persona stats are reset when the device reboots.
	* If the persona reconfigures their deck, the penalty stays with the lowest number eg. if their Attack score is reduced to 2 and they swap Attack and Sleaze, their Sleaze stat is now 2.
* Blaster / Grey IC / Black IC - damage-dealers
	* resisted with Willpower + Firewall
	* does (net hits) matrix damage to the persona
	* Grey IC also does stun biofeedback
	* Black IC also does physical biofeedback
	* Any given host will only have one of these programs; which one depends on how secure it is / how paranoid its owners are.
* Track & Trace
	* Resisted with Willpower + Firewall
	* Any net hits linklocks the decker
	* Any net hits on a decker who is already linklocked does an automatic Trace Icon test without any further chance to resist


### Patrol IC

**TODO**

