---
title: Initiative and determining the number of actions
linkTitle: Initiative
date: 2020-07-05
type: docs
weight: 50
---

{{% pageinfo %}} 
These rules are currently canon for my campaign.
{{% /pageinfo %}}

## The basics

Same as SR5: there are Simple and Complex actions.

A single combat turn runs like this:

*   Everyone rolls initiative, same as usual
*   Count down from highest to lowest; when a character's number comes up, they get their phase
	*   break ties with ERIC as per 5e RAW
*   When you get to 0, the turn is over. Re-roll initiative and start over at the top again[^1]

On your phase, you get 1 Complex action as usual, plus bonus Simple actions depending on your augments (see below). Complex and Simple actions can still be interchanged as usual (1 Complex = 2 Simple and vice versa.) Youir first Complex action can be used for anything, but the bonus Simple actions are locked to specific types of action, depending on where you got them from.

## Rolling for initiative

What you roll is determined by "where" your character is:

| Where 	| Roll      	|
|--------------------------------------	|----------------------	|
| In the physical world (including AR) 	| Rea + Int + 1d6      	|
| In VR, cold sim                      	| DataProc + Int + 3d6 	|
| In VR, hot sim                       	| DataProc + Int + 4d6 	|
| Astrally projecting                  	| (Int × 2) + 2d6     	|

* Physical initiative can be boosted by various sources: augmentations, spells, adept powers, combat drugs.
* Mages who aren't astrally projecting and deckers/riggers who are using AR roll physical initiative.

## How to get bonus actions

### Cyberware, adept powers, etc

This includes wired reflexes, Improved Reflexes, and other cyberware, bioware, or magical initiative augments (including spells).

*   Generally run from Rating 1-3.
*   Each rating makes the usual changes, eg +1d6 to initiative.
*   For each d6 added to initiative, the user _also_ adds 1 Simple action to the amount they can do in their phase _but_ this action can only be used on physical (meatspace) actions, not on matrix or magic.
	*   So someone with rating 2 wired reflexes can do 4x Simple actions; or 2x Complex actions; or some other combination.

{{% alert title="Example" %}}
Example: Alice (streetsam, with Wired Reflexes III) and Bob (ganger) are fighting.

*   Turn 1: Alice rolls 22 (Rea+Int+4d6), Bob rolls 8 (Rea+Int+1d6).
*   On 22, Alice has a phase. She can do 1 Complex _plus_ 3 Simple actions.  
*   On 8, Bob has a phase. Bob can do 1 Complex or 2 Simple actions.
*   Both characters now re-roll and a new turn begins.
{{% /alert %}}

### Magic actions

For every initiate grade from 1-3, mages get an extra Simple action that can only be used for magical actions (incl spellcasting, summoning, banishing, etc). This bonus applies equally in the physical world and while astrally projecting.

(Note that this means after their first initiation, a mage can summon a spirit (1 Complex) and order it (1 Simple) in a single phase.)

### Matrix actions

These depend on the decker’s or rigger’s interface mode.

*   In AR without DNI: no extra actions
*   In AR with DNI or cold-sim VR: +2 Simple actions
*   In hot-sim VR: +3 Simple actions

As above, the bonus actions received can only be used for Matrix actions. These include driving tests if the character is piloting a vehicle via AR.

### Drugs

Drugs that increase your initiative roll do not grant extra actions. However, their effect does stack with extra actions gained from other sources. So an initiated mage using Kamikaze can go earlier in the turn and still use their 2 normal simple actions and any bonus magical actions from initiating.

Obviously, combat drugs come with [other downsides]({{< relref "addiction.md" >}}) 

### Multiple competing bonus actions

No human brain can cope with the multiplicity of inputs of being active in more than one “world” at once. Hence, they can receive bonus meatspace actions, bonus matrix actions, or bonus magic actions; but only one. If they are eligible for more than one at once, through whatever combination of gear/augments/spells/etc, they can choose freely when rolling for initiative which “world” is getting their attention and hence which minor actions they will receive.


### Deferring actions




[^1]: Or keep the values same and start over without re-rolling as SR 6e does, if you prefer. I like the dynamic feel of re-rolling each turn though.
