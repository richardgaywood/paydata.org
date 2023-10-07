---
title: The houserules
linkTitle: Rules
type: docs
date: 2020-07-26
weight: 20
description: How to use (most of) the 6e Matrix rules in 5e
categories:
  - archived
aliases: 
  - /archive/matrix_backport/rules  
---
{{% pageinfo %}} 
These rules are canon for my current campaign. However, I am working on superseding them with a set of rules that is further streamlined.
{{% /pageinfo %}}

## Marks: change to access levels

Remove the concept of marks entirely. Replace with three levels of access:

*   **Outsider** access is what you have when you first log into a system, and it doesn’t grant you anything other than the ability to look around and interact with others in the location. Equivalent to 0 marks. A host might or might not allow Outsiders to enter it, depending on its purpose and configuration.
*   **User** access allows you to scan information — read files, perform basic functions, that sort of thing. Equivalent to 1 mark.
*   **Admin** access allows you to change configuration, turn devices on or off, etc. Equivalent to 3 marks.

(Note there is no equivalent to 2 marks, a small efficiency gain. GMs don’t need to track it and deckers don’t need to pass through it on the way to Admin access.)

All iconography around marks is also removed. No more visible marks or designing a mark that matches your persona.

In addition, most of the time, a character’s hack targets will be an entire PAN or WAN, not not an individual device ([see below]({{< relref "rules.md#pans--wans" >}})). Accordingly, access levels are tracked against the entire PAN or WAN. This also reduces book-keeping.

### Programs and effects that depend on marks

There are a variety of things in 5e’s version of the Matrix rules that derive an effect from the number of marks you possess, eg. the Brute Force action does extra Matrix damage, so does the Mugger program, and so on. I am preserving these by ruling that User access is equivalent to 1 mark, and Admin access is equivalent to 3 marks.

## PANs & WANs

For the purposes of this doc, a WAN is a PAN that is run off a host rather than a commlink/cyberdeck/RCC. Same game mechanics, though, just with more dice.

*   The concept of “master” and “slave” devices doesn’t really exist any more as an explicit thing. Devices can be naked on the Matrix or merged into a PAN/WAN. A PAN/WAN is always centered around a commlink, cyberdeck, RCC, or host.
*   If a device is in a PAN/WAN, you cannot hack into it directly via the Matrix. You have to hack the PAN instead. (But see below about direct connections.)
*   Access levels gained against a PAN - User or Admin - apply to every device on the PAN.
*   PAN sizes are essentially unlimited[^5]. I’m just not interested in tracking them, honestly. I will revisit this if it turns out to break anything important.
*   If you can get a direct cable connection to the device, you can hack just the device. It no longer benefits from the stat boosts from being in the PAN/WAN, so now rolls (likely) a pitiful dice pool[^6]. But access levels gained against it still count for the entire PAN/WAN and everything in it.
    *   Yes, physically compromising devices is very powerful. 

## Matrix skills; Matrix attributes (ASDF); deck stats & configuration

No changes to make here.

{{% design %}}
I have rejected several 6e changes. 6e decks can run twice as many programs as in 5e, but I feel that just leads to modifier explosion from too many overlapping effects. 6e also splits the cyberdeck into two components - the 'deck itself and the cyberjack - but this doesn't really change the substance of the system a great deal and makes converting existing characters awkward.
{{% /design %}}

## Matrix damage & repair; dumpshock

Any device that uses the Matrix to function - including any gear like guns and cyberware that have wireless bonuses - incurs dice pool penalties when they take Matrix damage: -1 per three full boxes. This makes Data Spike wielding deckers more dangerous. 

No changes to dumpshock or link-locking.

Your failed Attack actions no longer give you Matrix damage, and your failed Sleaze actions no longer give the target marks against you. 

{{% design %}}
*Rejected rules: 6e also reduces matrix damage and changes the damage resistance test, in line with how normal damage works throughout 6e, but I'd rather keep these rules consistent with 5e's damage model. 6e has a slightly different Matrix repair test using the extended test mechanics, but it's slower to resolve, so I have left it out. 6e changes the damage codes for dumpshock, again to be inline with the reduced damage codes used throughout the edition. This is better left alone in 5e.*

*However, I've kept the changes to failed actions in, because getting hurt just because you failed to hit someone seems un-fun and (more importantly) not at all how any other Shadowrun combat type works. I prefer mechanical consistency across systems, where possible.*
{{% /design %}}

## Matrix modes (AR/VR); initiative

No changes.

{{% design %}}
Rejected rule: 6e reduces VR initiative. As I'm sticking with the 5e action economy in my game, I don't see the need to backport this change. I'm also keeping 5e's +2 dice pool bonus for hot sim VR, as without it hot sim offers a lot of risk for rather modest reward.
{{% /design %}}

## Connections; Noise

No changes.

## Overwatch, GOD, convergence

As in 5e, all hits rolled against the decker in opposed tests on illegal actions add to the Overwatch Score. These are any actions that use the \[Attack\] or \[Sleaze\] stats of your deck to determine their limit.

However, remove the secret +2d6 that is added to OS every 15 minutes. Instead, deckers accumulate OS in three new ways:

* +1 to OS every time they do an action that is affected by any [Hacking program]({{< relref "comparison.md#hacking-programs" >}})
 (see the list on SR5e CRB page 245)
* +1 to OS every combat turn that the decker maintains User access to a host or device that was gained via Brute Force
* +3 to OS every combat turn that the decker maintains Admin access to a host or device that was gained via Brute Force

{{% design %}}
I have elected to keep this change because I'm a bit uncomfortable about the "2d6 every 15 minutes" mechanic. It basically just means "whenever the GM says so", as that's a bit of an arbitrary schedule, and I'd prefer something that is more within the PCs control - ie. whenever they choose to hit the "go loud" button and start using Brute Force.
{{% /design %}}

As before, Overwatch Score is reset when the decker logs out or reboots their deck. And Convergence happens when the Overwatch Score reaches 40, and has the same effects.

{{% design %}}
SR6e does not have the special rules for convergence when inside hosts (instead of decker getting dumped, the host starts launching IC.) I'm keeping those rules as I think it adds more variety.

In addition: in 5e, the deck takes 12 boxes of resisted Matrix damage when Convergence happens. In 6e, it is automatically bricked. The latter can be very dangerous for deckers, as it'll always strip Firewall away from their biofeedback damage resistance test. I prefer the former approach for this reason.
{{% /design %}}

## Grids

Grids add little to the rules beyond book-keeping, and make some stuff confusing. Keep them for fluff and flavour (the Ares grid has Ares propaganda, the Seattle grid has Emerald City spam) but remove all mechanical effects. All hosts and devices are accessible from all grids without penalties.[^7] 

Keep only the -2 dice pool penalty to all actions while using the public grid - it still hurts to be poor, and the free public access grid still sucks.

## Matrix perception & running silent

Three important changes:

*   Drop the -2 dice pool penalty for running silent.
*   Running silent is done at the entire PAN level; it is no longer a per-device setting. This also applies to an entire Shadowrunner team with all their devices being covered by the team decker; either all their stuff is running silent, or none of it. This is a lot easier to track.
*   When attempting to spot icons that are running silent, you no longer need to randomly pick which ones you investigate with Matrix Perception. Instead, you make a single Matrix Perception test (Computer+Intuition [Data Processing]), and each icon running silent makes the opposing dice roll (Logic + Sleaze.) Every icon that fails this test is immediately revealed to you, all in one go.[^8]

Stealth tags are always running silent and resist Matrix perception actions with 10 dice.

## Matrix actions

### Sleaze attacks: Probe / Backdoor Entry

Remove the Hack on the Fly action. Replace it with two new linked actions: 

{{% alert title="PROBE (illegal)" color="gray" %}}
* Hacking+Logic [Sleaze] vs Willpower+Firewall or Firewall x 2 (1 Hour)
* Works at all access levels: Outsider/User/Admin 

You probe a host, PAN, or device for weaknesses, looking to gain access and create a lasting backdoor to the system. You take your time not to alert any security to your presence, and you can create an exploit that may last until you are ready to use it. While not as fast as using Brute Force, Probing a device does not raise an alarm automatically. Even if your attempt initially fails, it will not trigger an alarm unless you glitch. Systems and devices will not detect your presence until you have gained access to them. 

Once you create the exploit, you may then use the Backdoor Entry action at a later time. Net hits on this test count as a dice pool bonus on your future Backdoor Entry test. The duration of these backdoors depends on the device or host—generally speaking, the backdoor lasts for \[10 – Host/Device Rating\] hours. Most systems create a changelog and will automatically correct and report differences to their configurations caused by the presence of these exploits.
{{% /alert %}} 


{{% design %}}
According to Banshee (the Matrix rules author) the intention was that Probe can be repeated, albeit at a cost, using a variation on Shadowrun's usual extended test mechanism. The decker can keep attempting further rolls (at -1 dice pool each time, as usual for extended tests) against a threshold determined by the targeted system's defence roll, all while the Overwatch Score ratchets upward. It's a push-your-luck mechanism.

However the German CRB simply makes Probe a normal opposed test that happens to take one minute of game time to resolve. This is the rule I am applying in my game, principally because I prefer standardised game mechanics to one-off bespoke rules. But also because the former approach can result in a decker putting 50+ dice down on the table across multiple rolls, slowing down gameplay.
{{% /design %}} 

It isn’t completely clear if a decker’s Probe results persist if they log out of the Matrix then log in again later. For these houserules, I am ruling that they do.

Once a decker has successfully run Probe against a target, they can move onto the second new action:

{{% alert title="BACKDOOR ENTRY (illegal)" color="gray" %}}
* Hacking+Logic [Sleaze] vs. Willpower+Firewall or Firewall x 2 (Complex) 
* Outsider

You attempt to use a backdoor you have put in place to gain illicit entry into a host, device, or other Matrix area. This action can only be used if you have previously used Probe on the target successfully; net hits from that successful Probe count as a dice-pool bonus on this test. If the test is successful, you gain Admin access to the target, and it does not count as illegal Admin access (though taking illegal Matrix Actions will still increase your Overwatch Score). 

If this test fails, the backdoor you have made was detected and removed, and you cannot attempt Backdoor Entry again with the same host until a new backdoor is made through the Probe Action. Failing this test does not immediately set off alarms, but the character's OS increases as normal.
{{% /alert %}} 

### Brute Force

By default, a successful Brute Force check grants User access. If the decker wants to go from Outsider to Admin access in one go, they may attempt to do so, at a -6 dice pool penalty (reduced to -4 with the Go Big Or Go Home quality).[^9]

Note that access gained via Brute Force will accrue Overwatch Score as long as the decker maintains the forced access; at a rate of +1 per Combat Turn for User access, or +3 per Combat Turn if the decker has Admin access. So once you use this, the clock is ticking!

Also: Brute Force no longer does optional Matrix damage, in the name of up speeding play and simplifying things. One action = one result.

### Spoof Command

In these houserules, as in SR6e, Spoof Command no longer needs any marks on anything to work. (In SR5e, it requires a mark on an icon that can legitimately command the target device.)

{{% design %}}
The scope of Spoof Command has always been fairly unclear. Can you use it to eject a clip from a smartgun? Can you use it to loop a camera feed? These seem reasonable. Can you use it to shut down an opponent’s wired reflexes or cyberarm? That seems overly powerful, as well as making Spoof Command overlap with other, more explicit methods to achieve that goal (eg Data Spike, Format Device / Reboot device.) Force a hostile drone to fire on its allies? That one seems ok...?

"You spoof a device’s owner’s identity, making the device think that your command is a legitimate one from its owner. ...  This trick only works on devices and agents, not IC, sprites, hosts, personas, or any other icons."

**This needs consideration and playtesting; I don’t have the answers yet.**
{{% /design %}}

### New action: Tarpit

A sort of stun-damage analog to the physical-damage attack of Data Spike:

{{% alert title="TARPIT (illegal)" color="gray" %}}
* Cracking + Logic \[Attack\] vs. Data Processing + Firewall (Complex Action)
* Works at all access levels: Outsider/User/Admin 

Sometimes you want to deliver as much hurt as possible; sometimes you want to deliver a little pain and a little slowness, in order to make the rest of your blows land easier. If you succeed in making this attack, do (1 + net hits) damage to the icon you attacked while also reducing their Data Processing rating by the same amount. If a device's Data Processing rating is reduced to 0, the user cannot perform a Matrix action until it is 1 or more. The Data Processing rating recovers at a rate of 1 point per combat round.
{{% /alert %}}

### New action: Encrypt File

A very minor detail, but this is the counterpart to Crack File. This functionality is in 5e but buried in a weird little alternate mode in a footnote to the Edit File action.

{{% alert title="ENCRYPT FILE (legal)" color="gray" %}}
* Computer + Logic \[Data Processing\] (Complex Action)
* User/Admin 

The hits on the Encrypt File test establish an Encryption Rating that's used to oppose future Crack File attempts.
{{% /alert %}}

### Smaller action changes

There are a large number of small changes to various dice rolls and mechanics for actions throughout 6e. In the main, I am choosing not to include these in my houserules. I don’t think any of them have a drastic effect on gameplay, and they will invalidate the 5e quick reference material I use, which is painful. All these changes are documented in the [Matrix Actions Comparison]({{< relref "comparison.md#actions" >}}) section, if you want to see them.

Here are some smaller changes I do think it’s worth making:

*   **Format device**: treat the repair test for restoring a device as the same as repairing a device bricked through accumulated matrix damage.
*   _...maybe more to come here after playtesting..._

### Removed actions

*   **Invite Mark** - Hosts can now allow access to people with Outsider access level instead, so they no longer need to invite would-be visitors to get one mark first.
*   **Erase Mark** - the only way to erase marks now is to reboot the device. It is unclear how this works in the context of hosts, though.
*   **Hop Grid** - grids are gone, so this is gone.

## Programs

Almost all programs can be left as-is. 6e removes a number of programs that are in 5e ([see the comparison for details]({{< relref "comparison.md#programs" >}})), but they are harmless to leave in place, I think. 6e also changes how a few programs work in order to use the new Edge mechanic; again, this can be ignored.

The only exception is the **Guard** program, which should be removed, as it only works in the context of marks gained against the decker.

{{% design %}}
6e's cyberdecks have double the number of program slots that 5e's do. I am not adopting this rule in my game, as I think it encourages analysis paralysis from players as they try to juggle 8+ programs. It also results in modifier explosion as each program's effects is added together. YMMV.

Additional houserule for my table: Remove the Wrapper program. If it exists, it leads to requirement for endless Matrix Perception tests, slowing down gameplay.
{{% /design %}}

## Hosts & IC

Keep host and IC initiative, stats, and attack rolls the same. [See below for a detailed comparison]({{< relref "comparison.md#hosts--intrusion-countermeasures" >}}), but in general, make the following changes to IC effects:

*   **Hosts no longer get marks on deckers**: this is one less thing to keep track of. IC actions no longer grant marks or require marks. Remove the damage boost related to marks from Black IC, Blaster, etc.
*   **Scramble** forces a reboot at the end of the next Combat Turn[^10]. Otherwise it becomes a bit of a powerful one-blow-knockout against the decker, as it no longer requires any marks against them as a prerequisite.
*   **Acid / Binder / Jammer / Marker**: these are the IC that attack your deck’s Firewall / Data Processing / Attack / Sleaze stats. Change them so that:
    *   They degrade your deck stats by the net hits on their attack roll, not just 1 point.
    *   They do not do Matrix damage.
    *   Stat degradation recovers at the rate of 1 point per minute once the decker has left the host that did the damage.

## Other removed rules

**No -2 dice pool penalty to Matrix actions for running silent** - this is another fiddly detail to remember and easy to forget about. Furthermore, with the move to make running silent a setting that applies to an entire PAN rather than an individual device, it becomes quite painful for players to make decisions about. So it is removed in these houserules, in line with SR6e.

## Rules non-changes

To make it explicit, I don’t suggest changing anything on this list. They should still work fine with the former changes in this section.

*   **Cyberdecks**: Leaving aside the splitting of 5e’s cyberdecks into 6e’s cyberdecks and cyberjacks, the stats are broadly equivalent in both editions. No particular adjustments are needed to 5e’s deck’s stats to fit into the backported rules.

    However, I’d recommend GMs consider reducing the cost of cyberdecks significantly, at least by 50%, perhaps even more... or be prepared to make upgraded cyberdecks an occasional run reward from Mr Johnson, and give all PC's decks plot armour, as losing one will be financially ruinous.
*   **Use of ASDF stats to determine test limits;** also how cyberdeck stats are assigned and moved around between the ASDF slots.
*   All mechanics for what happens when **Convergence** occurs.
*   **Noise** is unchanged in this ruleset, both in terms of how it is calculated and its mechanical effects.
*   **Matrix Search** in 6e appears to have been the victim of mangled editing resulting in dubious maths[^11]. A strict reading of RAW suggests a decker can make an extended test, so rolling 50-100 dice in aggregate, against a results table where 10 hits reveals “deep secrets others are trying to actively hide” - a trivial accomplishment on so many dice. It is best left as-is in 5e, I think.

<!-- Footnotes themselves at the bottom. -->

[^5]: “PAN's were not originally meant to be as restrictive on number of devices as they ended up (if errata does not get approved to change it a good house rule would be to make it Device Rating x3 for max number of devices)” [source](https://forums.shadowruntabletop.com/index.php?topic=30059.msg524805;topicseen#msg524805)

[^6]: This is a houserule; in 6e RAW, direct connection doesn’t grant the firewall bypass.

[^7]: I have little love for the extended test mechanic in general. It’s good in theory, but it simply takes too long to roll 50-100 dice and count the hits.

[^8]: This is the rule in 5e, also, as of Kill Code (see page 32.)

[^9]: Confirmed by Banshee (Matrix rules author) as his intention [here](https://forums.shadowruntabletop.com/index.php?topic=30891.msg533892#msg533892).

[^10]: RAW is one minute; [Banshee originally intended it to be an hour](https://forums.shadowruntabletop.com/index.php?topic=30918.msg534063#msg534063). I prefer his version.

[^11]: Note I have removed the word “extended” here -- see the note below.
