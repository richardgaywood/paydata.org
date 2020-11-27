---
title: Hacking on the wireless Matrix
linkTitle: Hacking
type: docs
description: What to hack and how to hack it
date: 2020-07-05
weight: 200
---

## Types of hacking target

Sprawlrunners' RAW defines one type of hack target - nodes. In my houserules, these are expanded as follows:

1. Unattended devices - a device connected directly to the Matrix, with no additional security, standing on its own two feet (so to speak.) Generally not very well protected against hacking. As long as they are within local mesh range, a decker can hack these.
2. Civilian personal area networks (PANs) - all someone's owned gear, connected into a single network, running off their personal commlink. Can be hacked or attacked via AR over the local mesh.
3. Secure PANs - security forces in the field often have all their gear connected to a friendly decker's cyberdeck. This cannot be hacked as such unless the decker is extremely distracted; usually, hostile deckers have to crash the deck with cybercombat instead. This is done in AR over the local mesh.
4. Hosts - as per "nodes" in RAW. Can only be "entered" (and hence hacked) if the decker is in VR. Some host nodes also protect devices in Wide Area Networks (WANs).

## Local mesh hacking

All hacking against standalone devices or PANs is done over the local mesh. This has some implications:

* **Range**: the hacker must be within local mesh range of the target.

### Hacking standalone devices

Standalone devices have a rating and a Firewall stat (Matrix toughness) according to their type:

* Low-end consumer: d4 / 2
* High-end consumer: d6 / 3
* Security spec: d8 / 4
* Milspec: d10+ / 5+

They can be attacked by cybercombat or hacked as usual. The decker does not need to gain access before issuing hacking commands; common tasks such as opening a maglock or looping a camera feed is a single action and a single (Hacking) roll.

All successful or unsuccessful hacking attempts against standalone devices contribute 1 point to the alarm state of the local mesh. See [Alarms]({{< relref "alarms.md" >}}) for what this means.

### Hacking PANs

Civilian PANs have ratings and Firewall (Matrix toughness) as follows:

* Low-end consumer: d4 / 2
* High-end consumer: d6 / 3
* Elite consumer: d8 / 4

To manipulate devices attached to a PAN, first the decker must hack into the PAN itself. Roll Hacking vs toughness to do that, and accumulate alarm score as needed. Once there, the decker can manipulate devices on the PAN (eg snoop on phone calls, or trace the device's precise physical location). Each of those is an action and a Hacking roll against the PAN's toughness, same as Sprawlrunners RAW.

To interfere with all gear connected to a PAN, a decker can also use the Smoke action; this applies a -2 penalty to all actions that use gear attached to the PAN or node. -4 penalty on a Raise. This does not affect cyberware but does affect comms, weapons, drones, etc.

**Any** failed hacking roll against a PAN immediately makes the owner aware of the intrusion attempt; they will typically react by rebooting or shutting down their device, unless they are distracted or have some reason to think they are not under attack.

In addition, any successful hacking roll against a PAN or any device in a  PAN contributes 1 point to the alarm status of the local mesh, and any failed hacking roll contributes 2 points.

## Hacking Secure PANs

Secure PANs, guarded over by a watchful decker, cannot be hacked via stealth. Any would-be attacker has to engage them in active cybercombat. Cybercombat does not contribute to the local mesh alarm score.

## Hacking WANs

A WAN can only be hacked by entering the host or node that controls it, in VR, and avoiding or defeating the ICE within. See Sprawlrunners for rules.

Once a decker has gained access to the WAN, they can issue commands to the devices connected to the WAN. This includes the Smoke action, which can be used to disrupt the gear of security forces.


