---
title: Matrix houserules
linkTitle: Matrix rules
type: docs
draft: true
date: 2020-07-19
weight: 30
---

## Matrix basics

This is covered in more detail in [Matrix fundamentals]({{< relref "fundamentals.md" >}}) in my fluff writeup, but a quick summary:

* Devices (in the real world) have icons (in the Matrix).
* Commlinks/cyberdecks/RCCs being used by a person have a special type of icon called a persona.
* The Matrix comes in two parts:
	* the local mesh is a peer-to-peer network of devices routing traffic between themselves; typically extends a kilometre or so in an urban area (more in rural areas). It's vulnerable to signal disruption and has limited range.
	* the backbone is a world-wide network of fibre cables, satellite links, and other high-tech stuff that carry data around at approximately infinite capacity and speed. 
	* the local mesh and the backbone are bridged by uplink nodes, which are well-guarded hosts
	* devices send traffic between each other until it reaches an uplink node, at which point it is whisked away to the backbone.
* Hosts are the 'servers' of the Matrix
	* Some are "local hosts" - hosts that only work with devices within local grid range. These are smaller / cheaper. 
	* Others are "cloud hosts." These are connected to the backbone so are accessible world-wide. They are larger / more expensive.

{{% alert title="Notes" %}}
Real-world analogies: the local mesh is a bit like your wifi network (but bigger), the uplink node is a bit like your router, and the upper grid is a bit like the current-day internet. 
{{% /alert %}} 


## Matrix attributes

Unchanged from RAW; used as a combination of limits for tests and part of a dice pool for resisting tests done against you.

* Attack
* Sleaze
* Data Processing
* Firewall

## Cyberdecks

Stats are unchanged from RAW; Cyberdecks have an attribute array that can be allocated across the four Matrix stats. Takes a Free action to swap any two stats. Remember you can only do one Free action per turn. If you want to do more reconfiguring than that, you can use Matrix Simple Actions.

Cyberdecks are reduced in price to 25% of RAW. See [the gear houserules]({{< relref "electronics.md#cyberdecks" >}}) for more information and statblocks.

## Matrix damage

* Each device has (Device Rating / 2) boxes of Matrix damage.
* Matrix damage is resisted with Device Rating + Firewall.
* Tests using the device take a -1 penalty per 3 boxes of incurred Matrix damage.
* 

## Skills

* **Electronics** skill group:
	* **Computer**: for doing legal activities
	* **Hardware**: for repairing Matrix damage
	* **Software**: for creating 0-days and other coding tasks
* **Cracking** skill group:
	* **Electronic Warfare**: for attacking or manipulating the wireless signals between devices
	* **Cybercombat**: for attacking icons loudly and aggressively
	* **Hacking**: for getting access levels on devices, PANs, or WANs

## Matrix Actions

### Test resist dice pools for devices and hosts

All resistance rolls are expressed as an Attribute plus one of the ASDF stats. However this only applies when the defender is a persona. When it is a host or device, substitute values for the roll as follows:

* For the resistance Attribute: use the Host Rating or Device Rating.
* For the ASDF stat:
	* Device: use Rating for D/F, use 0 for A/S (unless it's special)
	* Host: use (Rating+2) for D/F, use Rating for A/S (most Hosts are defensively configured, but this can vary if desired)

This means it's typically one of these outcomes:

* Device Rating (commlink or other device resisting with A/S)
* Device Rating * 2 (commlink resisting with D/F)
* (Host Rating * 2) (Host resisting with A/S)
* (Host Rating * 2) + 2 (Host resisting with D/F)

{{% alert title="TODO" color="warning" %}}
Personas can add dice to this test via an interrupt action
{{% /alert %}} 

### Looking for stuff

* Roll: Computer + Intuition \[Data Processing\]
* If resisted: Logic + Sleaze
	* Or against a threshold for Matrix Search

* Matrix search
* Matrix perception

### Hacking in to get access

Roll: Hacking + Logic; \[Attack\] or \[Sleaze\]
Resist: Willpower + Firewall

#### Brute Force (aggressively)

Roll: Hacking + Logic \[Attack\]
Resist: Willpower + Firewall

* 1+ net hits gives User access. 
* 3+ net hits allows Admin access at decker's option. (Remember that Admin access accrues OS more quickly.)

#### Probe / Backdoor Entry (sneakily)

Roll: Hacking + Logic \[Sleaze\]
Resist: Willpower + Firewall

First do **Probe** to scout for security vulnerabilities: take net hits, split into two groups as decker wants.

* Base time is 60 minutes, divided by the however many hits decker wants to use to reduce the time.
* Rest of net hits is recorded to use on the Backdoor action later.
* Probe results stay valid for (3d6-Host/Device Rating) hours, but persist if the decker logs out or reboots.

Once Probe is successful, at some point later the decker can do **Backdoor Entry** to use the discovered vulnerabilities to get access. Same test as above.

* 1+ net hits gives User access.
* 3+ net hits allows Admin access at decker's option. (Remember Admin access accrues OS more quickly.)
* OS does not start accruing for a number of combat turns equal to the hits left over from the Probe test. After that it accrues as normal.

### Matrix attacks

Roll: Cybercombat + Logic \[Attack\]
Resist: Willpower + Firewall

Ways to deal damage or crash software.

* Data spike (Complex): does (net hits + Attack) boxes of Matrix damage, resisted by the target with Device Rating + Firewall.
* Popup (Simple?): Target must be a persona in AR. Flooded with Matrix spam. Takes (net hits) as a negative ongoing dice pool penalty until the end of the next turn.
* Denial of Service (Simple?):
* Subvert infrastructure

{{% alert title="Notes" %}}
removed: crash program

add other actions from Kill Code here for decker-to-non-decker combat 
{{% /alert %}} 

### Manipulating icons

Roll: Computer + Logic \[Data Processing\]
Resist: Willpower + Firewall

Once you have access on an icon (or the PAN/WAN that it is part of), you can do the following actions to it without any further tests. These are all Complex Actions except where noted.

If you have User level access:

* Edit file (no test, Complex action)
* Send command (no test, Simple action)
* Control device (can be Simple or Complex)

If you have Admin level access:

* Reboot device (Simple)
* Trace icon - gives you location not just right now, but live tracking for (3d6-Device Rating) hours or until the device owner reboots it
* Snoop (if you have Admin access on one of the devices)
* Change icon

Some actions still need tests however. 

User level access:

* Encrypt file

Admin level access:

* Set data bomb / disarm data bomb 
* Crack file


### Datastreams

Roll: Electronic Warfare + Logic
Resist: Willpower + Firewall

* Snoop (if you don't have admin access on one of the devices)
* Spoof Command

### Manipulating yourself (mostly no tests)

* Switch AR/VR mode
* Jack out (opposed test if link locked)
* Reconfigure deck
* Matrix defence / counterhacking (something like counterspelling?)

## Device ratings

* Hosts: 1-12
	* Typically, A/S are (Host Rating) and D/F are (Host Rating + 2)
* Commlinks: 1-7
	* A/S are 0, D/F are (Device Rating)
* Other devices: 1-6
	* Vending machines: 1
	* Public terminals, entertainment machines: 2
	* Standard personal electronics: 3
	* Basic/alpha cyberware, basic vehicles: 4
	* Beta/delta cyberware, expensive vehicles: 5
	* Milspec: 6 

## Overwatch & GOD

Overwatch is a 12-segment clock. Clock is public. (Delete: baby monitor program, check OS action.)

The clock ticks up when:

* +1 on any Attack roll, success or failure
* +1 on any failed Sleaze roll
* +1 per combat turn if maintaining user access to any systems *after* rolling any attack roll or failing any sleaze roll
	* increase to +2 if maintaining admin access
	* if the intrusion was via a successful Probe / Backdoor Entry, there is a grace period before the clock starts incrementing; see above.

The clock resets only when the deck reboots and the decker's persona logs off entirely. The decker loses all access to systems at that time, although any vulnerabilities discovered through Probe remain active.

### Convergence

Once the clock fills, GOD is onto the decker. A Demi-GOD starts tracing them.

At the end of each turn, the demiGOD rolls a number of dice equal to the clock vs a resistance from the decker of Intuition + Sleaze. If there are any net hits, the decker suffers convergence immediately. If there aren't, the number of hits (not net hits) are added to the clock, and the demiGOD will roll again at the end of the next turn.



## Hosts

### Host types

There are 

For more information, see [Matrix fundamentals]({{< relref "fundamentals.md#hosts" >}}) 


### Subsystems

## Programs

Maybe 

* decrease to ((Deck Rating) / 2) slots?
* add a few more impactful ones?
* add a one-shot +2 dice boosts that burn out after use? (like trinkets) (deckers craft these with Software in downtime?)

## Agents

* Deck can only run agents of a rating equal to or less than the deck rating
* Agent stats are equal to the deck rating and deck's ASDF, agent skills are equal to its rating
* If used to assist the decker on an action, it takes a Simple Action to order the agent to help. Then it rolls its dice pool as a teamwork test.

## How do I...

* **Spy on phone calls**: run Snoop while you have spotted one or more personas on the call. Once you run Snoop, you automatically spot all personas on the call, regardless of where they are.
* **Trace phone calls** even if you haven't spotted the icon on the other end of the call:
	1. have Admin access on one of the devices on the call *or* place the call from one of your own devices *or* have successfully Snooped the call
	2. Probe or Brute Force the device at the other end to get Admin access to it
	3. Trace Icon (no test required)
* **Mess with people's cyberware or weapons**: Spoof/Send Command doesn't work against cyberware, as the user's neural commands override any commands send from the Matrix. See instead the options under Matrix Attacks above.
* **Disable security cameras** if they are wirelessly connected:
	* With Outsider access: Spoof Command
	* With User access: Send Command to loop them
	* With Admin access: Send Command to shut them down
* **Bypass a host's firewall** via a device that is hardwired to the host:
	* Find the port on the device (might be armoured/hidden and require a Hardware roll to open it up)
	* Roll Hacking against the device's own rating, with no Firewall from the Host
	* Any access levels you get from this test are applied to the entire Host WAN
* **Spot icons inside a host**: By default, most personas connected to a secure Host (eg for work) will run silent, so drop off the public grid. Run Matrix Perception test as usual to spot them and initiate a hack.




{{% alert title="CRB contents" %}}
1. Matrix skills
2. Matrix attributes - ASDF
3. Cyberdecks - allocating attributes, stats
4. Matrix damage - bricking, repairing, biofeedback, dumpshock, link-locking
5. User modes - AR, cold/hot sim VR
6. Connections - noise
7. Failed illegal action consequences (attack -> damage)
8. Overwatch Score, convergence
9. Direct connections
10. PANs, WANs
11. Grids
12. Devices, personas
13. Matrix Perception, spotting, running silent, noticing hackers
14. Marks, owners
15. Actions
16. Programs
17. Agents
18. Hosts - archived files, attributes, host convergence, IC

{{% /alert %}} 



## Appendix: Design notes

Some loose, probably incomplete notes on why I've changed some of the things I've changed.

* Splitting the Matrix into local mesh / backbone: intended to justify why deckers have to get out into the field. 
