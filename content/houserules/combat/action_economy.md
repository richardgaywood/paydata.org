---
title: "New action economy for Shadowrun 5e"
linkTitle: Action economy
date: 2020-07-05
type: docs
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
| Astrally projecting                  	| (Int × 2 ) + 2d6     	|

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

Obviously, combat drugs come with other downsides...

### Multiple competing bonus actions

No human brain can cope with the multiplicity of inputs of being active in more than one “world” at once. Hence, they can receive bonus meatspace actions, bonus matrix actions, or bonus magic actions; but only one. If they are eligible for more than one at once, through whatever combination of gear/augments/spells/etc, they can choose freely when rolling for initiative which “world” is getting their attention and hence which minor actions they will receive.

## Deferring actions & interrupt actions

Interrupt actions no longer change your initiative score by -5 or -10 when taken. Instead:

*   A character may save any number of actions unused from their phase
*   These may be used at any point before or during their next phase
*   They can save them to use defensively (eg Parry) or take an action later for tactical reasons
*   The deferred action cannot be held any longer than whenever their next phase is
*   If they are still holding a deferred action when their next phase arrives, they can use it as part of that phase
*   No character can take any defensive actions on the first combat turn before their first phase 

{{% alert title="Example" %}}
Example: Alice (streetsam) and Bob (ganger) are still fighting.

*   Turn 1: Alice rolls 22, Bob rolls 8.
*   On 22, Alice uses one Simple Action to ready her katana. She saves the other Simple Action.
*   On 8. Bob tries to punch Alice (Complex Action.)
	*   Alice can use her saved Simple Action to add to her defence via Parry.
	*   Or she can take the hit.
*   Turn 2: Alice rolls 18, Bob rolls 7.
*   On 18, Alice now has her normal 2x Simple or 1x Complex action, and if she didn’t Parry earlier, she still has that Simple action saved up too. She attacks Bob. 
	*   Note that Bob cannot use Parry, as he does not have any Simple Actions saved up.
{{% /alert %}}

## New and changed actions

### Attacks

All the attacks from the SR5e CRB become Complex actions (but see “New Multiple Attack” below). You can now do as many attacks, during your turn, as you have actions to spend; the only exception is SS weapons, which can only be used to attack once per turn. The Long Burst Fire and SA Burst options are removed. So the attack options now are:

*   Complex actions:
	*   Fire Weapon (SS) _(only once per turn)_
	*   Fire Bow
	*   Fire Weapon (SA, BF, FA)
	*   Throw Weapon
	*   Melee Attack
	*   Quick Draw
*   Complex + variable number of Simple actions:
	*   _Carnival of Carnage_ multi-attack (full dice pool; see below)
*   Complex + Free action:
	*   Multi-attack (split dice pool)

Recoil is no longer tracked across turns, but it does apply (in total) across all the attacks done within a single turn. For example, if a character has 2x Complex actions to spend, and uses them to do 2x Fire Weapon (BF) attacks, that's 6 points of recoil that apply across both attacks. When they start their next turn, however, the recoil counter is reset.

### New multiple attack

The old multiple attack rule (use a Free Action to declare, a Complex Action to attack, split your dice pool amongst opponents) remains in place.

If the attacker has:

1. extra physical/meatspace actions and 
1. a smartlink with a DNI connection to a smartgun 

...then they can use a new type of multiple attack, _Carnival of Carnage_.  They can also perform CoC with a melee attack with any weapon, as long as they can move far enough to reach everyone.

To use CoC:

*   It requires one Complex action, plus one Simple action for each additional target in addition to the first
*   Calculate recoil according to the total number of bullets fired and apply it to each roll
	*   Eg. if using 1x Complex and 2x Simple actions to shoot three people with a burst-fire gun, it’s 9 bullets
*   Roll your full dice pool (plus modifiers) against each target
	*   (For simplicity's sake, unless the modifiers are different, just roll once and use the same number of hits against each target.)

### Mages

Remove Reckless Spellcasting (the ability to cast a spell for a Simple action at +3 drain.)

Spell defence now requires a Simple action to declare, which must be a deferred action from the mage’s last phase. However, it protects up to (Magic Rating) targets, all of whom get the mage’s full Counterspelling skill to add to their spell defence dice. This can be done as many times as the mage has actions. 

### Riggers

All the vehicle actions on CRB pg 202-203 count as Matrix actions for any character using AR or VR, and thus can be done with a rigger’s bonus actions.

*   Fire Mounted Weapon (when it’s an electronically controlled turret)
*   Rigger Jump In
*   Make Vehicle Test (for vehicle piloting actions eg. stunts, pursuits) 

Send Message (to command drones) remains a Simple matrix action. By default, it can command one drone; if the drones are connected to a PAN centered on an RCC the user can send the same command to multiple drones for a single Simple action.

When a rigger is jumped in, Control Vehicle becomes a Free Action ie. a rigger no longer needs to spend one Complex action per turn to stop the vehicle going uncontrolled. This is only true when jumped in, and jumped in continues to require VR.

### Matrix actions

The SR5 core rulebook has 37 normal actions plus 9 magic actions. It also has 42 Matrix actions. Kill Code adds another 11. This is too many. I am working on [reducing them]({{< relref "matrix_actions.md" >}}). 

**Fork** - modify Fork to work the same as Carnival of Carnage above (1 Complex action for the first target, then +1 Simple action for each additional target.)


## Appendix: possible future changes

* **Physads:** need consideration re: the new multi attack.
* **Deckers:** some bit of gear (deck add-on? A program?) that can grant an extra +1 Simple
* **Mages:** vary the number of actions necessary to cast a spell or summon a spirit:

Like:

*   Force \< (Magic rating /2): 1 Complex
*   Force between above and below: 1 Complex + 1 Simple
*   Force \> (Magic rating): 2 Complex

Or:

<table>
  <tr>
   <td>
   </td>
   <td>
<strong>Spellcasting</strong>
   </td>
   <td><strong>Summoning</strong>
   </td>
  </tr>
  <tr>
   <td>1 Simple action
   </td>
   <td>Force &lt;= Magic/2
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>1 Complex action
   </td>
   <td>(in between above and below)
   </td>
   <td>Force &lt;= Magic/2
   </td>
  </tr>
  <tr>
   <td>1 Complex + 1 Simple
   </td>
   <td>Force > Magic
   </td>
   <td>(in between above and below)
   </td>
  </tr>
  <tr>
   <td>2 Complex
   </td>
   <td>
   </td>
   <td>Force > Magic
   </td>
  </tr>
</table>





## Appendix - reddit threads about this

*   [v0.1 release][1]
*   [v0.2 release][2]

## Appendix - worked example with my current PCs


<table>
  <tr>
   <td colspan="3" ><strong>Dancer</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>Old rules (RAW)
   </td>
   <td>Proposed new rules
   </td>
  </tr>
  <tr>
   <td>Initiative roll
   </td>
   <td>12+3d6
   </td>
   <td>12+3d6
   </td>
  </tr>
  <tr>
   <td>Phases per turn
   </td>
   <td>74% chance of 3x
<p>
26% chance of 2x
   </td>
   <td>Always 1x
   </td>
  </tr>
  <tr>
   <td>Actions per phase
   </td>
   <td>1 Complex
   </td>
   <td>1 Complex (anything)
<p>
+1 Complex (physical)
   </td>
  </tr>
  <tr>
   <td>Max attacks per turn
   </td>
   <td>2x or 3x
   </td>
   <td>3x
   </td>
  </tr>
</table>



<table>
  <tr>
   <td colspan="3" ><strong>Eddie</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>Old rules (RAW)
   </td>
   <td>Proposed new rules
   </td>
  </tr>
  <tr>
   <td>Initiative roll
   </td>
   <td>9+1d6
   </td>
   <td>9+1d6
   </td>
  </tr>
  <tr>
   <td>Phases per turn
   </td>
   <td>83% chance of 2x
<p>
17% chance of 1x
   </td>
   <td>Always 1x
   </td>
  </tr>
  <tr>
   <td>Actions per phase
   </td>
   <td>1 Complex
   </td>
   <td>1 Complex (anything)
<p>
+1 Simple (magical)
   </td>
  </tr>
</table>



<table>
  <tr>
   <td colspan="3" ><strong>Mr Atom</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>Old rules (RAW)
   </td>
   <td>Proposed new rules
   </td>
  </tr>
  <tr>
   <td>Initiative roll
   </td>
   <td>10+1d6
   </td>
   <td>10+1d6
   </td>
  </tr>
  <tr>
   <td>Phases per turn
   </td>
   <td>2x
   </td>
   <td>1x
   </td>
  </tr>
  <tr>
   <td>Actions per phase
   </td>
   <td>1 Complex
   </td>
   <td>1 Complex (anything)
   </td>
  </tr>
  <tr>
   <td>Max attacks per turn
   </td>
   <td>2x
   </td>
   <td>1x
   </td>
  </tr>
</table>



<table>
  <tr>
   <td colspan="3" ><strong>Project: Heartbreak</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>Old rules (RAW)
   </td>
   <td>Proposed new rules
   </td>
  </tr>
  <tr>
   <td>Initiative roll
   </td>
   <td>9+1d6
   </td>
   <td>9+1d6
   </td>
  </tr>
  <tr>
   <td>Phases per turn
   </td>
   <td>83% chance of 2x
<p>
17% chance of 1x
   </td>
   <td>Always 1x
   </td>
  </tr>
  <tr>
   <td>Actions per phase
   </td>
   <td>1 Complex
   </td>
   <td>1 Complex (anything)
   </td>
  </tr>
  <tr>
   <td>Max attacks per turn
   </td>
   <td>2x
   </td>
   <td>1x
   </td>
  </tr>
</table>



<table>
  <tr>
   <td colspan="3" ><strong>Twitch (physical)</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>Old rules (RAW)
   </td>
   <td>Proposed new rules
   </td>
  </tr>
  <tr>
   <td>Initiative roll
   </td>
   <td>14+3d6
   </td>
   <td>14+3d6
   </td>
  </tr>
  <tr>
   <td>Phases per turn
   </td>
   <td>0.5% chance of 4x
<p>
83.3% chance of 3x
<p>
16.2% chance of 1x
   </td>
   <td>Always 1x
   </td>
  </tr>
  <tr>
   <td>Actions per phase
   </td>
   <td>1 Complex
   </td>
   <td>1 Complex (anything)
<p>
1 Complex (physical)
   </td>
  </tr>
  <tr>
   <td>Max attacks per turn
   </td>
   <td>2x - 4x
   </td>
   <td>4x
   </td>
  </tr>
  <tr>
   <td colspan="3" ><strong>Twitch (matrix AR DNI / VR cold sim)</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>Old rules (RAW)
   </td>
   <td>Proposed new rules
   </td>
  </tr>
  <tr>
   <td>Initiative roll
   </td>
   <td>14+3d6
   </td>
   <td>DataProc+6+1d6
   </td>
  </tr>
  <tr>
   <td>Phases per turn
   </td>
   <td>0.5% chance of 4x
<p>
83.3% chance of 3x
<p>
16.2% chance of 2x
   </td>
   <td>Always 1x
   </td>
  </tr>
  <tr>
   <td>Actions per phase
   </td>
   <td>1 Complex
   </td>
   <td>1 Complex (anything)
<p>
1 Complex (Matrix)
   </td>
  </tr>
  <tr>
   <td>Max attacks per turn
   </td>
   <td>2x - 4x
   </td>
   <td>
   </td>
  </tr>
</table>


## Footnote: Design goals

With the exception of 4e, Shadowrun has always tightly coupled together two concepts: how soon in a turn a character acts (their initiative roll) and how much they can get done in a turn (how many passes they get.) This document aims to explore what happens if we decouple these and allow them to vary independently under some combinations of character abilities.

Other goals:

*   Give AR deckers and riggers an easier time of it- so they can get out the car/van and come along on the run without worrying that their floppy meatbods will get hurt while they are in VR because that’s the only way to get a good action economy.
*   Make streetsams/physads more distinctive by giving them combat powers other archetypes cannot access.
*   Simplify handling initiative at the table: 
	*   Don’t change initiative score mid-turn.
	*   Remove multiple passes.
	*   Remove the need to track recoil across subsequent turns without making it meaningless.

## Notes

[^1]:

	 Or keep the values same and start over without re-rolling as SR 6e does; it’s not a big deal.

[1]:	https://www.reddit.com/r/Shadowrun/comments/gzuxd0/musings_on_a_new_action_economy_for_shadowrun/
[2]:	https://www.reddit.com/r/Shadowrun/comments/hheghk/houserules_for_a_streamlined_initiative_system_5e/