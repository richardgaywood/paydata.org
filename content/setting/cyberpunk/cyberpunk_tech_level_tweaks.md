---
title: Tweaking Shadowrun's tech level
description: Trying to maximise the 'cyberpunk feel' through changes to the technological sophistication
type: docs
draft: true
date: 2021-12-28
---


I have several slightly opposing goals for how I want my Shadowrun campaign to feel, at least in terms of the sophistication of technology.

* I desire a "classic cyberpunk" feel that is roughly aligned with Shadowrun 2e and the foundational works of cyberpunk fiction from the '90s. 
* But at the same time, I think the cyberpunk genre derives a lot of its power from feeling like it is near-future – and not retro-future or far-future. Character's problems and the shape of the world they inhabit should feel recognisable to us. 

    So I also want the world to reflect 20+ years of real-world technological advancement that has occurred in the last thirty years. SR5e and 6e do this, most notably in the form of wireless Matrix and all that goes with it.
* However, I do not want technology to be too advanced. I do not want my game to start to feel more like general sci-fi. SR 5e and 6e definitely do this, to my mind.
* I don't want to stuff to work too well. Cyberpunk tech (or at least, the tech within monetary reach of our players) should be like real-world tech: buggy, flawed, unreliable, sometimes frustrating. I don't want it to have this high-tech sheen where everything works and nothing has any downsides. 

Hence: I want to somehow find a way to blend these different approaches. This document attempts to do that for some aspects.

The changes/tweaks I have proposed are more about aesthetics than they are about rules. Nothing here is changed for game balance reasons. It's just about how the fictional world looks, works, and feels. 

## Tech to remove completely

* *Antigravity* - I mean, c'mon.
* *Practical energy weapons* - you can _make_ a laser cannon, but you can't power it from any sort of man-portable (or even troll-portable) energy cell.


## Limiting augmented reality

*Reasoning: sophisticated near-ubiquitous AR has the ability to transform the world beyond recognition. Road sights, billboards, car licence plates would be no more. Home appliances would have no buttons or other physical interface. Computer keyboards would cease to exist. It's too big a shift.*

**Datajacks / DNI cannot be used for AR**. AR requires realtime integration of synthetic content into your normal senses, whereas simsense replaces your normal senses entirely. In order to add digital content to your sensorium, your sensorium first has to be digitised.

**This means there are two ways to get AR features: cyberware or gear**.

* For visual elements: either cybereyes, or wearing glasses/goggles, or using your commlink. The glasses literally overlay your visual field with the AR elements, which avoids a lot of the complex overhead necessary in a cybernetic approach. As a last resort, you can even use caveman methods - hold your commlink up and move it around, using its screen as a viewport onto AR cyberspace. This has a cost advantage; even the cheapest 'link can do this, and with no additional hardware. 
* For auditory elements: either cyberears or wearing earbuds.
* For tactile elements: either cyberarms/hands or wearing special force-feedback gloves. The gloves are typically quite crude in terms of the "realness" of the feedback they offer.

Without tactile elements, AR control surfaces are downright clumsy to use. Touch targets have to be rendered large enough that the user can use them, and even so, prolonged use is frustrating as mis-taps are just frequent enough to annoy you.

Resolution and focus of AR elements is limited when using glasses/goggles. Reading large amounts of text for long periods is likely to cause nasty migraines.

Combined, these mean that society does not run on AR, because AR has not reached a big enough critical mass so that it can entirely replace other display methods. Street signs still exist. Most restaurants still have signs on the door (except for the occasional hipster speakeasy trying to synthesis some mystique.) Keyboards still exist, as do monitors and TV screens. 

AR is more about how you interact with your gear than it is about how the world presents itself to you. 

## Limiting virtual reality

*Reasoning: cyberpunk has armies of wageslaves crammed on commuter trains travelling to vast open-plan offices of beige cubicles and flickering neon lights. Why, if VR is so good? Why don't people stay home and jack into remote hosts instead? Their employers can still watch their every move.*

* Simsense requires an extremely high-bandwidth, low-latency connection between the brain and the device encoding the simsense signal. This requires a wired connection. Therefore, **a decker must be physically connected to their cyberdeck**, although the 'deck can be wirelessly connected to the rest of the world.
* **Normal people find it profoundly uncomfortable to be in VR for a prolonged period of time in public areas**. The sense of disconnect from your body provokes deep unease and vulnerability. This ruins productivity.

    In the workplace, VR is therefore mostly reserved for:
	   
	* Elite knowledge workers, deckers, scientists, architects, and the like. These people get private offices.
	* Occasional use by wageslaves for eg. telepresence in remote meetings. In short bursts, people are generally fine with it.

## Clarifying VR vs AR

*Reasoning: this is just to try and clean up the profusion of overlapping interface modes and Matrix stuff that Shadowrun offers.*

You are in VR (ie: full simsense, body in ragdoll RAS-override mode) when you are in a host system. All Matrix actions done not in a host are done in AR. The action of entering a host and the action of switching to VR are the same action.

## DNI is not telepathy 



## Wireless Matrix interfaces on gear

*Reasoning: I think 5e's wireless gear bonuses and subsequent hacking is immersion-breakingly stupid, and I wish to hurl it into the sun.*

Domestic / civilian gear like home appliances are completely controllable from the wireless Matrix. This allows smart home control, AR control surfaces, remote monitoring, etc. It also makes these devices controllable to anyone who hacks them.

For obvious reasons, items like weapons and cyberware are not built like this.

While they may offer Matrix control surfaces, these are strictly for secondary control and user interface only. The device's primary functions are all controlled via other means.

For example: a cyberarm's primary control method is the nerve splice between the cybernetic component and the user's body. This is how the user issues all normal "commands", ie. moving it around, picking stuff up, deploying cyberclaws, etc. 

Some models of arm might also offer a secondary Matrix interface. This is used by the arm to present information to the user, such as diagnostics, service requests, user manuals, and the like. If the arm has functions that are too complex to be mapped onto the nerve splice, such as a colour-changing surface coating, they may be controlled here via an AR interface panel. 

Crucially: **hacking attacks over the wireless Matrix can only effect the secondary interfaces** and cannot bypass the device's internal hardware firewall. A hacker cannot shut down or take over someone's arm, or eyes, or any other cyberware. They cannot remotely detonate a grenade or remotely eject a weapon’s magazine. 

Smartguns use a subdermal induction pad mounted in the user's palm and the gun's handle to establish an ultra short range private wireless connection that is used for the primary control surface (eg. cybernetic commands to eject magazines, switch firemodes, etc.) Again, a hacked smartgun cannot be instructed to fire, or not fire.

## Drone brains

*Reasoning: cyberpunk still has lots and lots of low-paid, unskilled labour. There are warehouse workers, dock hands, construction workers, shop clerks, pizza delivery drivers. They have not been replaced en masse by machines.*

* **General purpose drone automation is limited** by the lack of (controllable) general AI. Drones are heavily used in fields such as construction, manufacturing, and other heavy industry; but they are under close supervision at all times, as the dog-brain will frequently get into unexpected states and freeze.
* As a special case, GridGuide empowers self-driving cars in urban areas by providing a mesh network that drones can use to co-ordinate between themselves. This does a lot to keep the dog-brains within their normal operating parameters. Outside of a GridGuide connection, self-driving cars can handle good conditions, but are easily confused by inclement weather, traffic, and so forth. This manifests as the car either parking itself or bleeping and requiring manual intervention from the passengers.
* **Delivery drones are highly vulnerable to hacking and physical attacks**, followed by being looted for their parts and cargo. Companies are reluctant to use drones for automated delivery because of this. The cost-benefit is marginal at best, and favours human deliveries in the rougher neighbourhoods.


## Nanotech

*Reasoning: full-on nanotech, especially nanoware and nanoforges, pushes the tech level further than I am comfortable with.*

Nanotech is in its infancy. It can do two things well: 

1. **Very simple tasks in complex environments**. An example of this is cyberware implantation, where nanobots carry out minimally-intrusive installation of subdermal wiring and splicing of technology onto nerve shunts. Viewed from a nanotech scale, these are relatively large pieces of engineering.
2. **Complex tasks in very simple environments**. An example of this is orbital factories that produce nanosteel, aerogels, exotic carbon matrices, and other materials in hard vacuum / microgravity conditions. These nanobots cannot be used on Earth, as they cannot deal with any environmental complications while nudging carbon atoms accurately into place inside a molecular iron lattice. 

Most nanomaterials cannot be constructed on Earth. Nanobots cannot achieve precision tasks inside the complex environment of the human body; nanoware does not exist. Nanobots are expensive to produce and are totally tailored to one very narrow task; there are no "general purpose" or programmable nanobots. Desktop nanoforges are not a thing. 

(NB: "nanotech" is a misnomer. The 'bots that carry out the procedures are built on the scale of hundreds of nanometers and operate on material on a scale of, at best, tens-of-nanometers.)



