---
title: Gridguide
linkTitle: Gridguide
type: docs
description: What it does and how it works
date: 2021-01-19
weight: 200
---

Gridguide is a centralised, automated traffic control system. When within its jurisdictional area, vehicles are guided and advised by its management systems. This covers both traffic routing around the city, managing flow for minimal congestion, and second-to-second control for accident avoidance and junctions.

Gridguide's area is expansive but not total. It covers all major roads throughout the city, and all minor roads in downtown areas. It fades out in side-streets in the suburbs and is completely absent in the Barrens.

## Game mechanics

In game terms, GridGuide acts as a special sort of WAN that all vehicles are connected to. This does not provide the usual anti-hacking protection that WANs do, but it does provide the following game benefits:

* All Piloting and Notice rolls the vehicle makes get a d6 Wild die.
* While the vehicle is in motion, it gets the benefit of the [Active Integrity Checking]({{< relref "additional_rules.md" >}}) program, and so rolls Hardening instead of Firewall to resist attempts to crash it. (Parked vehicles are not a hazard if their computers get crashed, so the system doesn't cover them.)
* Vehicles have numerous tracking tags hidden in various places on their body shell. Gridguide tracks their location in realtime through these tags. Finding and disabling them all is a difficult and lengthy process.
* If any decker hacks control of a vehicle with a GridGuide connection, it will continue to attempt to re-assert control; it rolls d8 vs the decker's Hacking skill. *(todo: how often?)*
  * This applies during remote control or normal control via augmented reality surfaces in the vehicle. But some vehicles (not all) are fitted with either manual override controls or rigger adapters. Using either of those completely locks Gridguide out, stopping the attempts to re-establish control.

## Hacking Gridguide

As a very well-defended cloud host, hacking Gridguide directly is extremely difficult. However, Gridguide uses a distributed architecture with delegated controls to short-range local hosts, responsible for vehicle control across a small area as well as associated infrastructure like traffic lights. These are vulnerable to hacking in the usual way. They count as standalone devices with a d8 rating. Once a decker gains access, they can issue commands to all nearby connected devices, including vehicles - one hacking roll per command. Note that this will often quickly attract attention from GOD, however it can still be used to facilitate a speedy escape.


