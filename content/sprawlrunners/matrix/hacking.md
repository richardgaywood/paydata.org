---
title: Sleaze hacking on the wireless Matrix
linkTitle: Sleaze hacking
type: docs
description: What to hack and how to hack it
date: 2020-07-05
weight: 275
aliases: ["sprawlrunners/deckers/hacking.md"]
---

## Types of hacking target

Sprawlrunners' RAW defines one type of hack target - nodes. In my houserules, these are expanded to include unattended devices and networks of devices controlled by a commlink, cyberdeck, or host. See [Hacking the Wireless Matrix]({{< relref "setting/matrix/hacking_the_matrix.md" >}}) for definitions of these terms.

## Local mesh hacking

All hacking against unattended devices or networks is done over [the local mesh]({{< relref "making_the_matrix.md" >}}). This means the hacker must be able to reach the target via the local mesh, which has a typical range of around 50-100 metres (but can vary with local network conditions, Faraday cages, signal-blocking smartpaint, etc.)

To carry out the hack, the decker rolls Hacking skill vs the device's Hardening stat (also called System Toughness in some places in Sprawlrunners; same thing). If hacking a network consisting of lots of devices, it's the network controller's rating that is used here.

All local mesh sleaze hacking rolls contribute to [the local mesh alarm state]({{< relref "alarms.md" >}}) as follows:

* successful hack with a raise - 0 points
* successful hack - 1 point
* failed hack - 2 points (and if the hack target was a network, the network owner is alerted)
* critical failure - 3 points (everyone on the local mesh is alerted)

All local mesh hacking is carried out in augmented reality.

### Hacking unattended devices

The decker does not need to gain any sort of access before issuing hacking commands; common tasks such as opening a maglock or looping a camera feed is a single action and a single (Hacking) roll vs the device's Hardening stat.

### Hacking networks 

To manipulate devices attached to a network, first the decker must hack into the device that is running it. Once there, the decker can manipulate devices on the network (eg snoop on phone calls, read files stored on the commlink, or trace the device's precise physical location). Each of those is an action and a further Hacking roll against the network controller's Hardening (note: not the device's Hardening), same as Sprawlrunners RAW.

**Any** failed sleaze hacking roll against a network immediately makes the owner aware of the intrusion attempt; they will typically react by rebooting or shutting down their devices, unless they are distracted or have some reason to think they are not under attack.

If the network controller device is a cyberdeck or a dronedeck, the decker/rigger also gets a chance to notice successful sleaze hacks. They roll Notice versus the results of the Hacking roll. On a success, they realise what is going on.

## Hacking networks controlled by hosts

A network controlled by a host can only be hacked by entering the host or node that controls it, in VR, and avoiding or defeating the ICE within. See Sprawlrunners for rules. Once a decker has gained access to the host or node that is running the network, they can issue commands to the devices connected to it. 

When hacking tough hosts, it can be particularly useful to compromise a device in its network and use it as a [back door]({{< relref "additional_rules.md#back-doors" >}})