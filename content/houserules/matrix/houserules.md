---
title: Matrix houserules
linkTitle: Matrix rules
type: docs
draft: true
date: 2020-07-19
weight: 30
---

## Matrix skills

The skills you use to get stuff done:

* **Computer**

## Matrix actions

### Looking for stuff

Matrix search / Matrix perception

* Computer + Intuition \[Data Processing\]
* against a threshold if searching
* resist if hiding: Logic + Sleaze

### Hacking in

Ways to get access levels on devices, PANs, or hosts.

* aggressively / loudly:
	* Brute Force: Cybercombat + Logic \[Attack\]
	* target is always aware the attack happened
	* 1-2 net hits: User access. 3+ net hits: Admin access.
* sneakily:
	* Probe: Hacking + Logic \[Sleaze\]
	* Backdoor: same

### Matrix attacks

Cybercombat + Logic \[Attack\]

Ways to deal damage or crash software.

Data Spike - net hits + Attack boxes of damage
Jam Signals - add net hits to Noise
Format device - if 1+ net hits, device is scrambled after next reboot

### Manipulating icons (No tests)

Once you have access on an icon, either directly or through the PAN/WAN it is connected to, you can do the following actions to it without any further tests. These are all Complex Actions except where noted.

If you have User level access:

* Edit file (also copy/delete/etc)
* Encrypt file
* Send command (Simple Action)
* Control device (can be Simple or Complex) (test might be required)

If you have Admin level access:

* Reboot device
* Trace icon
* Change icon

### Manipulating icons (Tests)

If you have Admin level access:

* Set data bomb / disarm data bomb (test required)
* Crack file (test required)

### Manipulating datastreams

Electronic Warfare + Logic, limit as below

* Jam signals \[Attack\]
* Snoop \[Sleaze\]
* Spoof command \[Sleaze\]

### Manipulating yourself

(no tests)

* Jack out
* Change AR/VR mode
* Jump into rigged device

### Test resist dice pools

Whenever a character tries to hack something, that something is going to resist. As usual, pool has two parts: one part from an attribute, one part from the device's ASDF stats.

* Attribute: for a persona, use Wil/Int/Log. For a device, use Host rating or Device Rating.
* ASDF:
	* Device: use Rating for D/F, use 0 for A/S
	* Host: use Rating+2 for D/F, use Rating for A/S (most Hosts are defensively configured, can vary if desired)


{{% alert title="TODO" color="warning" %}}
Personas can add dice to this test via an interrupt action
{{% /alert %}} 

### Device ratings

Host ratings: 1-12

Commlink Ratings: 1-7

Device ratings: 1-6

1. Vending machines
2. Public terminals, entertainment machines
3. Standard personal electronics
4. Cyberware, vehicles
5. Alpha grade cyberware, military vehicles 
6. High-end cars


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
