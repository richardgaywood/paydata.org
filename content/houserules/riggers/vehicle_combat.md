---
title: "Driving, chases, stunts, and crashes"
linkTitle: "Vehicle combat"
type: docs    
weight: 20
---

{{% pageinfo %}} 
These rules are **not canon** for my current campaign.
{{% /pageinfo %}}

## Piloting conditions

All vehicular action happens in one of two types of environment:

* Speed environments are when the terrain is open: clear roads, calm seas, open skies. Tests are limited by the vehicle's Speed stat.
* Handling environments are when the terrain is crowded: busy roads, heavy storms, nape-of-the-earth flying. Tests are limited by the vehicle's Handling stat.

As vehicles travel, the type of environment may change. Characters may seek to use this to their advantage by steering the action to an environment that favours them and their vehicle.

## Standard test types

### Vehicle driving tests

All vehicle driving checks use Intuition when a rigger is jumped in. Reaction continues to apply for vehicles being piloted in AR or via physical controls.

As per RAW, stunts are an unopposed driving tests with a threshold of between 1 and 4+, depending on difficulty of the manoeuvre being attempted. Stunts are always limited by Handling, even in speed environments. 

* Basic form of test when not jumped in:
	* Reaction + Vehicle Skill \[Handling\] or \[Speed\]
* Basic form of test when jumped in:
	* Intuition + Vehicle Skill \[Handling\] or \[Speed\]
	* Reduce threshold by VCR rating

### Vehicle defence tests

When a vehicle is attacked - either shot at or rammed - we need a dice pool to defend against that damage. What this dice pool should be is pretty unclear from RAW. I am borrowing the below wholesale from [A Light In The Dark](https://docs.google.com/document/d/1OY5wjybJXY297QBfUvXPCJZww72tRXYn-NqE0Umknno/edit); that link has further discussion about why they made these choices.

* **Vehicle or drone on autopilot**: The vehicle or drone defends with pilot + maneuvering autosoft. If it has no autosoft, with twice its pilot. The vehicle can full defense; if it does, it applies its pilot to the roll.
* **Driving vehicle in the meat** (physical or AR controls): You make defense tests for the vehicle using your Reaction + Intuition, as normal. You can’t block or parry.  You can’t full defense for the vehicle, but you can evasive drive, which applies your intuition to the defense test.  Combat sense applies.
* **Piloting in VR (no control rig)**: You make defense tests for the vehicle using your Intuition + Intuition. You can’t block or parry  You can’t full defense for the vehicle, but you can evasive drive, which applies your Intuition to the defense test. Combat Sense does not apply. Hotsim does not apply a bonus.
* **Jumped in (VR, control rig)**:  You make defense tests for the vehicle using your Intuition + Intuition. You can block or parry if the drone or vehicle has arms, or arm-equivalents (GM discretion); if you do, the vehicle’s handling is your limit. You can full defense, and if you do, the full defense “follows” you if you switch what vehicle you’re jumped into; it applies your Intuition to the defense test. Your control rig’s rating is not applied to the defense test. The Control Rig Booster or Control Rig Optimization bonuses do apply.  Combat Sense does not apply.

### Controlling vehicles

A person controlling a vehicle manually must spend at least one Complex Action per turn on a Control Vehicle action, otherwise they will lose control of the vehicle at the end of the turn. Uncontrolled vehicles impose -2 dice pool penalties on all occupants as they skid around, and will either be brought under control by the autopilot or crash.

However, if the driver is controlling the vehicle via AR and choose to receive two bonus Matrix simple actions, they can use those actions to control the vehicle, effectively doing so for "free." This does mean they cannot receive any bonus meatspace actions, however. See the [action economy page]({{<relref "houserules/action_economy/basics.md">}}) for more information.

A jumped-in rigger can do their Control Vehicle for a vehicle with a Free action.

## Vehicle damage

{{% alert title="TODO" color="warning" %}}
Filling a vehicle's damage track does not destroy it; it immobilises it. Hence repairs are cheaper.

Jerry rig - mechanics roll, same mechanics as First Aid but for removing boxes of vehicle damage to get it running again, takes a few minutes (extended test?)

shooting: choose to shoot at passengers (use cover/barrier rules, no damage to vehicle) or shoot at vehicle (counts as called shot, -4 penalty, does damage to vehicle's damage track as normal)
{{% /alert %}}

## Crashes & ramming

First, work out the impact speed:

* If the vehicle is ramming a stationary object, as long as it has enough runup, the driver can choose any speed up the vehicle's maximum. GM might restrict this if there's not enough room.
* If it's vehicle versus vehicle and both are moving:
	* If it's a handling environment, use the two vehicles' Acceleration stat. Putting on a last-second surge of speed is the important thing here.
	* If it's a speed environment, use the two vehicles' Speed stat. Raw top speed is what matters.
	* If it's a head-on collision, the attacker can choose the impact speed, up to their vehicle's full Speed or Acceleration stat.
	* If it's a from-behind collision, subtract the stats. If this ends up less than 1, use 1.

Second, roll to hit:

* Attacker rolls: Int/Rea + Vehicle skill \[Handling\] or \[Speed\]
* Defender rolls: defence test as detailed above (usually Rea+Int or Int+Int)

There is no clean miss here. If the defender gets more hits, they can still end up damaging the attacker - keep following the below.

Third, work out the damage code done to the defender: take attacking vehicle's Body, subtract defending vehicle's Body (minimum 1.) Add attacker's net hits. Multiply by the impact speed. This is the number of boxes the defending vehicle has to soak with Body + Armour.

Fourth, work out the damage code done to the defender: take defending vehicle's Body, subtract attacking vehicle's Body, minimum 1. Subtract attacker's net hits. Multiply by the impact speed. This is the number of boxes the attacking vehicle has to soak with Body + Armour.

{{% alert title="Example" %}}
Alice is jumped in and driving a Ford Americar (Body 8, Armour 4, Acceleration 2) and tries to ram Bob who's riding a Suzuki Mirage (Body 5, Armour 6, Acceleration 3). It's a Handling environment. Bob is trying to get away, so we use the difference in the stats.

Alice rolls Int+Pilot+VCR and gets 4 hits, Bob rolls Rea+Pilot and gets 2 hits. The impact speed is only 1, as Bob's bike is faster.

Bob's Mirage now has to take damage: the difference between the Body stats is 3, plus 2 net hits, times impact speed 1 = 5 boxes of damage, soaked with 11 dice.

Then Alice's Americar has to take damage: the difference between the Body stats is -3, which becomes 1, minus Alice's net hits means she takes no damage. 
{{% /alert %}}

{{% alert title="Example 2" %}}
This time, Alice tries to ram Bob in a head-on collision. This time the impact speed is 2. Same test result: 2 net hits to Alice.

Bob's Mirage now has to take damage: the difference between the Body stats is 3, plus 2 net hits, times impact speed 2 = 10 boxes of damage.

Then Alice's Americar has to take damage: the difference between the Body stats is -3, which becomes 1, minus Alice's net hits means she takes no damage. 
{{% /alert %}}

{{% alert title="TODO" color="warning" %}}
crashing (like ramming but against immobile objects)

damage to passengers:

* same number of boxes as vehicle takes? soak with body+armour as usual. Maybe some AP-x penalty.
* if passengers are strapped in -> stun damage
* if passengers are not -> physical damage
{{% /alert %}}

### Forcing a stop

Attacker declares as a Complex action. Resolve initial test as for a ram, but if there are any net hits to the attacker then before damage is taken, the defender has a choice: they can avoid all damage and come to a halt, or they can keep moving but resolve it as a ramming attack with full damage for both sides.

## Chases & pursuits

For each pairing of vehicles, start a four-segment clock to represent the distance between them. The clock represents the distance between the vehicles, from very close (empty) to very far (full). For example, if the PCs are being chased by two NPC vehicles, there'd be two clocks. (If there are large numbers of NPCs, combine their clocks as appropriate.)

For special circumstances where a longer range applies - eg. air combat - use a six-segment clock instead. (I don't expect to do this often, if at all.)

At the end of each turn, roll a vehicle test, limited by each driver's vehicle's \[Handling\] or \[Speed\] depending on what kind of environment the vehicles are in. Compare each pair of rolls for each clock. The winner of the test can choose to increase or decrease range by one step, as they prefer.

If the clock is empty, the vehicles are almost on top of each other, and either driver can attempt to ram or force a stop. If the clock is full and any driver adds another segment to it, they get away clean, and the chase is over.

### Stunts in pursuits

As a Complex action during the turn, any driver can attempt a stunt to try and increase or decrease the distance clock. The driver nominates a stunt difficulty, then both drivers roll separately against the stunt's threshold. If one driver succeeds and the other fails, they can increase or decrease the clock by one tick.

### Pursuit clock segments & gun ranges

A gently streamlined list of clock segments and ranges for different types of guns:

|                                 	| 0      	| 1      	| 2       	| 3       	| 4      	| 5       	| 6       	|
|---------------------------------	|--------	|--------	|---------	|---------	|--------	|---------	|---------	|
| Pistols                         	| Medium 	| Long   	| Extreme 	| -       	| -      	| -       	| -       	|
| SMGs, shotguns                  	| Short  	| Medium 	| Long    	| Extreme 	| -      	| -       	| -       	|
| Rifles, long arms               	| Short  	| Short  	| Medium  	| Medium  	| Long   	| Extreme 	| -       	|
| Machineguns                     	| Short  	| Short  	| Medium  	| Medium  	| Medium 	| Long    	| Extreme 	|
| Assault cannon, rocket launcher 	| Short  	| Short  	| Short   	| Medium  	| Medium 	| Long    	| Extreme 	|

<!-- | (approximate range in meters)   	| 5      	| 20     	| 40      	| 80      	| 150    	| 500     	| 1000    	| -->

## Vehicle-mounted weapons

If a gun is being used manually (either via a pintle mount or manual/AR remote controls of a mobile turret), the standard roll is Agility+Gunnery. The character can choose to roll Agility+appropriate weapon skill instead with a -2 penalty. Smartgun bonuses apply to both the above rolls if appropriate.

If a turret is being controlled via VR (either a jumped-in rigger or anyone else in VR), it's Logic+Gunnery. 

{{% alert title="TODO" color="warning" %}}
something with sensors that work like smartguns
{{% /alert %}}


## Appendix: some typical vehicle/barrier ratings

Vehicles (ratings are body / armour):

* scooter: 4 / 4
* small car: 8 / 4
* sports car: 10 / 8
* armoured limo: 15 / 15
* SUV: 15 / 12

Barriers (ratings are structure / armour)

* Glass: 1 / 2
* Drywall, plaster, doors: 2 / 4
* Furniture, ballistic glass: 4 / 6
* Trees, hardwood, posts, chain-link fence: 6 / 8
* Security door, armoured glass, Kevlar wall lining: 8 / 12
