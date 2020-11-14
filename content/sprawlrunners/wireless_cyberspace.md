---
title: Chargen
linkTitle: Chargen
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

## Types of hacking target

Sprawlrunners' RAW defines one type of hack target - hosts. Expand that as follows:

1. Hosts - as per "nodes" in RAW. Can only be "entered" and hence hacked if the decker is in VR.
2. Civilian personal area networks (PANs) - all someone's owned gear, connected into a single network, running off their personal commlink. Can be hacked via AR. No concept of "entering" it in VR.
3. Host networks - security forces usually have all their gear connected to a security host for extra hack-proofing. Decker has to hack the host as normal before they can target the gear. Only works within short range of the host's hardware.
4. Deck networks - security forces in the field often have all their gear connected to an decker's cyberdeck. Cannot be hacked as such unless the decker is extremely distracted; usually, hostile deckers have to crash the deck with cybercombat.

## Hacking PANs

Civilian PANs typically have a rating of d4-2 / d4 / d6 (toughness 3/4/5.) Unusually tough systems like milspec devices are higher, even without a deck network to protect it.

To hack into a PAN - roll Hacking vs toughness to get in. Once there, the decker can edit/copy/erase data, decrypt data, manipulate the device to eg. snoop on phone calls or trace the target's location. Each of those is an action and a roll, same as Sprawlrunners RAW.

To interfere with all gear connected to a PAN, a decker can also use the Smoke action; applies a -2 penalty to all actions that use gear attached to the PAN or node. -4 penalty on a Raise. This does not affect cyberware but does affect comms, weapons, drones, etc.

**Any** failed hacking roll against a PAN immediately makes the owner aware of the intrusion attempt; they will typically reboot or shut down their device.

## Maintaining access to a host

Suppose a decker has hacked into a building facility's security node in VR and now wish to move with the team while maintaining that access.

They can do so via a new utility **KeepAlive**. This allows the decker to switch to AR while keeping their matrix presence active. They can carry out actions against whichever node they are in as if they were still in VR, although they cannot move to other nodes without logging back in.

The decker has to keep KeepAlive in their deck's memory to maintain the access. In addition, while running KeepAlive, the decker cannot act promptly to defend themselves; all ICE take +2 on all rolls against the decker.

