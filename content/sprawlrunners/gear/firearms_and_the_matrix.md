---
title: "Firearms and the Matrix"
linkTitle: "Guns & the IoT"
description: How modern firearms interact with the Matrix
type: docs
weight: 450
date: 2021-04-21
---

Unless otherwise stipulated, all normal firearms in the game are assumed to be "modern", for a 207x version of the word "modern." This means they have:

* caseless ammo
* electronic firing mechanism
* electronic trigger
* wireless mental controls for fire mode selection
* a backup (fully mechanical) trigger & firing mechanism
* internal sensor package that enables the gun to track its state and display it to the user via an AR holo display (eg. ammo count, current fire mode, barrel temperature, warnings about maintenance schedule)
* optional extra (for more ¥) - friend-or-foe ID system [^1]
* optional extra (for more ¥) - biometric-based safeties
* optional extra (for more ¥) - active gas-vent recoil reduction systems, that use the gun's onboard processing to compute the best way to use weapon exhaust gases to compensate for barrel climb in realtime
* "squealer" tags that broadcast the presence of the gun on the Matrix, and track the gun's legal owner (more on these below); also, the same applies to ammo

[^1] Notoriously finicky, and infamous amongst security personnel for occasional false-positives that stop them shooting people they really, really need to shoot. Widely hated. Corp execs keep insisting on them, though, because they're micromanaging arseholes. 

### Illegal guns

Any gun the PCs purchase with Logistic Points has been supplied to them through criminal contacts that have already wiped the gun. Squealer tags are disabled (but can be re-enabled if it is helpful for disguise reasons), all other RFID tracking features are disabled, any present biometric safeties or friend-or-foe ID system are removed.

### Squealer tags

If you have a [normal open-carry firearms licence]({{< relref "sins_and_licences.md" >}}), then you are required to have a broadcasting tag on your gun at all times. This tells everyone who cares to know that you are armed.

If you have a concealed carry licence, you are legally permitted to disable this broadcast. Criminals routinely do this on their guns, too, for obvious reasons. 

If a cop or a guard spots a gun poking out of your clothes and you *don't* have a squealer tag running, they are going to be intensely curious about you. For this reason, even criminals sometimes turn gun broadcasts on - it can, paradoxically, help you blend in better.

### Hacking modern firearms

Although modern firearms use various Matrix features, they are all secondary to the functionality of the gun, or have purely non-Matrix backup failsafes. Hence, a gun cannot be completely disabled by hacking it.

A decker who wishes to disrupt guns wielded by their enemies can, however, carry out a [Denial of Service attack]({{< relref "combat_decking.md" >}}). This follows the normal SWADE rules for a Test action.

## Smartguns

Smartguns represent the pinnacle of firearms electronic control. The gun's sensor package is extended to include LIDAR mapping and time-of-flight sensing; on-board secondary processing includes a ballistics model calibrated to the specific gun[^2]. This links to a primary processor implanted into the user's nervous system which can compute likely ballistic trajectories and overlay them onto the user's cybereyes display, providing for firing accuracy unrivalled by any other mechanism -- even from the hip.

**Houseruled game mechanics**: A smartgun can cancel up to 2 points of Shooting penalties from the same sources as an Aim action: range, cover, speed, scale and called shots. If there aren't 2 points of penalties to cancel, it grants +1 to the roll instead. 

A smartgun is required to use cyberarms with recoil compensation systems.

[^2]: This requires "sighting in" after fitting to a new weapon, similar to dialling in optical sights.

## Throwbacks

Weapons that are not modern (per the above definition) are called *throwbacks*. They have entirely mechanical firing mechanisms, use cased ammo, and have iron or optical sights only.

**Game mechanics**: Throwback guns are entirely invisible on the Matrix and cannot be hacked via Denial of Service attacks. 

Throwback guns in good condition that aren't linked to existing crimes via ballistics traces are difficult to find on the street, as is cased ammo for them. All throwback guns incur a +1 LP penalty, as does each purchase of ammo for them. Throwback ammo is only available in normal variety - no APDS or Ex-Ex.

Throwback guns cannot take certain accessories and modifications:

* Smartgun adapters
* Gas-vent recoil reduction system - relies on on-weapon processing to make realtime adjustments to accurately compensate for recoil


