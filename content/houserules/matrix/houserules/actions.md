---
title: Matrix actions
linkTitle: Actions
type: docs
draft: true
date: 2020-07-19
weight: 30
description: A streamlined set of Matrix actions
---

{{% pageinfo %}} 
These rules are *not yet* canon for my current campaign.
{{% /pageinfo %}}

## Test resist dice pools for devices and hosts

All resistance rolls below are expressed as an Attribute plus one of the ASDF stats. However, this only applies when the defender is a persona. When it is a host or device, substitute values for the roll as follows:

* For the resistance Attribute: use the Host Rating or Device Rating.
* For the ASDF stat:
	* Naked/standalone device: use Rating for D/F, use 0 for A/S (unless it's special)
	* Device in a PAN or WAN: use the PAN/WAN controller's ASDF stat 
	* Host: use (Rating+2) for D/F, use Rating for A/S (most Hosts are defensively configured, but this can vary if desired)

{{% alert title="TODO" color="warning" %}}
Personas can add dice to this test via an interrupt action
{{% /alert %}} 

## Just lookin'

* Roll: Computer + Intuition \[Data Processing\]
* Resist: Logic + Sleaze 
  *or* against a threshold

* Matrix search
* Matrix perception

## Getting into places you shouldn't be

Roll: Hacking + Logic \[Attack\] or \[Sleaze\]
Resist: Willpower + Firewall

### Brute Force (aggressively)

Roll: Hacking + Logic \[Attack\]
Resist: Willpower + Firewall

* 1+ net hits gives User access. 
* 3+ net hits allows Admin access at decker's option. (Remember that Admin access accrues OS more quickly.)

### Probe / Backdoor Entry (sneakily)

Roll: Hacking + Logic \[Sleaze\]
Resist: Willpower + Firewall

Ideally, the decker first does **Probe** to scout the target for security vulnerabilities: roll as above, take net hits, split into two groups as decker wants.

* Base time is 60 minutes, divided by the however many hits the decker wants to use to reduce the time.
* Rest of net hits is recorded to use with the Backdoor action later.
* Probe results stay valid for (3d6-Host/Device Rating) hours (minimum 1), but persist if the decker logs out or reboots.

To actually hack the system the decker does **Backdoor Entry** to use the discovered vulnerabilities to get access. Same test as above.

* If the decker didn't do Probe before Backdoor Entry, they take a -6 penalty.
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

Ways to deal damage or crash software. These are all Complex actions.

* Data spike: does (net hits + Attack) boxes of Matrix damage, resisted by the target with Device Rating + Firewall.
* Popup (requires User access): Target must be a persona using AR. Flooded with Matrix spam. Takes (net hits) as a negative ongoing dice pool penalty to all tests until the end of the next turn.
* Denial of Service: Target is one or more specific devices. Target's data streams are polluted with noise. Take 2*(net hits) as an ongoing penalty to all use of the device until the end of the next turn.

  If the decker has no access, this can only be used against a single device. If the decker has User access to a PAN or host, it can be used against up to 3 devices that are in that PAN/WAN. If the decker has Admin access, it can be used on 6 devices. 
  
  "Devices" can include smartguns and cyberware.

## Manipulating icons

Roll: Computer + Logic \[Data Processing\]
Resist: Willpower + Firewall

Once you have access on an icon (or the PAN/WAN that it is part of), you can do the following actions to it without any further tests.

If you have User level access:

* Edit file (no test, Complex action) - create, change, copy, delete, or protect any type of file. 

	Note that some of these actions (particularly copy) may not complete instantly. The decker doesn't need to spend any other actions, but they may need to wait.
	
	If the edit is particularly intricate or tricky, GM may call for a test of Computer + Logic \[Data Processing\] vs a threshold to determine how successful it was.
* Send message (Simple action) - send a message to a person or an order to a drone or other semi-smart device. Can be textual, audio, a picture, or a short video clip.
* Control device (Simple/Complex depending on what you're doing) - may require a test depending on what the goal is eg. shooting a turret requires a Gunnery roll. Control Device cannot override the neural connections used control cyberware.

If you have Admin level access:

* Reboot device (Simple) - you cannot reboot cyberware. Rebooting weapons or vehicles disables their electronic features but they typically still work via manual controls.
* Trace icon (Complex) - see below.
* Snoop (Complex) - if you have Admin access on one of the devices, you can run Snoop without any further tests.
* Change icon (Simple action)

Some actions still need tests however. These both need User level access to the file in question:

* Encrypt file (Complex action) - roll Computer + Logic \[Data Processing\]. Number of hits is the protection rating on the file's encryption.
* Crack file (Complex action) - roll Hacking + Logic \[Attack\] vs protection rating x 2. 

### Trace Icon

**TBD**

## Manipulating datastreams

Roll: Electronic Warfare + Logic
Resist: Willpower + Firewall

These are all Complex actions.

* Snoop (no access required): listen in on the link between any two or more devices. Can be used to monitor a video feed, listen to an audio call, intercept commands sent to drones, etc.

	Note that if you have Admin access to any device in the link, you can perform Snoop without any test being required.
	
	Once you have performed Snoop, you can also insert hacking commands into the datastream to hack the remote device. This can even be achieved if the remote device is outside of local mesh range. Roll Probe/Backdoor Entry/Brute Force as normal.
* Spoof Command (no access required): send a single command to a device, carefully constructed to look like it came from a legitimate source. See below for discussion.
* Subvert Infrastructure (requires User access): Take control of up to (net hits) simple infrastructure devices connected to the PAN/WAN. Control continues as long as the decker maintains access to the host. Examples of devices include traffic lights, vending machines, home appliances, desk lamps, etc. Different commands can be issued to multiple devices for a single Simple action.
* Squelch (no access required): prevents target device from calling or sending any messages for (net hits) number of minutes. If the target is a host subsystem, it prevents alerts leaving that subsystem and deploying IC in other subsystems for (net hits) combat turns.

### Spoof Command

Spoofed commands are considered to have User level access, not Admin.

What you can do with Spoof Command:

* Lock or unlock electronic doors and maglocks
* Tell a camera to replay its last footage endlessly, creating a camera loop
* Tell a drone to target a specific person, as long as that person is not specifically tagged as a friendly
* Tell a drone to cease firing (although its controlling host or rigger will likely tell it to start again soon afterwards)

What you cannot do with Spoof Command:

* Interfere with cyberware - the neural interface used by cyberware overrides commands sent from the Matrix
* Reboot, format, or shut down devices completely - these need Admin level access
* Change a drone's friend-or-foe identifier 

## Manipulating yourself (mostly no tests)

* Switch AR/VR mode
* Jack out (opposed test if link locked)
* Reconfigure deck
* Matrix defence / counterhacking (something like counterspelling?)
