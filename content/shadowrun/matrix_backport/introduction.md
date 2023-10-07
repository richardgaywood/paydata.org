---
title: Introduction
linkTitle: Introduction
type: docs
date: 2020-07-26
weight: 10
description: What I'm trying to do
categories:
  - archived
aliases: 
  - /archive/matrix_backport/introduction  
---
The SR6e ruleset contains a gently streamlined version of the Matrix rules from Shadowrun 5e; these have several useful changes that reduce book-keeping and give deckers a simpler and more agile action economy. 

Some of the changes to the Matrix rules are not compatible with the rest of SR5e: for example, the use of attack and defence ratings to distribute Edge during Matrix actions. Fortunately, it is easy to ignore those, and still use other parts of the SR6e Matrix system within SR5e. These houserules aim to do just that.

*   **Goals of doc**:
    *   To present a set of house rules for deckers in Shadowrun 5e, based on the Matrix rules in Shadowrun 6e. 
    *   Where possible, existing 5e rules from the wider system (stuff like limits, the action economy, etc) will be kept, in order to maintain compatibility with other 5e houserules, splatbooks, etc. 
*   **Non-goals**:
    *   To explicitly cover any content from splatbooks for SR5e; only CRB content is included here.
    *   To exactly reproduce 6e rules inside 5e; where I feel it necessary, I will houserule to bridge the gaps. I’ll try and call this out, though, so you know I’ve done it. 
        *   There are some subtle changes in 6e to things like which stat to roll for some actions that might just be annoying for tables that are already familiar with the 5e Matrix rules or use existing 5e Matrix rules reference material. I have mostly left these out of the first part of the document, although they are listed one-by-one in the second part.
    *   To be a 100% complete ruleset. I am not a professional RPG writer, so I’m not aiming to produce content that anyone would/should pay for. I’m going to attempt to cover 80% of the stuff and hope GMs can fill in the remaining 20% at their table. That said, if you notice any glaring holes, please tell me!
*   **Todo**: technomancers. There are none at our table, and never have been, so I haven’t looked at their rules yet. If you’d like to help out, please get in touch.

## Overview of the changes

I will ignore here the wider changes to SR6e that the decker rules fall into line with, eg. attack-rating-vs-defence-rating, Edge, and so forth. I’m concentrating on Matrix rules.

*   **Decker action economy is simplified:** mostly by making deckers able to do more with a single action and single test then they could in SR5e, where they'd often have to roll to get marks then roll again to achieve goals. This could be particularly difficult during combat, where the decker might target one opponent to get marks against, only for that opponent to be killed by other team-mates before the decker could exploit the marks. 
    *   **Hack on the Fly:** this is the stealth-orientated method for deckers to get access to things they shouldn't. In 6e, it is replaced by two separate actions: Probe[^2], which is slow but establishes backdoors, and can be done hours ahead of time. And then Backdoor Entry[^3], which exploits weaknesses found earlier by Probe to give the decker access as they need it during the run. [See more here]({{< relref "rules.md#sleaze-attacks-probe--backdoor-entry" >}}).
	*   In SR6e, **Spoof Command** can be used by a decker to send a single command to a device _without_ first getting any marks/access levels on anything. In SR5e, the decker would first need a mark on a device that can control the target device to do this. Again, this gives deckers more ability to be useful in the field and react to dynamic situations. [See more here]({{< relref "rules.md#spoof-command" >}}).
*   **Marks have been replaced by Access Levels**, which helps reduce book-keeping slightly. There are fewer access levels than there were mark levels, and they’re easier to remember. [See more here]({{< relref "rules.md##marks-change-to-access-levels" >}}).
*   **Overwatch Score (OS) accumulation is different**. Instead of getting 2d6 every 15 minutes, as happens in 5e, in 6e the decker accumulates OS as they remain connected to compromised systems or [See more here]({{< relref "rules.md#overwatch-god-convergence" >}}).
*   **Matrix damage gives penalties to dice pools** just like physical and stun damage; ie -1 per 3 boxes. This makes Data Spike deckers more dangerous, as even if they don’t do enough damage to take a device offline, they can still damage it. [See more here]({{< relref "rules.md#matrix-damage--repair-dumpshock" >}}).
*   **Grids**: in SR6e, grids no longer have any mechanical effect. They are kept only as cosmetic fluff. Every host/device is equally accessible on every grid. Players never need to hop grids to get to targets[^4].



## A note about the document structure

This section is very long, but you don't need to read most of it. 

The second and larger section - Comparing SR5e and SR6e - goes through the two systems item-by-item, and is the section I wrote first, to convince myself I understood both rulesets. This is the bulk of the section.

However this section is not needed if you just want to read the houserules. For those, you only need to read the Rule Changes section (which is a good deal shorter, at ~8 pages.)

## Discussion links

* [Reddit](https://www.reddit.com/r/Shadowrun/comments/explj3/houserules_to_use_sr6es_matrix_system_in_sr5e/)
* [Shadowrun forums](https://forums.shadowruntabletop.com/index.php?topic=30918)


[^2]: Snigger.

[^3]: Snigger. Again.

[^4]: This showed up in 5e as an optional rule in Kill Code.
