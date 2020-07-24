---
title: Matrix actions
linkTitle: Actions
type: docs
draft: true
date: 2020-07-19
weight: 30
---

{{% pageinfo %}} 
These rules are *not yet* canon for my current campaign.
{{% /pageinfo %}}

## Recon

* Roll: Computer + Intuition \[Data Processing\]
* If resisted: Logic + Sleaze
	* Or against a threshold for Matrix Search

* Matrix search
* Matrix perception

## Getting in

Roll: Hacking + Logic; \[Attack\] or \[Sleaze\]
Resist: Willpower + Firewall

### Brute Force (aggressively)

Roll: Hacking + Logic \[Attack\]
Resist: Willpower + Firewall

* 1+ net hits gives User access. 
* 3+ net hits allows Admin access at decker's option. (Remember that Admin access accrues OS more quickly.)

### Probe / Backdoor Entry (sneakily)

Roll: Hacking + Logic \[Sleaze\]
Resist: Willpower + Firewall

First do **Probe** to scout for security vulnerabilities: take net hits, split into two groups as decker wants.

* Base time is 60 minutes, divided by the however many hits the decker wants to use to reduce the time.
* Rest of net hits is recorded to use on the Backdoor action later.
* Probe results stay valid for (3d6-Host/Device Rating) hours, but persist if the decker logs out or reboots.

Once Probe is successful, at some point later the decker can do **Backdoor Entry** to use the discovered vulnerabilities to get access. Same test as above.

* 1+ net hits gives User access.
* 3+ net hits allows Admin access at decker's option. (Remember Admin access accrues OS more quickly.)
* Even after the decker trigger's GOD's interest, if they are only maintaining access to systems that was gained via Probe then OS does not start accruing for a number of combat turns equal to the hits left over from the Probe test. After that it accrues as normal.

{{% alert title="Example" %}}
Probe opposed test has 4 net hits. Decker uses 2 hits to reduce the time, keeps the other 2 hits back. The Probe action takes 30 minutes.

Decker rolls for Backdoor Entry and gets 4 net hits, choosing to take Admin access. They're not maintaining access to any other systems. Later, the decker has to use a Data Spike against hostile IC. That would normally start the Overwatch Score clock, but the decker has 2 Combat Turns before that happens because of the Probe result.

If the decker then goes on to Brute Force a second system, the OS score starts counting up immediately, including for the first system that was hacked via Probe.
{{% /alert %}} 


## Matrix attacks

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

## Manipulating icons

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


## Datastreams

Roll: Electronic Warfare + Logic
Resist: Willpower + Firewall

* Snoop (if you don't have admin access on one of the devices)
* Spoof Command

## Manipulating yourself (mostly no tests)

* Switch AR/VR mode
* Jack out (opposed test if link locked)
* Reconfigure deck
* Matrix defence / counterhacking (something like counterspelling?)


## Test resist dice pools for devices and hosts

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