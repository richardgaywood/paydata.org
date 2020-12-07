
---
title: Additional rules
linkTitle: Additional rules
type: docs
description: Extra bits and pieces; hacking via back doors; new utilities
date: 2020-11-27
lastmod: 2020-12-07
weight: 800
---

## Distraction hacking

A decker facing an opponent using wirelessly connected devices can distract them by interfering with the systems using a special form of the Test action (see SWADE pg 108.) The decker makes a Hacking roll opposed by the target's Smarts stat. The following modifiers apply:

* If the target has a few items of cyberware and/or wireless gear: no modifier.
	* If they have lots of gear, extensive cyberware, or both: +1 to the decker's roll
	* If the target is a drone or vehicle working on autopilot: +2 to the decker's roll
* If the target's gear is protected by a PAN and the decker hasn't hacked the PAN: -2 to the decker's roll
* If the target's gear is protected by a secure PAN, or by a WAN that the decker hasn't hacked: -4 to the decker's roll

On a success, the decker can inflict either Distracted or Vulnerable on the target, as they prefer. On a Raise, they can also inflict Shaken.

{{% alert title="TODO" color="warning" %}}Add something here about internal routers?{{% /alert %}} 

## Hacking hosts via a back door

If a decker can get physical access to debug ports on a device that is connected to a WAN, they can use this to get into the host that is running the WAN more easily. This will usually require a roll of the lower of Electronics and Repair to open up the device and hook up the necessary connections. If the decker succeeds, they take +2 on all actions in the connected node.

Sysadmins are aware of this weakness, and do not usually put external devices like cameras or maglocks onto WANs for that reason. Security WANs tend to be reserved for more serious defences that are harder to get near, like turrets or security guard's weapons.

## Maintaining access to a hacked node from AR

Suppose a decker has hacked into a building facility's security node in VR and now wish to move with the team while maintaining that access.

They can do so via a new utility called **KeepAlive**. This allows the decker to switch to AR while keeping their matrix presence active. They can carry out actions against whichever node they are in as if they were still in VR, although they cannot move to other nodes without logging back in.

The decker has to keep KeepAlive in their deck's memory to maintain the access. In addition, while running KeepAlive, the decker cannot act promptly to defend themselves; all ICE take +2 on all rolls against the decker.

## Reducing the local mesh alarm score

Deckers can use a new utility called **Spoof** to dodge the effects of a high local mesh alarm score. Spoof works by routing all the decker's traffic through a nearby device, setting it up to look like the culprit when the authorities notice.

The decker has to have had Spoof loaded before the first hack begun, and kept it loaded throughout. Whenever Spoof is unloaded, the local mesh alarm value immediately halves (rounded down).

Spoof doesn't help with host hacking.