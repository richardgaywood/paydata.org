---
title: Hacking on the wireless Matrix
linkTitle: Hacking
type: docs
description: What to hack and how to hack it
date: 2020-07-05
lastmod: 2020-12-23
weight: 200
---

## Types of hacking target

Sprawlrunners' RAW defines one type of hack target - nodes. In my houserules, these are expanded to include unattended devices, PANs, secure PANs, and hosts/WANs. See [Hacking the Wireless Matrix]({{< relref "hacking_the_matrix.md" >}}) for definitions of these terms.

## Local mesh hacking

All hacking against unattended devices or PANs is done over [the local mesh]({{< relref "making_the_matrix.md" >}}) . This means the hacker must be able to reach the target via the local mesh, which is typically around 50-100 metres (but can vary with local network conditions.)

To carry out the hack, the decker rolls Hacking skill vs the device's Firewall stat. If hacking a PAN consisting of lots of devices protected by a commlink, it's the commlink's rating that is used here.

Hacking attempts against standalone devices or PANs contribute to [the local mesh alarm state]({{< relref "alarms.md" >}}) as follows:

* successful hack with a raise - 0 points
* successful hack - 1 point
* failed hack - 2 points (and if the hack target was a PAN, the PAN owner is alerted)
* critical failure - 3 points (everyone on the local mesh is alerted)

All local mesh hacking is carried out in augmented reality.

### Hacking unattended devices

Unattended devices have a rating and a Firewall stat according to their type (Firewall is dice type / 2):

* Low-end consumer: d4 / 2
* High-end consumer: d6 / 3
* Security spec: d8 / 4
* Milspec: d10+ / 5+ (unusual for these to be unattended)

The decker does not need to gain any sort of access before issuing hacking commands; common tasks such as opening a maglock or looping a camera feed is a single action and a single (Hacking) roll.

### Hacking PANs

Civilian PANs have ratings and Firewall as follows (Firewall is 1 + dice type / 2):

* Low-end consumer: d4 / 3
* High-end consumer: d6 / 4
* Elite consumer: d8 / 5

To manipulate devices attached to a PAN, first the decker must hack into the PAN itself. Once there, the decker can manipulate devices on the PAN (eg snoop on phone calls, read files stored on the commlink, or trace the device's precise physical location). Each of those is an action and a further Hacking roll against the PAN's Firewall (note: not the device's Firewall), same as Sprawlrunners RAW.

**Any** failed hacking roll against a PAN immediately makes the owner aware of the intrusion attempt; they will typically react by rebooting or shutting down their devices, unless they are distracted or have some reason to think they are not under attack.

## Hacking Secure PANs

Secure PANs, guarded over by a watchful decker, cannot be hacked via stealth. Any would-be attacker has to engage them in active [cybercombat]({{< relref "cybercombat.md" >}}) . Cybercombat does not contribute to the local mesh alarm score.

## Hacking Hosts and WANs

A WAN can only be hacked by entering the host or node that controls it, in VR, and avoiding or defeating the ICE within. See Sprawlrunners for rules. Once a decker has gained access to the host or node that is running the WAN, they can issue commands to the devices connected to the WAN. 

## Distraction hacking: messing with people's gear

Deckers can also use denial-of-service attacks to flood specific matrix devices or PANs with nonsense traffic, greatly impeding their ability to function. See [Distraction Hacking]({{< relref "additional_rules.md#distraction-hacking" >}}).

## Back doors

If a decker can get physical access to debug ports on a device, they can get easier access to hack it. They take +2 on the Sleaze roll.

This can be used when hacking standalone devices or PANs but it becomes particularly potent when hacking hosts. The bonus applies if the decker can access *any device in the host's WAN*, as well as any ports that are part of the host infrastructure itself.

To hack a host through a WAN device, this usually requires a roll of the lower of Electronics and Repair to open up the device and hook up the necessary connections. If the decker succeeds, they take +2 on all actions in the connected host node.

Host sysadmins are aware of this weakness, and do not usually put external devices like cameras or maglocks onto WANs for that reason. Security WANs tend to be reserved for more serious defences that are harder to get near, like turrets or security guard's weapons.