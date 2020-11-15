---
title: Wireless Matrix & hacking
linkTitle: Wireless Matrix
type: docs
description: Wi-fi for all!
date: 2020-07-05
weight: 500
---

By default, Sprawlrunners presents a classic cyberpunk take on cyberspace: wired decks and VR hacking. Modern Shadowrun has moved away from this somewhat to incorporate wireless technology. People have different takes on this, but I quite like the idea, so below are some houserules aimed at putting wireless hacking into Sprawlrunners - while keeping it Fast! Furious! And Fun!

*NB I will use Shadowrun-speak below ie "decker" not "operator", "host" not "system."*

## Goals

The main game scenarios these rules are intended to support are: 

1. sleazing on commlinks - snooping on calls and files, legwork type stuff, tracing people and tracking them.
2. hack the security host in a facility (in VR), then switch to AR (so the decker can move with the team), and during combat, use access to that to mess with gear on the defending security team - AR spam, disrupt smartlinks/smartguns, disrupt their comms.
3. environmental hacking - switch the lights off so the enemies are confused, turn traffic lights to green to expediate an escape, make GridGuid freak out to block pursuers with traffic, trigger a fire alarm in a building to cause confusion.

## A note about hosts and nodes in my game

Sprawlrunners RAW describes very large hosts that are made up of many, many nodes, in sprawling, labyrinthian maps. I do not plan to use this typically. Most hosts in my game will either have a single node that takes care of everything; or be divided into a small number of nodes, each dedicated to a task (eg. file access, building system control, security.) Each node can be access from any other node; there is no "map" as such.

## Types of hacking target

Sprawlrunners' RAW defines one type of hack target - hosts. In my houserules, these are expanded as follows:

1. Hosts - as per "nodes" in RAW. Can only be "entered" and hence hacked if the decker is in VR.
2. Civilian personal area networks (PANs) - all someone's owned gear, connected into a single network, running off their personal commlink. Can be hacked via AR. No concept of "entering" it in VR.
3. Standalone devices - a device just connected directly to the Matrix, standing on its own two feet (so to speak.) Generally not very well protected against hacking.
4. Host networks - security forces usually have all their gear connected to a security host for extra hack-proofing. Decker has to hack the host as normal before they can target the gear. Only works within short range of the host's hardware.
5. Deck networks - security forces in the field often have all their gear connected to an decker's cyberdeck. Cannot be hacked as such unless the decker is extremely distracted; usually, hostile deckers have to crash the deck with cybercombat.

## Hacking PANs or standalone devices

Civilian PANs typically have a rating of d4-2 / d4 / d6 (toughness 3/4/5.) Civilian-grade devices are typically d4-2 / d4. Unusually tough systems like milspec devices are higher, even without a deck network to protect them.

To hack into a PAN or device - roll Hacking vs toughness to get in. Once there, the decker can edit/copy/erase/decrypt data or manipulate the device to eg. loop camera footage, snoop on phone calls, or trace the device's precise physical location. Each of those is an action and a roll, same as Sprawlrunners RAW.

(For simplicity's sake, hacking a device to send a single command - open a maglock, loop a camera feed - will usually just be resolved via a single roll at -2.) 

To interfere with all gear connected to a PAN, a decker can also use the Smoke action; applies a -2 penalty to all actions that use gear attached to the PAN or node. -4 penalty on a Raise. This does not affect cyberware but does affect comms, weapons, drones, etc.

**Any** failed hacking roll against a PAN immediately makes the owner aware of the intrusion attempt; they will typically reboot or shut down their device, unless they are distracted or have some reason to think they are not under attack.

## Hacking hosts via a back door

If a decker can get physical access to debug ports on a device that is connected to a Host network, they can use this to get into the host more easily. This will usually require a Repair roll to access the innards of the device and hook up a cabled connection. If the decker can manage this, they take +2 on all actions in the connected node.

Sysadmins are aware of this weakness, and do not usually put external devices like cameras or maglocks onto Host networks for that reason.

## Maintaining access to a node from AR

Suppose a decker has hacked into a building facility's security node in VR and now wish to move with the team while maintaining that access.

They can do so via a new utility **KeepAlive**. This allows the decker to switch to AR while keeping their matrix presence active. They can carry out actions against whichever node they are in as if they were still in VR, although they cannot move to other nodes without logging back in.

The decker has to keep KeepAlive in their deck's memory to maintain the access. In addition, while running KeepAlive, the decker cannot act promptly to defend themselves; all ICE take +2 on all rolls against the decker.

