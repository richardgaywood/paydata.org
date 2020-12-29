
---
title: Additional rules
linkTitle: Additional rules
type: docs
description: Extra bits and pieces; hacking via back doors; new utilities
date: 2020-11-27
lastmod: 2020-12-29
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

## Maintaining access to a hacked node from AR

Suppose a decker has hacked into a building facility's security node in VR and now wish to move with the team while maintaining that access.

They can do so via a new utility called **KeepAlive**. This allows the decker to switch to AR while keeping their matrix presence active. They can carry out actions against whichever node they are in as if they were still in VR, although they cannot move to other nodes without logging back in.

The decker has to keep KeepAlive in their deck's memory to maintain the access. In addition, while running KeepAlive, the decker cannot act promptly to defend themselves; all ICE take +2 on all rolls against the decker.

## Reducing the local mesh alarm score

Deckers can use a new utility called **Spoof** to dodge the effects of a high local mesh alarm score. Spoof works by routing all the decker's traffic through a nearby device, setting it up to look like the culprit when the authorities notice.

The decker has to have had Spoof loaded before the first hack begun, and kept it loaded throughout. When Spoof is unloaded, the local mesh alarm value immediately halves (rounded down).

Spoof doesn't help with host hacking.

## Tacnets

A tacnet is a realtime augmented reality overlay used by all members of a team to co-ordinate their actions and share tactical data. Tacnets were created for us by elite corp special-ops teams, but have been co-opted by shadowrunners and other criminals (at least, those who can afford them.)

Tacnets can only be run by a decker using a cyberdeck. They require an s-PAN, and they require the hosting cyberdeck to be running the **Tacnet** utility.

### Game effects of tacnets

Tacnets extent the Command Range for all Leadership edges to include everyone using it (see SWADE pg 44).

If anyone on the tacnet has a Battle skill of d8 or more, the tacnet itself also gains a Bennie pool with 1 Bennie in it. This can be spent by anyone attached to the tacnet if they have no Bennies of their own left (ie the shared pool is used last.) It refreshes at the same time as other player pools, and receives a bonus Bennie if any user of the tacnet draws a Joker action card.

All of these benefits are lost if the s-PAN is crashed. This makes s-PANs a priority target for Matrix attack during combat - and the deckers priority targets for physical attack.

When the NPCs are using a tacnet, they get an extra Bennie to spend. If the PCs can crash it, the GM loses **two** Bennies immediately.