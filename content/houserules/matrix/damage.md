---
title: Matrix damage and how to fix it
linkTitle: Damage
type: docs
draft: true
date: 2020-07-31
weight: 31
description: Various kinds of Matrix damage, link-locking, biofeedback, etc
---

## Matrix damage

* Each device has (Device Rating / 2) boxes of Matrix damage.
* Matrix damage is resisted with Device Rating + Firewall.
* Tests using the device take a -1 penalty per 3 boxes of incurred Matrix damage.
* If the Matrix damage track fills, the device is bricked, and is non-operable until repaired.

{{% alert title="Notes" %}}
*Like 6e, but unlike 5e, I am applying penalties for Matrix damage.*
{{% /alert %}} 

### Repairing Matrix damage

* Base time of 60 minutes
* Hardware + Logic \[Mental\] test
* Split hits between reducing time and doing repair
	* Divide base time by number of hits spend to reduce time
	* Repair number of boxes of Matrix damage equal to hits spent doing repair

## Biofeedback

* In AR via goggles/glasses/image link: no effect
* Stun damage if in AR with DNI or cold-sim VR
* Physical damage if in hot-sim VR
* Resisted with Willpower + Firewall

{{% alert title="Notes" %}}
*Unlike RAW, biofeedback can affect AR users also if they are using DNI. I have made this change because my houserules make AR generally more powerful, so the risks should be greater to compensate.*
{{% /alert %}}

## Dumpshock

* In AR via goggles/glasses/image link: no effect
* If in AR with DNI or in cold-sim VR: 6S
* If in hot-sim VR: 6P
* Resisted with Willpower+Firewall
	* If the deck just got bricked, Firewall will be 0
* -2 dice on all actions for next (10-Willpower) minutes

{{% alert title="Notes" %}}
*My [action economy changes]({{< relref "action_economy.md" >}}) put AR with DNI on a similar footing to cold-sim VR. Hence, I have also made it equally vulnerable to dumpshock and link-locking. This also makes sense to me from an in-game perspective as both access modes are based on DNI.*
{{% /alert %}} 

## Link-locking

* Can affect any user in AR with DNI, cold-sim VR, or hot-sim VR
* While locked, cannot use Switch Interface, Enter/Exit Host, or Reboot
* Can take Jack Out action but with an opposed test
	* Hardware + Willpower \[Firewall\] vs Logic + Attack
	* Will take dumpshock if succeed