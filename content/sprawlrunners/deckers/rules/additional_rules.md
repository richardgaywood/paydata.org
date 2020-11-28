
---
title: Additional rules
linkTitle: Additional rules
type: docs
description: Extra bits and pieces; hacking via back doors; new utilities
date: 2020-11-27
weight: 800
---

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