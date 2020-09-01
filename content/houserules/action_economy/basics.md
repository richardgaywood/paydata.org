---
title: The combat turn, initiative, and bonus actions
linkTitle: The basics
description: How to figure out who goes when and what they can get done
date: 2020-07-05
type: docs
weight: 50
---

{{% pageinfo %}} 
These rules are currently canon for my campaign. Although they are a bit experimental.
{{% /pageinfo %}}

## The combat turn

Initiative time is split into a series of *turns*, with each turn representing a few seconds of in-game time. During a turn, each character gets a *phase* in which to do their actions. The order in which characters get phases is determined by the initiative roll. 

Each combat turn runs like this:

*   Everyone rolls initiative.
*   Count down from highest to lowest; when a character's number comes up, they get their phase.
	*   (Break ties with "ERIC" as per 5e RAW - compare the two characters Edge, Reaction, Intuition stats. If it's still a draw, flip a coin.)
*   During their phase, each character takes their action(s).
*   During any phase that is not theirs to act on, any character can take one Free action.
*   When you get to 0, the turn is over[^passes]. Re-roll initiative and start over at the top again[^reroll].

On their phase, everyone gets one normal Complex or two Simple actions as usual, and they might also get bonus Simple actions[^bonus] (see below). 

Complex and Simple actions can be freely interchanged as usual (one Complex = two Simple and vice versa.) 

A character's normal Complex action can be used for any type of action, but their bonus Simple actions can only be used to perform specific types of action (physical / Matrix / magical), depending on where the character got the bonus actions from.

[^reroll]: Or keep the values same and start over without re-rolling as SR 6e does, if you prefer. I like the dynamic feel of re-rolling each turn though.
[^passes]: These rules eliminate multiple passes. 
[^bonus]: These bonus actions replace the multiple passes mechanic of normal Shadowrun 5e.

## Free actions

Each character can take a Free action on any phase, including their own. They can do this as many times during the turn as there are phases.[^free]

[^free]: This restores how Free actions worked in older editions of Shadowrun. It faciliates team communications via the "speak/text/transmit phrase" option. I don't think there are any game balance consequences to speak of, but we’ll revisit this rule if I’m wrong.

## Rolling for initiative

What you roll is determined by "where" your character is:

| Where 	| Roll      	|
|--------------------------------------	|----------------------	|
| In the physical world (including AR) 	| Rea + Int + 1d6      	|
| In VR, cold sim                      	| DataProc + Int + 3d6 	|
| In VR, hot sim                       	| DataProc + Int + 4d6 	|
| Astrally projecting                  	| (Int × 2) + 2d6     	|

* Physical initiative can be boosted by various sources: augmentations, spells, adept powers, combat drugs, etc.
* For avoidance of doubt: mages who aren't astrally projecting and deckers/riggers who are using AR roll physical initiative.

## Getting bonus actions

Summary table; discussion follows below:

|                                     	|          	| Bonus actions               	|
|-------------------------------------	|----------	|----------------------	|
| Wired Reflexes / Improved Reactions (etc) 	| Rating 1 	| +1 Simple (physical) 	|
|                                     	| Rating 2 	| +2 Simple (physical) 	|
|                                     	| Rating 3 	| +3 Simple (physical) 	|
| Drugs                               	|          	| None                 	|
| AR with DNI or cold-sim VR          	|          	| +2 Simple (Matrix)   	|
| Hot-sim VR                          	|          	| +3 Simple (Matrix)   	|
| Initiated magician                  	| Grade 1  	| +1 Simple (magic)    	|
|                                     	| Grade 2  	| +2 Simple (magic)    	|
|                                     	| Grade 3  	| +3 Simple (magic)     	|


Note that no metahuman brain can cope with the multiplicity of inputs of being active in more than one “world” at once. Hence, characters can receive bonus meatspace actions, bonus matrix actions, or bonus magic actions; but only one. If they are eligible for more than one at once, through whatever combination of gear/augments/spells/etc, they can choose freely when rolling for initiative which “world” is getting their attention and hence which bonus minor actions they will receive.

### Physical actions

Characters can receive bonus physical actions via any sort of normal initiative augmentation: this includes wired reflexes, Improved Reflexes adept powers, and other cyberware, bioware, or magical initiative augments (including spells like Increase Reflexes). But not drugs; see below.

*   They generally run from Rating 1-3.
*   Each rating makes the usual changes, eg +1d6 to initiative.
*   For each d6 added to initiative, the user _also_ adds 1 Simple action to the amount they can do in their phase _but_ this action can only be used on physical (meatspace) actions, not on Matrix or magic.
	*   So someone with rating 2 wired reflexes can do 4x Simple actions; or 2x Complex actions; or some other combination.

{{% alert title="Example" %}}
Example: Alice (streetsam, with Wired Reflexes III) and Bob (ganger) are fighting.

*   Turn 1: Alice rolls 22 (Rea+Int+4d6), Bob rolls 8 (Rea+Int+1d6).
*   On 22, Alice has a phase. She can do one Complex _plus_ three Simple actions, or some other combination (eg two Complex plus one Simple action).  
*   On 8, Bob has a phase. Bob can do one Complex or two Simple actions.
*   Both characters now re-roll and a new turn begins.
{{% /alert %}}

### Magic actions

For every initiate grade from 1-3, mages get an extra Simple action that can only be used for magical actions (incl spellcasting, summoning, banishing, etc). This bonus applies equally in the physical world and while astrally projecting.

(Note that this means after their first initiation, a mage can summon a spirit (Complex action) and order it (Simple action) in a single phase.)

### Matrix actions

Bonus Matrix actions depend on the decker’s or rigger’s interface mode.

*   In AR without DNI: no extra actions
*   In AR with DNI or cold-sim VR: +2 Simple actions
*   In hot-sim VR: +3 Simple actions

As usual, the bonus actions received can only be used for Matrix actions. These include driving tests if the character is piloting a vehicle via AR.

### Drugs

Drugs that increase your initiative roll do *not* grant extra actions. However, their effect does stack with extra actions gained from other sources. So an initiated mage using Kamikaze can go earlier in the turn and still use their normal Complex action and any bonus magical actions from initiating.

Obviously, combat drugs come with [other downsides]({{< relref "addiction.md" >}}).
