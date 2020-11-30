---
title: Combat
linkTitle: Combat
type: docs
date: 2020-11-29
weight: 200
---

## Actions

* Initiative is determined by card draw. Some Edges let you manipulate this.
* On your go, you can perform a few free actions and one normal action. Multiple free actions can be combined only if they can reasonably be done at the same time in real life, eg. speaking a sentence and drawing a gun while dropping prone.
* If you are shaken, you first attempt to unshake as a free action.
* Free actions:
	* Move up to your Pace stat (without penalty). (NB: -1 to Pace stat per Wound taken.)
	* Run up to your Pace stat + Running die (at -2 penalty to all other actions during this turn)
	* Speak a couple of sentences
	* Drop prone
	* Drop an item
	* Ready up to two weapons or other items, as long as they are not in awkward positions eg. ankle holsters.
* Normal actions:
  * Attacking
  * Aiming (special rules apply; see SWADE pg 97)
	* Supporting allies
	* Testing foes
	* Using a power
* Can do **multi actions**: more than one action on your turn.
	* If you do two actions: take -2 to both.
	* If you do three actions: take -4 to all three.
	* Some Edges and cyberware modify these penalties.

## Combat basics

1. Attacker rolls Shooting skill vs target number 4 (for ranged combat) or defender's Parry score (for melee combat).
2. Roll damage for the weapon type. Ranged weapons are fixed; armed melee are weapon + Strength state; unarmed is just Strength (some Edges increase that).
3. If damage < target Toughness, nothing happens.
4. If damage >= Toughness, stuff happens. (Full rules: SWAGE pg 94.)
	5. Target wasn't Shaken: they become Shaken. They also take an additional Wound for each Raise.
	6. Target was already Shaken: they take a Wound. The first Raise does nothing. Second and subsequent Raises each do a further Wound.
5. Target can spend a Benny to Soak damage. Roll Vigor; each Success and Raise reduces damage by one Wound. If they soak all Wounds, they also remove Shaken.

### Common ranged combat situational modifiers

* **Range**: -2 at Medium; -4 at Long; -8 at Extreme. Aim action is mandatory at Extreme.
* **Light level**: -2 (dim) / -4 (dark; can only see 10" distance) / -6 (pitch darkness / target invisible or totally concealed). Can be countered by vision augmentation.
* **Recoil**: -2 if shooting multiple rounds in one attack. Reduced by gas-vent or some other gun mods.
* **Called shots**: -2 for limbs, -4 for hand/vitals/head. Can be used to shoot around armour. Vitals/head shots do +4 damage. Hand shots can disarm.
* **Injured**: -1 for each Wound you have taken. 
* **Scale**: from -6 to +10 when attacking objects of different sizes. 
  * Small drones are -2.
  * All metahumans are 0.
  * Most vehicles are +2. 
* **Cover**: -2 / -4 / -6 / -8 depending on how much cover there is. 
  * If the cover makes the difference between the shot hitting and missing, and the cover material could be shot through, then the cover acts as armour instead, rated between +2 and +10.
* **Aiming**: an Aim action before shooting allows attacker to ignore 4 points of penalties due to range / cover / called shots / scale / speed.
* **"The Drop"**: if the defender is *totally* unaware of an incoming attack, the attacker gets +4 to attack and +4 damage.
	* If Shaken or worse from The Drop, character must pass a Vigor or be knocked out. If the attacker calls a shot to the head, this Vigor check is at -2. 
* **Ganging up**: when melee attackers outnumber the attacked characters, they all get +1 to their attack rolls for each additional person they have on their side. Eg. if three people attack one, the three are all at +2. 

## Armour

**Armour**: armour adds its value to the character's Toughness stat, and therefore effects what damage roll is needed to inflict Shaken or Wounds. Toughness is written as eg. 11 (2), meaning they have 11 total toughness and 2 of those 11 points come from worn armour.

Some weapons are **armour piercing**: they remove the value of their AP stat from the defender's armour value before the damage effect is calculated.

## Mixing ranged and melee

* **Firing into melee**: on a normal shot, each skill dice that rolls a 1 hits the wrong target. If using a shotgun or firing more than 1 bullet, becomes a 1 or a 2.
* **Using a ranged weapon in melee:** nothing larger than a pistol. Target number for test is the defender's Parry stat. If you fire against anyone other than the person you're in melee with, you become Vulnerable.

## Slow attacks and evasion

* **Evasion**: if the attacked character is aware of the attack and it is an attack type that can be evaded, they can take an Agility check at -2; if they pass, they take no damage. 

## Status effects

These are caused by various things happening to you.

* **Shaken**: can only take free actions until you pass a Spirit check or spend a Bennie to cancel the Shaken status.
* **Distracted**: take -2 on all Trait rolls until the end of the next turn.
* **Vulnerable**: All actions and attacks against you take +2 until the end of the next turn.

## Fancy guns

### Shotguns

Shotguns firing shot give attackers +2 to hit. They do 3d6 damage at Short range, 2d6 at Medium range, 1d6 at Long range.

Shotguns firing slugs do 2d10 damage at all ranges. You don't get the +2 bonus to hit.

### Full-auto fire

Each gun has a rate of fire (RoF) stat. If this is greater than 1, it can fire more than a single shot in each attack. With most guns (but not all), this is optional, and you can fire at a lower RoF if you want.

1. Declare how many shots you are going to take and who you are targeting.
2. Roll one Shooting dice per shot taken, plus one Wild die.
3. Assign the dice to targets however you want. Any single Shooting die can be replaced by the Wild die roll, if you want.
4. Resolve each damage rolls separately.

Note that full-auto attacks take a -2 recoil penalty to all Shooting rolls (listed under situational modifiers above.) This penalty can be reduced by Edges and gun modifications.

### Three-Round Bursts

If a gun description notes it can fire Three-Round Bursts (or it has been modified to add that ability), then that counts as a RoF of 1 (so incurs no penalty to attack), but it adds +1 to Shooting and damage rolls. This can only be done against a single opponent.

## Supporting others

Declare how you are helping, what skill of yours this is using, and what skill roll you are supporting. Roll a test using the skill as usual.

On a success, the person you are helping takes +1 on their next action using the skill you declared. Get another +1 per Raise. But if you critically fail, they take -2!

If they don't use their bonuses before the end of the round, they expire.

## Testing opponents

This is the opposite of supporting: it's annoying an enemy in some way. Declare what you're doing and a skill for it. Roll an opposed test of your skill vs. the opponents stat that is linked to the skill.

On a success, you can choose to inflict Distracted or Vulnerable.

Taunt is a good skill for this!


