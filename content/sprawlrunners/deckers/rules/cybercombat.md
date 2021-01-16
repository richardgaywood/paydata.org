---
title: Cybercombat
linkTitle: Cybercombat
type: docs
description: Disregard stealth; brick devices instead
date: 2020-11-27
weight: 500
---

The rules in [hacking]({{< relref "hacking.md" >}}) cover stealthy intrusion techniques so a decker can discreetly manipulate devices for their own ends. But if you want to take something offline right fraggin' now, what you need is cybercombat.

## Basics of cybercombat

* Attacker must have the Fighting utility loaded (or roll to improvise a replacement, as usual.)
* Roll Hacking skill against the defender's Parry value, calculated as:
	* Cyberdeck with Fighting utility: (1/2 the user's Hacking skill) + 2.
	* Cyberdeck without Fighting utility: 2
	* Commlink or standalone device: 2
	* ICE: (1/2 the host rating) + 2
* Do base damage of 1d4 + Hacking skill. +1d6 if the attack roll had a Raise.
* Compare attack damage to target Firewall, calculated as:
	* Cyberdeck - intrinsic stat depending on 'deck rating
	* Commlink or standalone device: (1/2 the device rating)
	* ICE: (1/2 the host rating)

Calculate Shaken and Wounds as usual.

## Matrix damage

### Cyberdecks

As per Sprawlrunners core. Shaken applies to the decker using the 'deck. Cyberdecks have three Wounds; if all Wounds are taken, the decker must resist dumpshock.

### Commlinks and other devices

A commlink or other device that is Shaken is put into a crashed state. Starting on the next turn, it can attempt to restart itself (on the owner's turn, but not costing the owner an action) by making an unshake roll using the device's rating die type. Until it does so, it is offline, cannot function, and cannot be targeted for further Matrix attacks. The owner/controller of a Shaken device can choose to immediately restart it as an action without needing to pass any test.

If the device takes a Wound (via a raise on the attack roll) then they are bricked. They do not function again until repaired.

If the commlink that is running a PAN is Shaken, every device on the PAN is Shaken (and hence unusable) with it, until the commlink comes back. If it is crashed, every device on the PAN is Shaken. They can roll to unshake as usual (just roll once for all of them), but will come back as standalone devices, without the protection of the PAN.

## Consequences of crashing things

**Smartweapons** and similar gear that are Shaken can still be fired, as they have manual fallback controls, but they lose any bonuses they normally get from their electronics eg. smartgun bonuses. Note that it might be more effective for offensive deckers to use a [DoS attack]({{< relref "combat_decking.md#denial-of-service-attacks" >}}) instead.

Similarly, if you disrupt the Matrix component of a **vehicle**, then the autopilot and navigation is disrupted, but the occupants can still use manual controls to drive it. If they don't, then a backup failsafe will attempt to bring it to a safe halt.