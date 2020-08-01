---
title: Hosts & devices
linkTitle: Hosts & devices
type: docs
draft: true
date: 2020-07-19
weight: 50
description: Hosts, common devices, and IC
---


## Device ratings

* Local hosts: 3-8, Cloud hosts: 6-12
	* Typically, A/S are (Host Rating) and D/F are (Host Rating + 2)
* Commlinks: 1-7
	* A/S are 0, D/F are (Device Rating)
* Other devices: 1-6
	* Vending machines: 1
	* Public terminals, entertainment machines: 2
	* Standard personal electronics: 3
	* Basic/alpha cyberware, basic vehicles: 4
	* Beta/delta cyberware, expensive vehicles: 5
	* Milspec: 6+ 

Some devices from rating 4 up might run additional protection software that grants small bonuses to its Firewall stat.

Unattended vehicles with active GridLink subscriptions automatically connect to a GridLink firewall service, giving them +3 to Firewall.

{{% alert title="Notes" %}}
This is intended to make parked cars less of a trivial target. Otherwise every script kiddie with a hacking dongle would be causing routine chaos.
{{% /alert %}}

## Hosts

### Host types

* Cloud hosts are planet-scale servers attached to the backbone. They can be accessed from anywhere on the planet. They are close to unhackable, not only because of their own defences, but also because of the security on uplink nodes and the backbone itself prevents hacking traffic from ever reaching them.
* Local hosts are hosts that only work in the context of the local mesh. Most corp facilities will have a local host that runs the office, provides security to wageslave's devices, and keeps all their files and work. Corporate local hosts are often combined with RF-blocking buildings to further reduce their range to inside an office. Local hosts can connect to cloud hosts for backup etc, either via the backbone or via dark fibre.

For more information, see [Matrix fundamentals]({{< relref "fundamentals.md#hosts" >}}) 

### Subsystems    

Many hosts are internally divided into different subsystems. Each subsystem has a different purpose and different access levels.

For example, a corp R&D facility might have:

* general host: the lowest security level, and the first subsystem users attach to when they log in. Low-security users like admin staff might never go deeper than this.
* industrial control: runs all the obscure tech junk the eggheads are using to do their jobs
* secure file storage: where the eggheads keep their juicy data 
* security: runs the cameras, doorlocks, turrets, etc. Also runs the WAN that hosts the security personnel's guns and gear.

In game terms, each subsystem is treated as a separate host in terms of hacking rolls. Access levels are per-subsystem. However, for Overwatch Score accumulation, the entire host is tracked as one value. For example, if a decker has Admin access to the secure file storage subsystem and User access to the general host, it's still only +2 OS per turn.

Note that there is no "map" of these hosts; the internal architecture is flat. Any user can see all the subsystems at once and move between them with ease.

{{% alert title="Notes" %}}
*The introduction of host subsystems is intended to give GMs some flexibility around the importance of a hacking target, and correspondingly, how long it'll take to resolve. Incidental hacks can be kept small and fast. Larger hacks - that provide spotlight moments for deckers - can be made more challenging. However, I have not kept host maps. I find them to be overly fussy.*
{{% /alert %}} 

### IC

**TODO**

