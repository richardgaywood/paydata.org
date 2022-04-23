
---
title: Furious Hacking in our Sprawlrunners
linkTitle: Furious Hacking
type: docs
description: Draft proposal for integrating ManuFS's Furious Hacking rules into our game
date: 2022-04-23
weight: 1000
draft: true
---

{{% pageinfo %}}Draft proposal for using [Furious Hacking](https://www.drivethrurpg.com/m/product/394371) in our Sprawlrunners game.

**NOT CURRENTLY CANON**{{% /pageinfo %}}

## Overview

Furious Hacking (FH) presents a new set of streamlined rules for host hacks in a cyberpunk game setting. It is faster to resolve that Sprawlunner's "Slow Burn" hacking rules, but offers a more dynamic and exciting difficulty ramping mechanic than the "Fast Lane" hacking option.

As written, FH covers a 'classic' no-wireless cyberpunk scenario of an operator hacking into a computer host. It doesn't cover a few scenarios that we use at our table for wireless hacking, tactical use of hacking in combat, and so forth. This document presents some ideas for expanding FH to cover those.

## Proposed modifications

### Hacking into hosts/systems

All aspects of hacking into hosts can be run as per FH. As in my existing rules, hacking into hosts is always undertaken in VR, and the operator's body is consequently in ragdoll mode.

#### Host/system active defences

Particularly valuable hosts might have, as a last line of defence, either a metahuman counter-hacker or nearline-sapient Black ICE. These are always played as Wild Cards and will attack the intruding operator in cybercombat.

{{% alert title="TODO" color="warning" %}}Define how/when these get deployed in terms of the FH mechanics. Escalating chance based on the number of the card drawn for failure perhaps?{{% /alert %}}

### Device hacking on the local mesh

The wireless Matrix is divided into cells. Within each cell, devices use peer-to-peer connections to pass traffic around; this is called the _local mesh_. At the centre of each cell is an uplink host that is actively guarded by GOD counter-hackers. Hackers are free to attempt hacks against any devices within the local mesh, but hacks agains the uplink host are widely regarded as suicide. This means hackers must always be within local mesh range of their targets.

Treat each cell as its own system, per the FH rules. This represents a combination of anti-malware scanning by the devices within the mesh as well as traffic inspection from the uplink host.

For the purposes of determining slice rolls, treat the local mesh as a system of d4 to d8 value (ie. blue, green, or orange). Blue would apply in poor neighbourhoods, where the devices are cheap and GOD are not watching; orange would be downtown where people are carrying fancy commlinks and GOD are ever-vigilant. In the slums, also apply the "lax security" modifier (+2 slice rolls); in corporate facilities, the "extra tight" modifier will probably apply (-2 slice rolls.)

When determining the actual opposing dice type for any roll, however, consider the device being hacked. A fancy commlink does not become easier to hack because the owner has travelled into the slums; it still opposes with d8 rather than d4. But slice rolls work against it as usual, as they are a function of the local mesh network working as a whole noticing the hacker's nefarious actions.

Apart from that, all normal FH rules apply, including slice rolls, opposed rolls, and card draws to determine consequences of failure. 

As in my existing rules, all local mesh hacking is carried out in AR.

The Exotic Utilities Edge (reduces the multi-action penalty) does not apply to any hacks done in AR. You're still limited by your meatspace reflexes.

### Networks

Networks are ways for operators to use their 'deck to construct secure areas on the local mesh. Each device inside the network severs its connection to the local mesh, communicating only with the cyberdeck. The cyberdeck inspects and patrols all traffic to and from the device, sheltering it from hacking attacks.

Devices inside a network cannot be hacked (but they are vulnerable to DoS attacks; see below.) A hostile decker's only option is to take the network down first, either by engaging the decker in cybercombat and crashing their deck, or by meatspace means - a bullet in the cyberdeck is a popular choice...

Maintaining a local network uses a portion of the cyberdeck's power and the operator's attention. The network will disconnect if the operator enters VR. This also means networks are limited in size, typically to only a dozen or so devices. It is not practical for even very secure corp facilities to have all their security cameras hooked into a network.

Networks only apply on the local mesh and for AR hacking. 

### Cybercombat

*Cybercombat* is any operator-vs-operator or operator-vs-Black ICE combat. Cybercombat can take place in VR or AR.

Treat cybercombat as similarly to melee combat in SWADE. 

Give each deck a die type rating, depending on the decker's Edge rank; Deck Builder = d6, Deck Optimiser = d8, Deck Customizer = d10.

* Attack actions roll Hacking skill.
* _Firewall_ ('cyberspace parry') is 1/2 the operator's Hacking skill, +2
* _Integrity_ ('cyberspace toughness') is equal to 1/2 the deck's die type, +2
* Damage is equal to the deck's die type plus the operator's Smarts.
* Some meatspace actions also apply in cybercombat, such as:
	* Defend (+4 to Integrity, cannot take any actions)
	* Ganging Up
	* Wild Attacks (+2 to Hacking, but becomes Vulnerable)
	* ...more...
* If an operator attempts a graceful logoff, their opponent gets an immediate Free Attack, similarly to withdrawing from combat in meatspace. Alternatively, they can yank the cable from their deck, avoid the Free Attack, but will take Fatigue as usual from dumpshock.

{{% alert title="TODO" color="warning" %}}Game out the integrity/damage scores to check balance.{{% /alert %}} 

Resolve damage to determine Shaken and Wounds as usual. 

When operators fight each other, each Wound is only applied to their respective cyberdecks. When operators fight Black ICE, the Wounds are applied to the deck _and the operator_. 

{{% alert title="TODO" color="warning" %}}Some room here to allow the use of LP to purchase utilities to expand the deck, eg: do extra damage, have extra toughness, gain the ability to use Edges like Frenzy, Counterattack, First Strike, lots of others...{{% /alert %}} 


### Denial of service (DoS)



DoS attacks involve a hacker flooding someone's electronic and cybernetic systems with bad traffic, jamming up their responses.

DoS is resolved as a Test action, pitting the operator's Hacking skill versus the Smarts of the target. 



### Tacnets

{{% alert title="TODO" color="warning" %}}Might drop this concept entirely.{{% /alert %}} 



