---
title: Physical actions
linkTitle: Physical actions
description: Actions done in meatspace
date: 2020-08-30
type: docs
weight: 100
aliases: ["/houserules/action_economy/physical_actions"]
---


## Misc

* Speak/text/transmit phrase (Free)
* Observe in detail (Simple)
* Use skill (Complex)

## Movement

Characters move at different rates, measured in the number of metres they travel during their phase.

* **Crawling** (no action used) - prone characters can crawl up to 2 metres.
* **Walking** (no action used) - all characters can walk up to 5 metres[^walking] in their phase without using any actions or taking any penalties.
* **Running** (Free) - characters can quicken their pace to a run by spending a Free action. This lets them move 10+(Agi×2) metres. They will take a -2 penalty to almost all actions they do during the phase, though. (However, note it becomes a +2 bonus to melee combat; this is the 'charging in' modifier.)
* **Sprinting** (Complex) - characters may travel even faster by spending a Complex action to make a sprinting test (Running + Strength [Physical]). For every hit on this test, most metatypes can travel a further 2 metres than their running distance. Dwarves can only travel 1 metre further per hit, however. They will continue to take a -2 penalty, as for running.

[^walking]: This is deliberately a fair bit less than RAW for many characters. My table plays theatre-of-the-mind and we hardly ever have accurate grids during combat. So I wanted there to be a clearer difference between 'walking' and 'running' rates.

### Take cover (Simple) 

Assuming there is some nearby suitable object, this grants the in cover bonus (+2 or +4 to defence rolls) until the character moves again. Note they might get flanked, though.

### Drop prone (Free) / Stand up (Simple)

Drop to the ground or get back up again[^standup].

[^standup]: I have removed the requirement to pass a test to stand up if the character is wounded.

## Gear

* Drop object (Free)
* Pick up / put down object (Simple)
* Use simple device - includes pressing buttons, turning something on or off, ejecting a weapon clip, changing a weapon's fire mode, etc.
  * with DNI (Free)
  * without DNI (Simple)

## Weapons

* Ready weapon [^readyweapon]
	* Pistol w/ slide or quick draw holster (Free)
	* Handgun (up to SMG) or short melee/thrown weapon (Simple)
	* Long gun, sword, bow, etc (Complex)
* Insert clip (Simple)
* Reload non-clip weapon (special)

[^readyweapon]: This is changed from RAW; I have removed the Quick Draw action and instead made quick draw holsters a Free action. Larger weapons become a Complex action rather than a Simple to ready up.

## Attacking related

* Call a shot (Free)
* Take Aim (special) (**TODO**)
* Attack (Complex) (see below)
* Declare split multiple attack (Free)
* Carnival of Carnage (special) (see below)

### Attacks

You can do as many attacks, during your turn, as you have actions to spend; the only exception is for single-shot (SS) weapons, which can only be used to attack once per turn[^dual-wield].

[^dual-wield]: Although you can dual-wield them and attack once per turn per weapon, if you wish.

*   Complex action:
	*   Fire Weapon (SS) _(only once per turn)_
	*   Fire Bow
	*   Fire Weapon (SA, BF, FA)
	*   Throw Weapon
	*   Melee Attack
*   Complex + Free action:
	*   Multi-attack (split dice pool - as per 5e CRB)
*   Complex + variable number of Simple actions:
	*   _Carnival of Carnage_ multi-attack (full dice pool; see below)[^coc]

[^coc]: Shoutout to the rad action movie RPG Feng Shui, from whence I stole this name.

**Recoil** is no longer tracked across turns, but it does apply (in total) across all the attacks done within a single phase.

{{% alert title="Recoil example" %}}
Alice has two Complex actions to spend, and uses them to do two Fire Weapon (BF) attacks, so that's 6 points of recoil that applies across both of her attacks. If she has four points of Recoil Compensation, she takes a net -2 penalty on *both* attacks. However, when she starts her next turn, the recoil counter is reset.
{{% /alert %}}

### Carnival of Carnage 

If the attacker has either:

1. a ranged weapon *and*
1. extra physical/meatspace actions *and* 
1. a smartlink with a DNI connection to a smartgun 

or:

1. a melee weapon *and*
1. multiple targets within movement range

...then they can use a new type of multiple attack, _Carnival of Carnage_. 

To use CoC:

*   It requires one Complex action, plus one Simple action for each additional target in addition to the first.
*   Calculate recoil according to the total number of bullets fired and apply it to each roll.
	*   Eg. if using one Complex and two Simple actions to shoot three people with a burst-fire gun, it’s 9 bullets.
*   Roll your full dice pool (plus modifiers) against each target.
	*   (For simplicity's sake, unless the modifiers are different, just roll once and use the same number of hits against each target.)
* Resolve damage against each target as usual.

Note that you *cannot* use Carnival of Carnage to attack one target multiple times.