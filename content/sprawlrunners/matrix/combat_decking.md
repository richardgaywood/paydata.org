---
title: Combat decking
linkTitle: Combat decking
type: docs
description: How the decker can help in combat
date: 2021-01-16
weight: 525
aliases: ["sprawlrunners/deckers/combat_decking.md"]
---

The rise of wireless hacking has made the decker much more useful and powerful on the modern battlefield. Deckers are now key parts of combat squads, performing counter-hacking, defening against attacking deckers, hiding their team from sight on the Matrix, and running denial-of-service attacks against opposing forces.

## Denial-of-service attacks

A decker facing an opponent using wirelessly connected devices can distract them by interfering with the systems using a special form of the Test action (see SWADE pg 108), called a *DoS attack*. The decker makes a Hacking roll opposed by the target's Smarts trait. The following modifiers apply:

* If the target has a few items of cyberware and/or wireless gear: no modifier.
	* If they have lots of gear, extensive cyberware, or both: +1 to the decker's roll
	* If the target is a drone or vehicle working on autopilot: +2 to the decker's roll
* If the target's gear is protected by a network that the decker hasn't hacked: -2 to the decker's roll

On a success, the decker can inflict either Distracted or Vulnerable on the target, as they prefer. On a Raise, they can also inflict Shaken.

## Matrix stealth

As a general rule, you cannot hide on the matrix. Any smart devices - and this includes many items of gear and most items of cyberware - inherently rely on the matrix to work at all, and so anyone glancing in your direction will see the corresponding icons.

There is an exception, however. A decker or rigger running an network from their cyberdeck or dronedeck can 'hide' it by minimising traffic and disguising the devices within it as innocuous ones. 

The 'deck must be running the Stealth utility. Hiding a network is also an active, ongoing action that requires quite a bit of attention from the decker or rigger at all times. Out of combat, this takes about half their time. In combat, it takes one action per turn (so they will incur a multi-action penalty if they also wish to act.)

To attempt a successful sneak, roll Hacking against a target number of 4 (if no-one is actively looking for the network) or opposed by Smarts (if people are hunting for it.) This test will need to be repeated every so often as the situation changes.

While a network is in hidden mode, all traffic between devices is cut to the bone. It can only be used for voice and text comms; streaming video is capped to low-resolution, riggers cannot Jump In, and most electronic items are only semi-functional (eg. no smartlink or tacnet bonuses.) 

If combat starts and the network is still in stealth mode, the decker or rigger can drop the stealth and restore full functionality as a free action.

## Tacnets

A tacnet is a realtime augmented reality overlay used by all members of a team to co-ordinate their actions and share tactical data. Tacnets were created for us by elite corp special-ops teams, but have been co-opted by shadowrunners and other criminals (at least, those who can afford them.)

Tacnets can only be run by a decker using a cyberdeck. They require a network controlled by a cyberdeck, and they require the cyberdeck to be running the **Tacnet** utility.

### Game effects of tacnets

Tacnets extent the Command Range for all Leadership edges to include everyone using it (see SWADE pg 44).

<!-- If anyone on the tacnet has a Battle skill of d8 or more, the tacnet itself also gains a Bennie pool with 1 Bennie in it. This can be spent by anyone attached to the tacnet if they have no Bennies of their own left (ie the shared pool is used last.) It refreshes at the same time as other player pools, and receives a bonus Bennie if any user of the tacnet draws a Joker action card. -->

At the start of combat, the character on the tacnet with the highest Battle score can take a test. This test is at +2 if the character's have thoroughly prepared for battle and know the terrain, or -2 if the characters were ambushed. On a success, the tacnet earns an *anti-Bennie*. An anti-Bennie can be used to force one die reroll from the opposition, and the lower of the two results used.The anti-Bennie can be used by anyone on the tacnet, to force a re-roll of any action taken against them. This benefit expires at the end of the combat scene.

All of these benefits are lost if the network is crashed. This makes tacnets a priority target for Matrix attack during combat - and the deckers priority targets for physical attack.

## Maintaining access to a hacked node from AR

Suppose a decker has hacked into a building facility's security node in VR and now wish to move with the team while maintaining that access.

They can do so via a new utility called **KeepAlive**. This allows the decker to switch to AR while keeping their matrix persona active in the node. They can carry out actions against whichever node they are in as if they were still in VR, although they cannot move to other nodes without logging back in.

The decker has to keep KeepAlive in their deck's memory to maintain the access. In addition, while running KeepAlive, the decker cannot act promptly to defend themselves; all ICE take +2 on all rolls against the decker's persona.