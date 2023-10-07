---
title: Getting started with Shadowrun
linkTitle: Getting started
type: docs
description: Tips and tricks for first-time tables
date: 2020-08-29
weight: 100
aliases:
  - /gms/getting_started_with_shadowrun/
---

Scenario: you and your RPG group want to play Shadowrun. You've never played before; maybe you have experience of other RPGs, maybe you don't. You're intrigued by the *man-meets-magic-and-machine* setting but you've read some stuff about the game system. It sounds... daunting. Maybe you've gotten as far as looking through the rulebook, and thought: *eep!*

If this is you, I hope to help!

Shadowrun is a pretty tricky beast at first -- but I swear it does start to make a degree of sense once you get started. This document presents a grab-bag of tips and suggestions that might help you get past that initial barrier.

Note that this document was written specifically for Shadowrun Fifth Edition (5e), although some of the more generic advice applies to other editions also.

**What I'm not going to discuss**: to keep this document manageable, I am going to focus only on Shadowrun's mechanics. I am not going to talk about non-mechanical GMing advice (eg how to write and pace a mission) or suggest houserules to patch over some of Shadowrun's more annoying problems (these are very much a matter of taste, anyway.) There's plenty of material already written that covers both of those angles. 

## Things to immediately dispense with

There's a few obvious things that you and your table can agree not to use that'll make your initial games far easier without leaving any glaring holes in the game:

1. **Set the splatbooks to one side**: The SR core rulebook has plenty of content for all kinds of characters. So make a pact across your table that you'll start off without any of the content from the "splatbooks" (the per-character-type expansion books: Run Faster, Run & Gun, Street Grimoire, Rigger 5.0, etc.) Now, don't get me wrong - there's a lot of richness in there you'll want to use, probably sooner rather than later; this is a just-for-now deal. You can add the content back in as you find you want it.
2. **Leave technomancers out**: You'll all have enough on your hands with The Regular Matrix, let alone The Magical Matrix. Keep them aside for later.
3. **Approach riggers with caution** [^riggers]: it pains me to write this, because I love riggers and I think they're a huge amount of fun. But playing one involves a huge amount of special rules and even some special core mechanics, so they can be an uphill battle. And they are the least important of the core set of character types. So if you have no strong feelings, maybe avoid them for now. If you do want a rigger at your table, start on the small side with a driver and build up to drone armies.
4. **Aspected magicians** and **mystic adepts**: these character types suffer from some non-obvious problems and it's easy to build under- or over-powered characters with them. Plus, they don't add any flavour to the game that you don't get from having a regular, full mage. Consider them to be an advanced chargen option.

## How to approach character generation

*Oh my god there's so much stuff.*

There is, but there are some things you can do help narrow it down.

You might consider using pregen characters. But pregens suck, and the ones in the rulebook aren't very good (they have some very weird choices and they aren't even rules-legal, which is *incredible*), and dealing with the massive equipment list the pregens have is almost as overwhelming as generating a character. So, maybe skip that, and make your own.

### Chargen methods

First and foremost: use a tool to help you make characters. [Chummer5](https://github.com/chummer5a/chummer5a) is free. Make sure it's configured to use only the core rulebook.

Secondly, a word about chargen systems. Shadowrun has 3.5 different ways to generate characters (Priority, Sum-to-Ten, Karma, and Life Modules.) Each one has significant downsides. (Yes, I know this beggars belief.)

Priority gen is the one in the core rulebook, with the letters A-E. It's the default choice. It has two major downsides. Firstly, it makes some characters really difficult to make (famously, troll deckers are almost impossible.) Secondly, it can cause failure feedback loops. You allocate, say, D to resoures. You do all your skills and attributes. You start buying gear... and realise you need a C in resources. Now you need to go back to skills and attributes and re-do them so you can take the C and give it to resources. New players can bounce around this loop at lot and it gets really frustrating.

Sum-to-Ten is a minor variation on priority gen, described in Run Faster. It lets you trade letters eg. you can have AABEE or BBBEE. It fixes the first problem but not the second.

Life Modules (also in Run Faster) is this hippy weirdo thing were you pick different stages of your character's life and each grants you points in skills or attributes or whatever. Unless you're really good with it, it makes really, really jack-of-all-trade weird characters who aren't skilled enough at any single thing. Avoid.

Finally, we come to what the internet tends to call Karmagen (but Run Faster calls "Point Buy"; same thing.) Basically, you start with a pool of karma and 1 in all your attributes, and just buy whatever increases and gear and abilities you need from the pool. The major downside here is that it's a pain in the arse to do by hand, but [Chummer5](https://github.com/chummer5a/chummer5a) frees you from that. The risk is that it can be a bit overwhelming, but I think on balance as long as you're not doing chargen by hand this is the best option for new players.

### Thinking about characters

Shadowrun is classless, and you can build anything, which is great -- but also overwhelming. How do you get started navigating all this stuff?

* Think about **core archetypes** - most characters will pick a role in the team and specialise in it. Combat, magic, hacking are the most obvious and clear-cut examples. Shadowrun is a game of specialists, where the team is usually made up of people who do different things really well (as opposed to everyone doing everything poorly.)
* What does specialisation mean? This can vary a bit across tables but a good rule of thumb is being able to roll 12-15 dice in a few key skills, across your attribute, the skill itself, and any bonuses from gear. (Fewer than 12 and you're probably a little underpowered. It's fine to have more than 15 if you want, but be wary of being over-specialised; you could be better off spreading your points around across a broader base of skills.)
	* For a combat character, key skills might be a selection of small/concealable weapons and larger/more dangerous weapons. 
	* For deckers, it's the skills in the Hacking and Software groups. 
	* For magicians, it's spellcasting and summoning. 
* Once you have a core role, about **other secondary roles** you might take up - faces (negotiation and social infiltration), physical infiltration and breaking & entering, vehicles, and many, many more. This is where the classless system in Shadowrun really shines. There's usually enough room in your build to be rolling 9-12 dice in a few skills grouped around a secondary role.
	* Some of these other roles naturally pair off with other archetypes. For example, combat characters have high Agility for combat, and B&E skills mostly use Agility. So any combat character can roll good numbers of dice in skills like Lockpicking and Sneaking for a modest number of skillpoints.
* Think about **stuff everyone should be able to do** - you probably want 4-6 dice in some standard-issue crime skills:
	* Firing a weapon, if only as a backup
	* Lying to people (Con)
	* Blending in with crowds (Etiquette)
	* Noticing stuff (like ambushes!) (Perception) [^EnigmaticOxygen]
	* Being stealthy (Sneaking) [^EnigmaticOxygen]

## Some notes on specific rules

Even with the splatbooks left aside, the SR 5e core rulebook (CRB) alone is still pretty large. It's a lot easier to get to grips with if you leave out the less important rules... but the book's organisation isn't great, so it doesn't do a great job of flagging up the rules that you can safely ignore when you're starting out.

In addition, some of the rules are just plain *bad*. Either completely confusing, a pain in the arse to use, or both.

Here I'm going to flag up some sections I suggest you ignore.[^Xenon]

### Rules to definitely skip over

I advise you to not even *read* these.

Characters:

* **Addiction** and **Overdosing** - these rules are, famously, completely confusing and don't even work that well once you unpick how they're supposed to be used. Skip. This will make combat drugs over-powered, however, as there'll be no counterbalance to them; later on, you might want to explore some simplified houserules for addicition. Or just ignore the issue if you don't mind it.
* **Swimming** - why does a game of urban cyberpunk thievery need more than half a page of rules for swimming, SCUBA diving, and treading water? Beats me, but I suggest you skip 'em. [^EnigmaticOxygen]

Combat:

* **"Blasts in a confined space" / "simultaneous blasts"** - these are sometimes called the "chunky salsa" rules because that's the effect they have on people. They're a pain in the arse to calculate and given how deadly explosives are anyway they only make the difference between being "dead" and being "really, really dead."

Magic: 

* **Background count** - this is a GM-fiat way of subtracting some dice from mages in a way they cannot do anything about. Most people think it's a fairly clumsy and un-fun attempt to balance mages, who are otherwise a bit overpowered. 
* **Initiation and metamagics** - these are down-the-road advancement options for Awakened characters (magicians and adepts)[^EnigmaticOxygen]. Safe to ignore until you need them.

Matrix:

* **Noise** - it's really just a way of saying "your connection is bad." Ignore the tables to calculate it. If you feel like the fictional situation the characters are in demands some, just make up a number and apply it. [^JerekTelorian]

Vehicles:

* **Sensor targeting** - heck of a lot of dice rolls that add little to the game. Entirely skippable.

### Rules to approach with caution

Combat:

* **Barriers** - the barrier rules (both for destroying structures and for shooting people through the cover they are cowering behind) are a bit fiddly. They work OK, but aren't the fastest thing to play out at the table. I'd suggest keeping them for only when it really matters. If it's a more trivial set of circumstances with a predictable outcome, like car vs. chain link fence or pistol vs armoured bunker, don't bother looking the rule up.
* **Surprise**[^LeonAquilla] - there's a throwaway line in the rules that suggests you should roll for surprise quite often, basically anytime one side wasn't fully expecting combat to start. However, failing a surprise check is extremely deadly, so rolling it routinely can result in some weird outcomes. I'd suggest saving the surprise rolls for genuinely unexpected ambushes, and handling most "combat is starting now" by simply rolling for initiative. 
* **Scatter** - the scatter rules only work if you're doing your combat on a grid with tokens or miniatures. If you're running anything theatre-of-the-mind, you'll have to do some handwaving to resolve the scatter roll.
* **Recoil** - recoil accumulates across each character's turns, which is deeply obnoxious to track. It's also reset by the character spending a single action to do anything other than aiming, so it's pretty easy for the character to avoid the penalty anyway. You won't break the game if you just ignore it adding up across turns and only consider it in the context of each individual attack action.

Magic:

* **Enchanting** and **ritual spellcasting** - these both sound cool (because they are cool!) but when you look really hard at the numbers they both turn out to be rather underpowered and consequently dull. If anyone at your table is passionate about them, come back later and houserule to make them more powerful.
* **Summoning** - there's nothing wrong with the rules here, it's just that spirits are very powerful, to the point where they can easily become unbalancing. There's a lot of houserule suggestions around to nerf them but initially I suggest you start out using the rules as written and see how you go. Just be aware of the problem. If it gets too much, consider removing the Binding mechanic as a quick fix.[^EnigmaticOxygen]
* **Foci** - many people (myself included) feel mages are overpowered in modern Shadowrun editons. This stems from a few key areas, one of which is spirits, but foci is another. In particular, they are very cheap for the benefits they deliver - particularly power, spellcasting, and summoning foci. Consider making the higher-rated ones much more expensive, or banning them entirely until you are comfortable with the rules.[^EnigmaticOxygen]

Matrix:

* **The whole damned thing** - well, I joke, buit only a little. The Matrix rules are pretty slow to play out so you probably want to reserve them for only the decker's spotlight moments: the big hack against the big target for the big score. If they're just, say, snooping someone's commlink to get some intel, I suggest you make them roll once against a threshold and then move on.
* **Bricking cyberware** - it's annoyingly easy for a hostile decker to render your team's street sam totally inoperable by using Matrix attacks against, say, their cybereyes. This isn't a great deal of fun for the player, and there's not a lot they can do about it either (it's not like they can turn their eyes off...) Steer clear of that at least until your non-decker players understand the risks, because if they're blindsided by it (pun intended) it's gonna piss them off.

Vehicles:

* **Vehicle speeds** - the Shadowrun tables for translating the abstract "speed" stat to actual miles-per-hour are, umm, broken. Don't look too hard at them or things fall apart. If you try really hard, [you can break the world with hilarious consequences](https://www.reddit.com/r/gametales/comments/1nbjhe/xpostshadowrun_everyone_is_dead_san_francisco_is/).
* **Drones** - drone swarms can get very overpowered very quickly. Also, having lots of drones around can really slow down gameplay, as they all get their own initiative roll, have to resolve their actions, etc. Like spirits, this isn't a reason not to have some (they're cool!), just be aware of the issues.
* **Vehicle damage** - if you follow the core rulebook to the letter, you will find that vehicles are almost absurdly easy to destroy and ruinously expensive to repair. In turn, your rigger characters will never make enough money to keep up with repair and replacement costs. I don't have any smart answers to this beyond full-on houserules, but at the start I suggest you just handwave your way around it an apply as much vehicle damage as "feels right", regardless of what the rules say.

Other stuff:

* **Lock picking** - per the rules, you usually have to roll once to break into the casing of a maglock, then roll again to actually pick it. This is nonsense on stilts. Just roll once.

## GMing

### Fake it till you make it

> Shadowrun has a lot of rules that do not come up very often, and for some reason, not all of them are intuitive. Instead of knowing each specific exception, make sure you know well the basic stuff, like skills, combat mechanics, common infiltration rolls and basic magic and hacking stuff. If a niche case comes up in game, make a quick call that makes sense in the system and move on.... Focus on having fun, cool descriptions and in the characters. -- Yomatius[^Yomatius]

Your player just said they want to do something, and you know there are rules for this but you can't remember how they work but you do remember they span several pages and you've already paused the session twice in the last hour to look stuff up. This doesn't feel like a good time to stop play. So now what?

*Don't panic*. For all of Shadowrun's voluminous rules, and 80+ skills, and millions of items of gear, and modifiers, and modifiers that modify the modifiers (!), it almost always boils down to the player:

* rolling a skill 
* ...plus an attribute
* ... plus or minus some modifiers
* ...against a threshold.

*As GM, you are well within your rights to make this up on the spot*. Now, whether or not to do so can be a tricky judgement call, with a few factors to weigh up:

* Is the character doing something the rules don't cover? If so, you're definitely going to be ad-libbing. (Despite the huge number of rules, this still happens a lot. Players are a wily bunch.)
* Is this something the rules cover, but you know the rules are too detailed and fiddly to use right now, perhaps because the player is taking a low-stakes or low-risk action? Then short-cut the rules down to a single roll.
* Is this something the rules cover, but you don't know them well enough to confidently use the full rules? You have a choice here: either pause play to look them up, or handwave them down to a single roll and look them up afterwards. There's no right answer, it depends on the situation and your table's preferences.

Suppose you want to make a roll up. How do you do that?

* **Picking a skill** - this isn't usually too tricky, because despite Shadowrun having a lot of skills, they're fairly well defined without too much overlap. The social skills can be slightly tricky - the lines between Con and Negotiate and Etiquette can be blurry - so watch out for that. 
* **Picking an attribute** - every skill has a linked attribute, which is a fine choice. Sometimes you might want to change it though, and that's perfectly fine too. For example, I have made players roll Strength + Unarmed Combat when attempting to grab someone and hold them still.
* **Modifiers** - use these to represent the situation. Are things making the character's task harder or easier? Do they have inadequate tools, are they working under time pressure, is the mana field here polluted, is the concealed weapon they are looking for small? Impose -2, -4, or -6. Was the sound they're trying to locate really loud, are they trying to convince a friendly NPC to do something innocuous, or are they searching the Matrix for public information? Give them +2, +4, or +6.
* **Threshold** - use this to capture the intrinsic difficulty of the job. Are they picking a poor quality lock? Use a threshold of 1. Are they trying to drive a motorbike through a narrow gap at high speed? Use a threshold of 3.

Note that there's a lot of overlap between modifiers and threshold, particularly when ad-libbing a roll like this. This is true on a statistical level as well, as a modifier of +3 is equivalent to changing the required threshold by -1. It's perfectly OK to skip the modifiers and just change the threshold instead. This is particularly true of tests like Perception, where the result is graduated rather than a flat pass/fail. I rarely modify Perception checks, and instead I vary the information the player received based on the outcome of an unmodified roll.

If there really isn't a skill to match, you can also ask for an attribute+attribute roll. There's a few of these defined in core rules, like Judge Intentions (Int+Cha) or Composure (Wil+Cha). You can combine any two you like though.

### Difficulty setting & NPC stats

Character generation is overwhelming enough when you're only doing one; what if you need six NPCs?!

The very short answer is: don't. It's not usually necessary. 

A real common GM trick is the "rule of threes". (This is also similar to the [Rule of Twelves](https://www.youtube.com/watch?v=lFdzTzqUlvw), described here in this video by u/Bamce[^EnigmaticOxygen].) If you need a dice roll for an NPC, pick a level:

* If their skill level is **basic**, roll **6 dice**. Examples: wageslaves driving a car, gangers trying to intimidate someone.
* If their skill level is **trained**, roll **9 dice**. Examples: wageslaves doing their job, gangers or mall cops fighting. 
* If their skill level is **skilled**, roll **12 dice**. Examples: standard security guards fighting, bouncers looking for concealed weapons.
* If their skill level is **professional**, roll **15 dice**. Examples: high threat response teams in combat, a Mr Johnson lying or negotiating.
* If their skill level is **elite**, roll **18 or more dice**. 

In-game, these dice can come from some combination of attribute, skill, and gear - it doesn't matter which.

When you want to speed play up even further, you can swap out opposed tests against NPCs for a threshold test against their dice pool divided by 3. (Don't use 4, here, as you usually would for buying hits, unless you want to make your NPCs even more cannon-foddery than they already are.) So a ganger would always roll 3 hits to attack and 3 hits to defend. This can get a bit boring if over-used though.

## Best splatbook content

I suggested above that you set the splatbook content aside at first, but there's a lot of good stuff in there that you'll want to introduce as you go along. Some suggestions for the most useful expansions to look at first are below. (These are in no particular order.)

* **Armour from Run & Gun** - lots of cool gear here, with lots of flavour.[^EnigmaticOxygen]
* **Augmentations from Chrome Flesh** - the cyberware, bioware, and other augments expand the options for mundane characters really usefully.[^EnigmaticOxygen]
* **Magic traditions from Street Grimoire** - I think these add nice flavour to expand role playing options for mage characters.
* **Vehicles and drones from Rigger 5.0** - Riggers thrive on their gear, and this expands their options a long way.[^EnigmaticOxygen]
* **Vehicle mods from Rigger 5.0** - I don't love the rules themselves, but the crunch is all done away from the table, and I think it makes riggers way cooler.
* **The decker actions from Kill Code** - gives deckers a lot more tactical flexibility.

<!--
## If RAW is not for you, but you still like the setting

There are [alternative systems](https://www.reddit.com/r/Shadowrun/comments/fiddqk/big_list_of_shadowrun_alternatives/) if you think you want to go that way. But if your table want to get to grips with the core Shadowrun system, hopefully this document can help.
 
-->

<!--

> I second this comment. Shadowrun has a lot of rules that do not come up very often, and for some reason, not all of them are intuitive. Instead of knowing each specific exception, make sure you know well the basic stuff, like skills, combat mechanics, common infiltration rolls and basic magic and hacking stuff. If a niche case comes up in game, make a quick call that makes sense in the system and move on.... Focus on having fun, cool descriptions and in the characters.
--- Yomatius [^Yomatius]



--> 


## Acknowledgements & further reading

This document was compiled from the many excellent suggestions in these following posts on r/shadowrun. I have only included a small selection of the tips contained in these links, so if you want more, click through!

* "[GMing Shadowrun is stressful, how can I improve? I am starting to feel like I am just not good enough to do it.](https://reddit.com/r/Shadowrun/comments/i6b7l6/gming_shadowrun_is_stressful_how_can_i_improve_i/)" - the thread that inspired this doc
* "['I am a new GM' tips and tricks doc](https://reddit.com/r/Shadowrun/comments/i8bfh0/i_am_a_new_gm_tips_n_tricks_doc/)" - thread where I first suggested creating this doc.
* [Your worst/most fiddly/most baffling rules in the 5e CRB](https://reddit.com/r/Shadowrun/comments/if4xon/your_worstmost_fiddlymost_baffling_rules_in_the/)
* [Thread were I posted this doc](https://reddit.com/r/Shadowrun/comments/iit9b5/i_wrote_a_getting_started_with_shadowrun_guide/) looking for feedback and suggestions.


[^LeonAquilla]: Thanks to u/LeonAquilla [this suggestion](https://www.reddit.com/r/Shadowrun/comments/if4xon/your_worstmost_fiddlymost_baffling_rules_in_the/g2m4p31/).
[^EnigmaticOxygen]: Thanks to u/EnigmaticOxygen for [these suggestions](https://www.reddit.com/r/Shadowrun/comments/iit9b5/i_wrote_a_getting_started_with_shadowrun_guide/g3asmqr/).
[^Xenon]: Thanks to u/ReditXenon for [these suggestions](https://www.reddit.com/r/Shadowrun/comments/iit9b5/i_wrote_a_getting_started_with_shadowrun_guide/g3asmqr/).
[^JerekTelorian]: u/JerekTelorian: https://reddit.com/r/Shadowrun/comments/i6b7l6/_/g0v0a3v/
[^riggers]: thanks to [u/CelticSurfer for this suggestion](https://reddit.com/r/Shadowrun/comments/if4xon/_/g2oiibn/)
[^Yomatius]: /u/Yomatius: https://reddit.com/r/Shadowrun/comments/i6b7l6/_/g0wlzkw/?context=1

<!--
## Basic rules everyone should know

(Page references below are for the SR 5e Core Rulebook (CRB).)

* How to roll tests(pg 44-47)
* Combat turns, actions, initiative (pg 49, 158-160)
* How to use Edge to your advantage (pg 56)
* How to resolve a combat attack, working out if someone gets hit and how much damage they take (pg 172-174)
	* Note there's a complex stew of modifiers that can apply, but you only need a sense of those
* Stuff for your speciality - combat, or controlling
	* If you're a combat type, 
-->