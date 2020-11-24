---
title: Wireless Matrix & hacking
linkTitle: Wireless Matrix
type: docs
description: Wi-fi for all!
date: 2020-07-05
weight: 500
---

By default, Sprawlrunners presents a classic '80s cyberpunk take on cyberspace: wired decks and VR hacking. Modern Shadowrun has moved away from this, blending in modern technologies like cellphones. People have different opinions about how good an idea this is, but I quite like it, so below are some houserules aimed at putting wireless devices and hacking into Sprawlrunners - while keeping it Fast! Furious! And Fun!

*NB I will use Shadowrun-speak below ie "decker" not "operator", "host" not "system."*

This doc concentrates on just the mechanics. To read information on how it works in the setting, see [Wireless World]({{< relref "wireless_world/_index.md" >}}).

## Goals

The main game scenarios these rules are intended to support are: 

1. Sleazing on commlinks - snooping on calls and files, legwork type stuff, tracing people and tracking them.
2. Hacking the security host in a facility (in VR), then switching to AR (so the decker can move with the team), and then during combat, use that access to mess with gear on the defending security team - AR spam, disrupt smartlinks/smartguns, disrupt their comms, etc.
3. Environmental support hacking - switch the lights off so the enemies are confused, turn traffic lights to green to expediate an escape, make GridGuid freak out to block pursuers with traffic, trigger a fire alarm in a building to cause confusion. The Matrix-of-things world are a decker's playground.

## A note about hosts and nodes in my game

Sprawlrunners RAW describes very large hosts that are made up of many, many nodes, arranged in sprawling, labyrinthian structures. I do not plan to use this (typically). Most hosts in my game will either have a single node that takes care of everything; or be divided into a small number of nodes, each dedicated to a task (eg. file storage, building system control, security.) Each node can typically be accessed from any other node; there is no internal "map" as such.

## Types of hacking target

Sprawlrunners' RAW defines one type of hack target - nodes. In my houserules, these are expanded as follows:

1. Unattended devices - a device connected directly to the Matrix, with no additional security, standing on its own two feet (so to speak.) Generally not very well protected against hacking.
2. Civilian personal area networks (PANs) - all someone's owned gear, connected into a single network, running off their personal commlink. Can be hacked or attacked via AR. No concept of "entering" a PAN in VR.
3. Secure PANs - security forces in the field often have all their gear connected to a friendly decker's cyberdeck. This cannot be hacked as such unless the decker is extremely distracted; usually, hostile deckers have to crash the deck with cybercombat instead. This is done in AR.
4. Hosts - as per "nodes" in RAW. Can only be "entered" (and hence hacked) if the decker is in VR. Some host nodes also protect devices in Wide Area Networks (WANs).

## Hacking standalone devices

Standalone devices have a rating and a toughness per their type:

* Low-end consumer: d4 / 2
* High-end consumer: d6 / 3
* Security spec: d8 / 4
* Milspec: d10+ / 5+

They can be attacked by cybercombat or hacked as usual. The decker does not need to gain access before issuing hacking commands; common tasks such as opening a maglock or looping a camera feed is a single action and a single (Hacking) roll.

All successful or unsuccessful hacking attempts against standalone devices contribute 1 point to the alarm state of the local mesh.

## Hacking PANs

Civilian PANs have ratings and toughness as follows:

* Low-end consumer: d4 / 2
* High-end consumer: d6 / 3
* Elite consumer: d8 / 4

To manipulate devices attached to a PAN, first the decker must enter the PAN itself. Roll Hacking vs toughness to get in. Once there, the decker can manipulate devices on the PAN (eg snoop on phone calls, or trace the device's precise physical location). Each of those is an action and a Hacking roll against the PAN's toughness, same as Sprawlrunners RAW.

To interfere with all gear connected to a PAN, a decker can also use the Smoke action; this applies a -2 penalty to all actions that use gear attached to the PAN or node. -4 penalty on a Raise. This does not affect cyberware but does affect comms, weapons, drones, etc.

**Any** failed hacking roll against a PAN immediately makes the owner aware of the intrusion attempt; they will typically react by rebooting or shutting down their device, unless they are distracted or have some reason to think they are not under attack.

In addition, any successful hacking roll against a PAN or any device in a  PAN contributes 1 point to the alarm status of the local mesh, and any failed hacking roll contributes 2 points.

## Hacking Secure PANs

Secure PANs, guarded over by a watchful decker, cannot be hacked via stealth. Any would-be attacker has to engage them in active cybercombat. Cybercombat does not contribute to the local mesh alarm score.

## Hacking WANs

A WAN can only be hacked by entering the host or node that controls it, in VR, and avoiding or defeating the ICE within. See Sprawlrunners for rules.

Once a decker has gained access to the WAN, they can issue commands to the devices connected to the WAN. This includes the Smoke action, which can be used to disrupt the gear of security forces.

## Alert states

...tbd...

## Additional rules

### Hacking hosts via a back door

If a decker can get physical access to debug ports on a device that is connected to a WAN, they can use this to get into the host that is running the WAN more easily. This will usually require a roll of the lower of Electronics and Repair to open up the device and hook up the necessary connections. If the decker succeeds, they take +2 on all actions in the connected node.

Sysadmins are aware of this weakness, and do not usually put external devices like cameras or maglocks onto WANs for that reason. Security WANs tend to be reserved for more serious defences that are harder to get near, like turrets or security guard's weapons.

### Maintaining access to a node from AR

Suppose a decker has hacked into a building facility's security node in VR and now wish to move with the team while maintaining that access.

They can do so via a new utility called **KeepAlive**. This allows the decker to switch to AR while keeping their matrix presence active. They can carry out actions against whichever node they are in as if they were still in VR, although they cannot move to other nodes without logging back in.

The decker has to keep KeepAlive in their deck's memory to maintain the access. In addition, while running KeepAlive, the decker cannot act promptly to defend themselves; all ICE take +2 on all rolls against the decker.

