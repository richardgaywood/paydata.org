---
title: Hacking on the wireless Matrix
linkTitle: Hacking
type: docs
description: What to hack and how to hack it
date: 2020-07-05
lastmod: 2020-12-07
weight: 200
---

## Types of hacking target

Sprawlrunners' RAW defines one type of hack target - nodes. In my houserules, these are expanded as follows:

1. Unattended devices - a device connected directly to the Matrix, with no additional security, standing on its own two feet (so to speak.) Generally not very well protected against hacking. As long as they are within local mesh range, a decker can hack these.
2. Civilian personal area networks (PANs) - all someone's owned gear, connected into a single network, running off their personal commlink. Can be hacked or attacked via AR over the local mesh.
3. Secure PANs - security forces in the field often have all their gear connected to a friendly decker's cyberdeck. This cannot be hacked as such unless the decker is extremely distracted; usually, hostile deckers have to crash the deck with cybercombat instead. This is done in AR over the local mesh.
4. Hosts - as per "nodes" in RAW. Can only be "entered" (and hence hacked) if the decker is in VR. Some host nodes also protect devices in Wide Area Networks (WANs).

## Local mesh hacking

All hacking against standalone devices or PANs is done over [the local mesh]({{< relref "making_the_matrix.md" >}}) . This means the hacker must be able to reach the target via the local mesh, which is typically around 50-100 metres (but can vary with local network conditions.)

To carry out the hack, the decker rolls Hacking skill vs the device's Firewall stat (the device rating dice type divided by two - same as Toughness in meatspace.) If hacking a PAN consisting of lots of devices protected by a commlink, it's the commlink's rating that is used here.

Hacking attempts against standalone devices or PANs contribute to [the local mesh alarm state]({{< relref "alarms.md" >}}) as follows:

* successful hack with a raise - 0 points
* successful hack - 1 point
* failed hack - 2 points (and if the hack target was a PAN, the PAN owner is alerted)
* critical failure - 3 points

All local mesh hacking is carried out in augmented reality.

### Hacking standalone devices

Standalone devices have a rating and a Firewall stat (Matrix toughness) according to their type:

* Low-end consumer: d4 / 2
* High-end consumer: d6 / 3
* Security spec: d8 / 4
* Milspec: d10+ / 5+

The decker does not need to gain any sort of access before issuing hacking commands; common tasks such as opening a maglock or looping a camera feed is a single action and a single (Hacking) roll.

### Hacking PANs

Civilian PANs have ratings and Firewall (Matrix toughness) as follows:

* Low-end consumer: d4 / 2
* High-end consumer: d6 / 3
* Elite consumer: d8 / 4

To manipulate devices attached to a PAN, first the decker must hack into the PAN itself. Once there, the decker can manipulate devices on the PAN (eg snoop on phone calls, or trace the device's precise physical location). Each of those is an action and a further Hacking roll against the PAN's firewall (note: not the device's firewall), same as Sprawlrunners RAW.

**Any** failed hacking roll against a PAN immediately makes the owner aware of the intrusion attempt; they will typically react by rebooting or shutting down their device, unless they are distracted or have some reason to think they are not under attack.

## Hacking Secure PANs

Secure PANs, guarded over by a watchful decker, cannot be hacked via stealth. Any would-be attacker has to engage them in active [cybercombat]({{< relref "cybercombat.md" >}}) . Cybercombat does not contribute to the local mesh alarm score.

## Hacking Hosts and WANs

A WAN can only be hacked by entering the host or node that controls it, in VR, and avoiding or defeating the ICE within. See Sprawlrunners for rules.

Once a decker has gained access to the host or node that is running the WAN, they can issue commands to the devices connected to the WAN. This includes the Smoke action, which can be used to disrupt the gear of security forces *en masse*.


