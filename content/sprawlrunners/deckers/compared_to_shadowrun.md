---
title: Comparing these houserules to Shadowrun 5e/6e
linkTitle: Compared to SR
type: docs
description: A quick list of the simplifying assumptions I have made
date: 2020-11-29
weight: 1000
---

These rules attempt to simplify the Shadowrun 5e Matrix rules by removing a number of options. For quick reference, some of the changes I have made include:

* Streamline and merge the "AR / VR" and "in host / on grid" distinctions. Now, being "in" a host means always being in VR, and if you're not in a host then you are in AR.
* Split the Matrix into two parts; a localised, short-range, wireless mesh network and a global, wired network. Hacking is only viable on the former; the latter is ruthlessly protected by GOD agents. Thus, deckers need to be fairly close to their targets, so they can reach them via the local mesh.
* Mostly remove the concepts of personas and their associated magic unhackable digital ownership.
* Introduce a hard line between regular PANs (hosted on a commlink) and *secure PANs* (hosted on a cyberdeck or drone deck.)

## Hacking & cybercombat

* Distill all primary decker offensive actions to three kinds: *hacking* (stealthy, grants access to manipulate devices), *cybercombat* (overt, violent, crashes devices), and disruptive *quickhacks* (disrupts traffic to/from a device or PAN to impose penalties on people using it.)
* If a device is in a PAN or WAN, it cannot be hacked directly; the attacker must hack the PAN or WAN instead (this is in Shadowrun 6e, to be fair.)
* If a device is in a WAN, and the decker can get physical access to its internal debug ports, they can compromise it and get a big bonus to hacking the WAN host through it. Hence corps rarely put easily-accessed external devices like maglocks and cameras on WANs; instead, WANs are reserved for stuff like security guard gear and internal turrets and sensors. 
* Secure PANs annot be hacked; they must be crashed in cybercombat.
* Via a program on their cyberdeck, hackers who have infiltrated a host (in VR) can switch to AR (to move with the team) but maintain a connection to the host and still send hacking commands to devices attached to it. However, the persona they leave running in the host is more vulnerable to ICE.

## Wireless off / running silent / Matrix stealth

* Wireless devices are always visible on the Matrix - no running silent, and devices connected to PANs or WANs don't disappear from view on the local mesh.
* s-PANs (and only s-PANs) can be configured to hide themselves on the Matrix; they minimise traffic between their devices, cutting back to just text/voice comms. All devices are otherwise inactive and no game mechanical bonuses can be derived from them as long as the s-PAN stays in stealth mode. This is an active process that must be maintained by the decker/rigger running the s-PAN.
