---
title: Overwatch, GOD & convergence
linkTitle: GOD
type: docs
date: 2020-07-19
weight: 70
description: All about the Grid's po-po
---

The Grid Overwatch Division is the Matrix police. **TODO: MORE**

## Overwatch

Overwatch is a 12-segment clock. This clock is public, ie. the decker player can see it. (Delete: baby monitor program, check OS action.)

The clock ticks up when:

* +1 on any Attack roll, success or failure
* +1 on any failed Sleaze roll
* +1 per combat turn if maintaining user access to any PANs or hosts *after* rolling any attack action or failing any sleaze action
	* increase to +2 if maintaining admin access
	* if the intrusion was via a successful Probe / Backdoor Entry, there is an additional grace period before the clock starts incrementing; see [Matrix actions]({{< relref "actions.md" >}})

The clock resets only when the deck reboots and the decker's persona logs off entirely. The decker loses all access to systems at that time, although any vulnerabilities discovered through Probe and not yet used for Backdoor Entry remain active.

Once the clock fills, GOD is alerted to the decker. A demi-GOD agent starts hunting them.

At the end of each turn, the demi-GOD rolls a number of dice equal to the clock vs a resistance from the decker of Intuition + Sleaze. If there are any net hits, the decker suffers convergence immediately. If there aren't, the number of hits rolled (not the net hits) are added to the clock, and the demi-GOD will roll again at the end of the next turn.

{{% alert title="Example" %}}
* Decker rolls 5 hits on a Probe test and carries 3 of those forward into Backdoor Entry.
* Decker rolls 4 hits on the Backdoor Entry test, and chooses admin level access.
* As long as they avoid any patrol IC, the decker can continue to ghost inside the host indefinitely.
* As soon as the decker fails a sleaze roll (eg. while avoiding the IC) or does an attack action (eg. to Data Spike the IC), GOD becomes aware of their activity. They take 1 tick to the OS clock immediately.
* 3 combat turns later (because of the 3 hits on the Probe test), GOD notices the decker's presence in the host. From now on the decker takes +2 OS per turn to maintain the admin access, plus more if they continue to fail sleaze actions or do attack actions.
{{% /alert %}} 

## Convergence

Same as RAW:

1. Persona's deck receives 12 DV of Matrix damage, resisted with Firewall + Device Rating
1. Persona is rebooted, erasing all access levels and inflicting dumpshock (6S or 6P; resisted with Willpower+Firewall; Firewall will be 0 if the <atrix damage bricked the deck)
1. Decker's physical location is traced and reported to authorities (including owners of the Host they were in, if any)

Convergence does not change if the persona is in a host or not when it happens.

## GOD & the megacorps

GOD is run by the Corporate Court and staffed by loaned headcount from all the AAA megacorps. Despite that, the corps do not completely trust it. They worry about a demi-GOD who is loyal to their parent corp using their position to leak information back to them. (Of course, they also attempt to convince their own demi-GOD agents to do the same. In practice, GOD keeps its deckers on very short leashes, so this rarely works - but not never.)

As such, the corps sometimes take measures to keep their darkest secrets outside of GOD's purview. This can include:

* Use of dark fibre connections to send traffic between sites that GOD cannot intercept or inspect. Can be used if the data itself is top secret, or simply to hide the location or existence of a secure facility that would otherwise be betrayed by its present on the Matrix.
* Refusal to alert GOD to hostile decker activity. In game terms, this means the decker does not accumulate OS for hacking attempts in the system. This is not good news for the decker in question, however. It means they are on dangerous ground that will be ruthlessly patrolled by novahot spiders and the blackest of IC.