---
title: Cybercombat hacking
linkTitle: Cybercombat
type: docs
description: Disregard stealth; brick devices instead
date: 2020-11-27
lastmod: 2021-03-25
weight: 500
aliases: ["sprawlrunners/deckers/cybercombat.md"]
---

The rules in [hacking]({{< relref "hacking.md" >}}) cover stealthy intrusion techniques so a decker can discreetly manipulate devices for their own ends. But if you want to take something offline right fraggin' now, what you need is cybercombat.

## Basics of cybercombat

* Attacker must have the Fighting utility loaded (or roll to improvise a replacement, as usual.)
* Roll Hacking skill against the defender's Firewall value.
* Do base damage of 1d4 + Hacking skill. +1d6 if the attack roll had a Raise.
* Compare attack damage to target Hardening.

Calculate Shaken and Wounds as usual.

## Matrix damage

### Cyberdecks

As per Sprawlrunners core. Shaken applies to the decker using the 'deck. Cyberdecks have three Wounds; if all Wounds are taken, the decker must resist dumpshock.

### Commlinks and other devices

A commlink or other device that is Shaken is put into a crashed state. Starting on the next turn, it can attempt to restart itself (on the owner's turn, but not costing the owner an action) by making an unshake roll using the device's rating die type. Until it does so, it is offline, cannot function, and cannot be targeted for further Matrix attacks. The owner/controller of a Shaken device can choose to immediately restart it as an action without needing to pass any test.

If the device takes a Wound (via a raise on the attack roll) then they are bricked. They do not function again until repaired.

If the commlink that is running a PAN becomes Shaken, every device on the PAN is Shaken (and hence unusable) with it, until the commlink comes back. If it is crashed, every device on the PAN is Shaken. They can roll to unshake as usual (just roll once for all of them), but will come back as unattended devices, without the protection of the PAN.

## Consequences of crashing things

**Smartweapons** and similar gear that are Shaken can still be fired, as they have manual fallback controls, but they lose any bonuses they normally get from their electronics eg. smartgun bonuses. Note that it might be more effective for offensive deckers to use a [DoS attack]({{< relref "combat_decking.md#denial-of-service-attacks" >}}) instead.

All cyberware is controlled via direct neural shunts to the user's wetware, so crashing the cyberware's Matrix component only inhibits minor parts of its functionality; it doesn't brick it entirely. You cannot render someone's cyberlimb or wired reflexes completely inert via a cybercombat attack, although you can impede their use with a DoS attack. A few pieces of cyberware do inherently rely on Matrix connectivity to work - like implanted commlinks - and they can be crashed via cybercombat, however. 
