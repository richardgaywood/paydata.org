---
title: Types of Matrix devices and their stats
linkTitle: Devices
type: docs
description: Stats for devices, stuff that matters
date: 2021-03-23
lastmod: 2021-03-25
weight: 200
---

## Device types

Every device active on the Matrix falls into one of a small number of types:
 
* Commlink
* Cyberdeck / dronedeck
* Host
* Standalone device - any device that has a Matrix connection and isn't one of the above.

Standalone devices connected directly to the Matrix are considered *unattended*. Unattended devices are very vulnerable to deckers. To protect them, they are often connected to a commlink (via a PAN), a cyberdeck (via an s-PAN), or a host (via a WAN.) Networked standalone devices cannot be directly hacked; the decker has to hack the hosting network first.

## Matrix stats

All matrix devices are defined by a small number of stats:

* **System Rating**: a single die (d4–d12) representing how powerful the system is. Used to oppose some attempted manipulations and by ICE hosted on the system when attacking deckers.
* **Hardening** (also called **System Toughness** in Sprawlrunners): how resistant the system is to outside manipulations. Used as the target number for sleaze hacking rolls, and as the toughness target in damage rolls.
* **Firewall** (called **Cyberspace Parry** in Sprawlrunners): the device's capability to block incoming hostile datastreams. Used as the target number for cybercombat hacking rolls.

For all devices except cyberdecks, Hardening is derived from System Rating in a similar manner to Toughness in normal SWADE; half the die type, plus a bonus. The bonus is 0/+1/+2 depending on the device type. Firewall is 2 if the device lacks any active intrusion scanning. If it has such protection, then it is equal to Hardening.

## Stats

Statlines below are listed as ([System Rating]) [Hardening] / [Firewall].

<!-- https://docs.google.com/spreadsheets/d/1u1-zV-cv1DeGR5zmPJYNVKa8yY8IP2t2vUXlhB9CvUg/edit#gid=0 -->

| Grade    | Standalone device | Commlink/PAN    | Drone/Vehicle    | Host        | Cyberdeck/s-PAN                      |
|----------|-------------------|-----------------|------------------|-------------|--------------------------------------|
| Cheap    | (d4) 2 / 2        | (d4) 3 / 2      |                  | (d4) 4 / 4  | 4 / varies ("student")               |
| Civilian | (d6) 3 / 2        | (d6) 4 / 2 [^2] | (d6)[^4] 4 / 2 [^3]  | (d6) 5 / 5  | 5 / varies ("cheap")                 |
| Security | (d8) 4 / 2        | (d8) 5 / 2 [^2] | (d8) 5 / 2 [^3]  | (d8) 6 / 6  | 6 / varies ("streetware" & "corp")   |
| Military | (d10) 5 / 2 [^1]  |                 | (d10) 6 / 2 [^3] | (d10) 7 / 7 | 7 / varies ("security" & "military") |
| Elite    |                   |                 |                  | (d12) 8 / 8 | 8 / varies ("fully custom")          |

[^1]: Very unusual for these devices to be running unattended.
[^2]: Can run an [active defence package]({{< relref "additional_rules.md#commlink-defence-programs" >}})  that boosts its Firewall stat to the same as its Hardening one.
[^3]: Vehicles or drones in use will almost always be part of a PAN or s-PAN, and protected by it.
[^4]: Drone/vehicle system rating is just the autopilot's Smarts die.