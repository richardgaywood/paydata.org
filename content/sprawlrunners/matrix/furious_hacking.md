
---
title: Furious Hacking in our Sprawlrunners
linkTitle: Furious Hacking
type: docs
description: Draft proposal for integrating ManuFS's Furious Hacking rules into our game
date: 2022-04-23
weight: 1000
---

{{% pageinfo %}}Draft proposal for using [Furious Hacking](https://www.drivethrurpg.com/m/product/394371) in our Sprawlrunners game.

**NOT CURRENTLY CANON**{{% /pageinfo %}}

## Overview

Furious Hacking (FH) presents a new set of streamlined rules for host hacks in a cyberpunk game setting. It is faster to resolve that Sprawlunner's "Slow Burn" hacking rules, but offers a more dynamic and exciting difficulty ramping mechanic than the "Fast Lane" hacking option.

As written, FH covers a 'classic' no-wireless cyberpunk scenario of an operator hacking into a computer host. It doesn't cover a few scenarios that we use at our table for wireless hacking, tactical use of hacking in combat, and so forth. This document presents some ideas for expanding FH to cover those.

## Proposed modifications

### Hacking into hosts/systems

All aspects of hacking into hosts can be run as per FH. As in my existing rules, hacking into hosts is always undertaken in VR, and the operator's body is consequently in ragdoll mode.

A hacker does not need to be physically connected to a system in order to hack it; they only need to be within local mesh range (see below). 

Note that wireless Matrix signals use high-frequency ultrawideband radio, and so very easy to block via physical means. Many secure corporate facilities will therefore use embedded Faraday caging in their construction to limit the size of the local mesh to their walls, making them very difficult to hack from outside the perimeter. This is expensive, however, as it means they will then need to run all building facilities via an on-premises system as well as running their own private uplink system.

#### Host/system active defences

Particularly valuable hosts might have, as a last line of defence, either a metahuman counter-hacker or nearline-sapient Black ICE. These are always played as Wild Cards and will attack the intruding operator in cybercombat.

{{% alert title="TODO" color="warning" %}}Define how/when these get deployed in terms of the FH mechanics. Escalating chance based on the number of the card drawn for failure perhaps?{{% /alert %}}

#### Keepalive

Once a hacker has logged in to a system, they can disconnect from VR, switch to AR, but maintain their persona's presence in the host. From there, they can continue to issue "control a device" commands to the system. These use slice rolls as usual.

While running under keepalive, the operator cannot benefit from the Exotic Utilites Edge, as they are limited by their meatspace reflexes. Nor can they use more complex Matrix actions like finding or manipulating information, or manipulating an entire subsystem.

Keepalive allows a hacker to move with the team through a facility, dealing with security measures as they do, without having to constantly dip into and out of VR.

#### Backdoors

A hacker can work more effectively inside a system if they can get physical access to a trusted device. If they can crack the device open and improvise a connection to it's debug ports, they can exploit it's trusted status.

To do this, they'll need an electronics kit, a suitable device (a commlink, camera, almost anything that is connected), some time, and a successful roll of Electronics. If the device is also armoured against physical attack, a roll of Repair may also be necessary to get into the guts of it without damaging the delicate components within.

If the operator succeeds in this, they gain a bonus +2 slice rolls, the same as if they had pre-existing security grade credentials on the system.

### Device hacking on the local mesh

The wireless Matrix is divided into cells. Within each cell, devices use peer-to-peer connections to pass traffic around; this is called the _local mesh_. At the centre of each cell is an uplink host that is actively guarded by GOD counter-hackers. All traffic between devices in different cells pass through the uplink host.

Hackers are free to attempt hacks against any devices within their local mesh, but hacks against or through the uplink host are widely regarded as suicide. This means hackers must always be within local mesh range of their targets.

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

#### Hiding a network

The operator running a network can choose to minimise and disguise all traffic within it, effectively making the constituent devices disappear from the Matrix. 

This requires active monitoring from the operator, and in combat, one action each round must be spent maintaining the stealth. This means combining it with any other actions will result in a multi-action penalty, as usual.

Noticing a hidden network involves a roll of the operator's Hacking skill. The observer must have some sort of running AR system for this. If the observer is  a counter-operator using a cyberdeck, they can oppose the Hacking roll with their Notice skill. If they are just normal schlubs with commlinks, the Hacking roll is unopposed.

Hiding is not used in VR/systems. It only applies in AR/meatspace.

### Cybercombat

*Cybercombat* is any operator-vs-operator or operator-vs-Black ICE combat. Cybercombat can take place in VR or AR.

Treat cybercombat as similarly to melee combat in SWADE. 

Give each deck a die type rating, depending on the decker's Edge rank; Deck Builder = d6, Deck Optimiser = d8, Deck Customizer = d10.

* Attack actions roll Hacking skill.
* _Firewall_ ('cyberspace parry') is 1/2 the operator's Hacking skill, +2
* _Integrity_ ('cyberspace toughness') is equal to 1/2 the deck's die type, +2
* Damage is equal to the deck's die type plus the operator's Smarts. +1d6 if the attack was a Raise, as usual.
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

Almost all electronic devices and cybernetic systems maintain a connection to the Matrix for secondary functions, diagnostic reporting, and similar. Hackers cannot disrupt the primary interface or functionality of a device; they cannot turn off someone's cybereyes, prevent a smartgun from firing, or remotely detonate a grenade on someone's belt.

What they can do is a _Denial of Service attack_. DoS attacks involve a hacker flooding someone's electronic and cybernetic systems with bad traffic, jamming up their responses and making them glitchy and unreliable.

DoS is resolved as a Test action, pitting the operator's Hacking skill versus the Smarts of the target. The operator takes -2 to +2, depending on the number of electronic devices the target has. Resolve Distracted/Vulnerable/Shaken outcomes as usual.

{{% alert title="TODO" color="warning" %}}Perhaps some Edges or LP-based gear here? I am tempted to add an AoE option.{{% /alert %}}

### Tacnets

{{% alert title="TODO" color="warning" %}}Might drop this concept entirely.{{% /alert %}} 



