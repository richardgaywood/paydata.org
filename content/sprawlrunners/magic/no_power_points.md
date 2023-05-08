---
title: Using Powers
linkTitle: Using Powers
type: docs
description: My take on No-Power-Points spell casting
date: 2023-01-15
lastmod: 2023-01-23
weight: 100
icon: "fa-solid fa-pencil"
---

{{< draft >}}

## The pitch / my goals

What I want to achieve:

* Maximum compatibility with SWADE supplements -- I want my players to be able to use new Powers in SWADE splatbooks and settings without modification
* Minimum book-keeping at the table
* Minimum extra rolling -- I don't want to force a Resist Drain roll for each power used
* (Ideally) support artificing, which per RAW is not compatible with No Power Points (NB: I have not yet managed this)
* Put Powers on a curve, so they improve with the character instead of being the same from the time the character learns them -- similar to the Epic Power Modifiers in Savage Pathfinder, I think this helps "deepen" the arcane character's progression curve

**Why not RAW No Power Points?** I strongly dislike the huge negative modifiers it imposes on PCs arcane skill rolls. Consider a Veteran character. Under the Power Point rules, they probably have 20-25 power points in their pool. An 8-10 PP power is well within their grasp, should they choose to use it. It’ll use a chunk of their pool, but they can fall back onto Bennies. Meanwhile, under the NoPP rules, that same 8-10 PP power is imposing a -4 or -5 penalty to the arcane skill roll – making it an extremely difficult roll. This, in turn, makes arcane characters under NoPP feel weak and underpowered, as they get no chance to stack power modifiers onto their powers to juice them up.

**Feel like Shadowrun:** the primary target audience for these rules are my home game and that is set in the Shadowrun universe. So, I want these rules to leave room for a few Shadowrun-specific details I want to incorporate, such as Drain (fatigue damage from spellcasting), blood and toxic magic, and the idea of less powerful "safer" casting and more potent casting but that comes at a potential price.

_TOOD: more here_

## Books in scope
These are the Savage Worlds books I am flicking through and drawing ideas from as I try and write these rules.

* SWADE CRB (obviously...!)
* Fantasy and Horror Companions, in particular the new Powers in each
* Savage Pathfinder CRB, in particular the new Powers and the Epic Power Modifiers
* [Tomes & Prayers](https://www.drivethrurpg.com/product/319970/Tomes--Prayers-Fantasy-AddOn?) by Cyril Ronseaux

## The core concepts

### Drain

The act of using magic involves drawing power from somewhere and channeling it through the practitioner's body. This is tiring and can be very dangerous. _Drain_ is what happens when the practitioner pushes themselves too far. 

Drain is usually Fatigue damage, but it can be a Wound in very bad cases. 

Drain is resisted just like Soak, costing one Bennie per resistance attempt. Instead of Vigor, the character uses the attribute associated with their arcane or Magic skill - Spirit or Smarts. 

Drain cannot be healed by magical or mundane means; only the passage of time and Natural Healing rolls. However, powers or abilities that allow a character to ignore wound or fatigue penalties do function normally against Drain damage. 

### Two new derived stats

New concept: **Power Limit**

* Starts at: (½ arcane skill die type) - 2
* Goes up when you increase your arcane skill
    * As with Parry and Toughness, also goes up +1 every other increase past d12. So an arcane skill of d12+2 gives 7, d12+4 (should you somehow get it that high!) gives 8, and so on.
* Goes up by 1 at each rank
* Goes up with Edge

New concept: **Mod Limit**

* Starts at 1
* Goes up with Edges

### Two different diceroll types for power usage

When using a Power, the arcane skill roll is defined as **Controlled Magic** or **Wild Magic**. 

* Controlled Magic is what happens when: 
    * the total PP of the power + all modifiers is equal to or less than the power limit, and 
    * the total number of modifiers is equal to or less than mod limit
* Otherwise, the Power usage is Wild Magic. 

**Controlled magic** works like this:

* Standard roll of standard arcane skill, no modifiers
* Crit fail[^1] results in mild backlash - sustained spells dropped, practitioner is Shaken, the Power might also go wild in some way (GM fiat) 
* During any Power usage where the practitioner's arcane skill die aces, after the effect of the Power is resolved, they must take (or resist) one point of Fatigue Drain. 
  * If they use a Bennie to reroll the Power usage, and the die does not ace on the roll they choose to keep, they do not take Drain. 

**Wild Magic** works like this:

* Roll of arcane skill with a -2 modifier [^2]
* Backlash happens a roll of a 1 on arcane skill die. Bad backlash: 
    * All sustained spells dropped
    * Practitioner is Stunned
* During any Wild Magic Power usage where the practitioner's arcane skill die aces, after the effect of the Power is resolved, they must take (or resist) one point of Woumd Drain. 
  * If they use a Bennie to reroll the Power usage, and the die does not ace on the roll they choose to keep, they do not take Drain. 
* (Probably) the maximum power you can use in wild magic is 2x your Power Limit; any more than that will just kill you dead on the spot.

[^2]: This may need tweaking, but -2 feels about right.

{{% design %}}
A box of fatigue damage “heals” in an hour, which is the same length of time that it takes to recover PP. Soaking allows the practitioner to potentially trade bennies for the “spellcasting resource pool”, which is fatigue here; this is similar to trading bennies for PP. So controlled casting is intended to be an approximate equivalent to a PP caster just using their pool and then relying on it refilling before they need it next.

At the same time, this reduces the ability of low-level practitioners to go all-in on one massive Bolt with +AP, +damage, +range like they can under the PP system. It smooths out the progression curve by capping modifiers on powers at lower levels.
{{% /design %}}

## Other notes and mechanics

### Healing Fatigue / Wounds from Drain

Fatigue and Wounds taken from use of powers is magical damage dealt to your entire body at the subcellular level; it cannot be treated with the Healing skill or the _healing_ or _relief_ powers. THe character can only recover with time. As normal, Fatigue recovers after an hour of rest, and Wounds heal with natural healing rolls.

### Sustaining Powers

Powers with durations measured in rounds can be cast in two ways, chosen when you use the power: either normal, or sustained. 

* If normal, the roll is normal, but the power terminates at the end of the normal duration. Practitioner needs to re-cast to do it again.
* If sustained, the power keeps going as long as they like, but they are at a cumulative -1 on all future arcane rolls per sustained power.

### Careful Casting (maybe)

A variation on controlled casting for when time is not a factor; designed to allow practitioners free-er use of powers during non-combat scenes without risking knocking themselves out. (This replaces the concept of "Power Preparation" from the core SWADE NoPP rules.)

* Takes ~minutes
* Allows a free Soak roll against the drain [^5]
* Cannot be used for limit break casting

[^5]: Maybe at a +1 or +2 modifier, too?

### Possible Edges

* **Initiate:** can take once at each of Seasoned, Veteran, Heroic. Adds +1 Power Limit [^3] and +1 Mod Limit. Requirements on arcane skill and stat. 
    * Maybe: can continue to take at every other Advance at Legendary, similar to More Power Points.
* **Sustaining focus:** allow “free” sustaining of a power, choose to use at time of casting, can only be used for one power at once
* **Wild Magic Masochist:** allow soak attempts on the Wound for using limit break casting, but this still needs Bennies in the usual way. [^4]
* **Wild Magic Mastery:** can attempt to use powers at 2x to 3x their Power Limit; take a -4 penalty on the arcane skill roll and take backlash on a roll of a 1 or a 2.
* **Flexible Caster:** use a Power modifier to change any Power’s trapping on the fly (Maybe Veteran rank)
* **Arcane Mastery:** (Only if using Epic Power Modifiers, see eg. Savage Pathfinder): Adds +1 to the Mod Limit, and allows the use of Epic Power Modifiers for those powers that have them. (Veteran or Heroic rank)
* Maybe an edge to unlock Careful Casting

[^3]: This should maybe be +2 power limit per Initiate Edge.
[^4]: This is underpowered and needs revising.

Variations:

* **Blood Magic:** each Wound inflicted on someone with a melee weapon gives some number of PP (5?) that can be added to the power limit for one Power usage. Blood mages often have a ritual weapon that can “store” these PP.
* **Toxic Shaman:** shaman gets a boost to their power limit when in their toxic domain. Could apply to “home ground” for other kinds of practitioners too.
* **Astral Shallows:** reduce everyone’s Power Limit.
* **Astral Surges:** increase everyone’s Power Limit.

## Gaming it out

### Examples

Alice is a Veteran with a d12 in Spellcasting who has one rank of the Initiate Edge. Bob is her slightly hapless and extremely bumbling apprentice, Novice rank, and a d8 Spellcasting skill.

Alice's power limit is calculated as: 1/2 of her d12 (=6), -2 to start with (=4), +2 for her Veteran rank (=6), +1 from Initiation (=7). Her mod limit is the base 1, +1 for Initiation (=2). Bob's power limit is ((1/2 * 8) - 2) = 2, and his mod limit is 1.

During a heated disagreement about rent, Alice and Bob both let fly with _bolt_ at their usurious landlord. 

Alice plays it safe and uses controlled casting. She adds two modifiers to the _bolt_'s base 1PP cost: 2PP for extra damage, and 3PP for AP6. The total PP cost (6) is still within her power limit, so this is definitely controlled. She rolls her d12 Spellcasting without modifiers.

Bob is getting a little carried away and overdoes it. He casts _bolt_ with the 2PP extra damage modifier. That's within his Modifer Limit, but the total cost of the _bolt is now 3PP - over his power limit. So this is now a Wild Magic cast. He rolls his d8 Spellcasting at a -2 penalty. He gets an 8 on his Wild Die, so the _bolt_ lands. But he rolls a 1 on his Spellcasting die! As the spell rips from his body, he pays a price: he is Stunned and he takes an immediately Wound. He has Bennies, but he can't try and soak this Wound.

<!-- Two _bolts_ are enough to subdue the landlord and Alice and Bob are free to go about their business. As the scene has ended, they both now take a box of Fatigue damage. Alice doesn't have anything else to do today, so she decides to just take her damage, and will spend an hour relaxing to let it heal naturally. Bob is feeling rather worse for wear, however, and spends a Bennie to attempt to soak the fatigue. He will roll his Spellcasting attribute -- Smarts -- to do so. -->

### Ranges of power/mod limits

Suppose a typical magic-focussed character starts at d8 arcane skill who takes the initiation edges each rank they are available:

| Rank              | Power limit | Mod limit         |
|-------------------|-------------|-------------------|
| Novice (d8 skill) | 2           | 1                 |
| Seasoned (d10)    | 4           | 2                 |
| Veteran (d12)     | 6           | 3 (4 with Epic)   |
| Heroic            | 7           | 4 (5 with Epic)   |
| Legendary         | 8+          | 5+ (6+ with Epic) |

### Modifier counts

Easily the most modifiers are for the combat spells blast, bolt, and burst. Considering blast, you might (in extremis!) want add to the 3PP base:

* +1 for LBT
* +2 for +d6 damage
* +3 for AP6
* +2 for Heavy Weapon
* +1/+2 for Range
* +1 for Selective
* +2 for lingering damage

=> 7 modifiers (and 16 PP)

The system as proposed above has players start with 1 modifier, then +3 through initiation => max 4 for controlled casting. Is that enough? Note that the total of 16 PP is a lot, but if the practitioner is willing to go all-in, it’s quite easily achievable for even middling ranks.
