---
date: 2020-07-16
title: Addiction rules
linkTitle: Addiction
type: docs
description: Drugs are bad, mmmkay
weight: 80
aliases: ["/houserules/characters/addiction"]
---

{{% pageinfo %}} 
These rules are **not yet** canon for my current campaign. Although simpler than RAW, they are still too complex, I feel.
{{% /pageinfo %}}

## Addiction qualities

(Unchanged from RAW; repeated here for ease of reference.)

1. Mild (4 karma):  If suffering from withdrawal, the character takes a -2 penalty to all tests that use Physical and/or Mental attributes, depending if the addiction is physiological, psychological, or both.
2. Moderate (9 karma): Withdrawal penalty is now -4.
3. Severe (20 karma): constant -2 to all Social tests as the character's degradation becomes obvious to everyone. Same -4 when in withdrawal as for Moderate addiction.
4. Burnout (25 karma): -3 to all Social tests. -6 penalty to all Mental and/or Physical attribute tests when in withdrawal. 
5. Beyond burnout: each time a character in Burnout fails an addiction test, they permanently lose 1 point from either Body or Willpower, whichever is higher. 

Dry Addict (also in mild/moderate/severe/burnout levels, at 50% of the karma of the above qualities): must pass a composure test at thresholds 1-5 (depending on stress level) to turn down an offer of the addictive substance. Take a 1-4 dice pool penalty on addiction tests following use of substance. 

## Addictive substances

|                             | Addiction Threshold | Recovery Period    | Addiction Period | Addiction Type |
|-----------------------------|---------------------|---------------------|-----------------|----------------|
| Alcohol [*]                 |                   2 |                   1 |               3 | Both           |
| Bliss                       |                   3 |                   1 |               3 | Both           |
| Cram                        |                   3 |                   1 |               3 | Psychological  |
| Jazz                        |                   3 |                   2 |               2 | Both           |
| Kamikaze                    |                   3 |                   3 |               1 | Physiological  |
| Long Haul                   |                   1 |                   1 |               3 | Psychological  |
| Nitro                       |                   3 |                   3 |               1 | Both           |
| Novacoke                    |                   2 |                   2 |               2 | Both           |
| Zen                         |                   1 |                   1 |               3 | Psychological  |
| BTL (Dreamchip)             |                   1 |                   2 |               2 | Psychological  |
| BTL (Moodchip)              |                   2 |                   2 |               2 | Psychological  |
| BTL (Personafix)            |                   2 |                   2 |               2 | Psychological  |
| BTL (Tripchip)              |                   3 |                   2 |               2 | Psychological  |
| Essence Drain               |                   2 | (Critter's Magic)/3 | [*]             | Psychological  |

<!-- unused entries
| Deepweed [*]                | ?                   | ?                   | ?               | Physiological  |
| Soykaf [*]                  |                   2 |                   0 |               4 | Physiological  |
| Focus [*]                   |                   2 | (Total Force)/3     | [*]             | Psychological  |
| Skillwires [*]              |                   2 |                   1 |               3 | Psychological  |
| Legal-Strength Simsense [*] |                   1 |                   0 |               4 | Psychological  |
| Hot-Sim Simsense [*]        |                   1 |                   1 |               3 | Psychological  |
| Psyche [*]                  |                   2 |                   2 |               2 | Psychological  |
-->

{{% alert title="Notes"%}}
For the purposes of my campaign, I won't be enforcing addiction rolls against soykaf, skillwires, simsense, or foci. I've removed them from the table above. I will only ask for rolls for addiction to alcohol when the character already has the qualities ie. an existing addiction can get worse but a character cannot acquire an addiction during play.

I've also deleted psyche completely. Deepweed has no addictiveness ratings in CRB, nor in any errata I can find. I've left it out for now. 

Addiction Period is a new field, calculated as RAW's "addiction rating" divided by 3. Recovery Period is calculated as (4-Addiction Period.) You can use these formulae to work out the stats for other drugs in SR5e not included above. That's also how you calculate the values for Essence Drain addiction, should it come up.
{{% /alert %}}

## Addiction tests

When asked to roll an Addiction or Withdrawal test, the dice roll is:

* Physiological: Body + Willpower vs Addiction Threshold for the drug
* Psychological: Logic + Willpower vs Addiction Threshold
* Both: roll both tests, if *either* fails then the whole test fails

## Addiction during missions

If you have an addiction and start a mission after not indulging in your addiction during the last downtime, you must roll for **withdrawal**. Roll an addiction test as above. If you fail, you take an ongoing penalty on all rolls, according to your addiction level, as listed above. This will vanish immediately if you use the drug again.

If you use any addictive drugs during the mission that you do not already have an addiction to, make a note that during the next downtime you will experience **cravings**.

## Addiction during downtime

### Cravings

Drugs are more-ish. That's kinda their whole deal.

After any use of an addictive substance, your character will crave it. This will last for a number of downtime sessions equal to the drug's Addiction Period. Keep track of how many missions you use the drug on while this is happening.

At the end of the Recovery Period, make an Addiction Test. Subtract one from the drug's Addiction Threshold for each entire mission where you didn't use the drug at all. You cannot use Edge on this test. If you pass the test, the cravings end and you're in the clear. If you fail the test, bad news: you now have the Addict (Mild) quality.

Characters with the Dry Addict quality take a penalty of -1 to -4 on this test, depending on the level of their former addiction. In addition, if they fail the test, they get the Addict quality at the same level as their Dry Addict quality, not at the Mild level.

If you pick up an addiction quality this way, you do not receive any karma for it.

### Addiction-related downtime scenes

Addictions place certain requirements on you between your missions, as per [my downtime houserules]({{< relref "downtime_shadowrun.md#addiction-related-activities" >}}).

You can choose to **Indulge** your addiction. This means you will suffer no ill-effects during your next mission. However, you lose a number of downtime scenes according to your addiction level:

* Mild - 0 scenes lost
* Moderate - 1 scene
* Severe - 2 scenes
* Burnout - 4 scenes (this means you will not be able to do a Leisure scene, so will not heal stun damage or recover Edge during downtime. Yes, this hurts.)
	
Instead of indulging, you can **go cold turkey**: you will have to roll for withdrawal at the start of your next mission, and take the penalty for withdrawal if you fail (or choose to get a fix during your next mission.)

Finally, you can choose to **rehab**, for 1-3 scenes of time. Each scene will grant you +2 dice on your next Addiction Test. There is an escalating cost associated with this, as your character spends time in therapy, purchases detox meds, undergoes magical treatments, etc. In a given downtime phase, the first rehab scene costs 1000¥, the second costs 2500¥, and the third costs 10k¥.

## The downward spiral

After a number of consecutive downtime phases and missions during which you indulge your addiction equal to the drug's Addiction Period, you must roll an Addiction Test. You cannot use Edge on this test. If you fail, the addiction gets one step worse (Mild -> Moderate, Moderate -> Severe, etc.) You do not gain karma for the worsening addiction. If you are at Burnout and fail this test, you stay at Burnout, but also permanently lose one point of either Body or Willpower - whichever is higher.

## Getting clean

To get clean, a character must:

* Successfully go cold turkey for Recovery Threshold downtime phases in a row
* not have used the drug during missions 
* make one final successful Addiction Test (you can use Edge on this test, but this Edge will not return until after your next Downtime phase.)
* and pay the karma to buy off the negative quality (at 1x price, so 4 karma for a Mild addiction.)

They can then swap the Addiction quality for Dry Addiction. They do not receive karma for this new negative quality.

After another period of (Recovery Threshold) downtimes of complete abstinence (ie. you cannot have rolled any Addiction Tests at all), they can once again pay karma (at 2x the cost of the Dry Addict quality) to remove that as well.
