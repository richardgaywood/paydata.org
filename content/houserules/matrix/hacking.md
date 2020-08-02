---
title: Access, getting it, and protecting against hacking
linkTitle: Hacking
type: docs
date: 2020-07-26
weight: 30
---

## Networks

"Naked" devices - low-end things connected directly to the Matrix - are notoriously at risk of being hacked. Most people therefore protect their stuff by creating a Personal Area Network (PAN) and using their commlink as a shield against incoming hacking attempts.

### PANs

Personal Area Networks - PANs - are local networks of devices all sheltered under a controller. The controller must be a device running a persona, so a commlink, cyberdeck, or RCC. The controller monitors all traffic within the PAN and between the PAN and the public Matrix, guarding against hack attacks.

PANs always run across the local mesh part of the Matrix, and have a restricted range to around 500 metres, depending on local network conditions (it gets smaller if the area is noisy). Devices that pass out of range will drop off the PAN. (Note that riggers can extend their PAN to greater ranges for drone control, as their RCCs have heavy-duty antennas. This also makes them physically bulky however.)

PANs can have dozens of devices attached to them; for most game purposes it isn't worth keeping track of.

A device in a PAN can choose to roll the PAN controller's device rating and the PAN controller's ASDF stats instead of its own to defend against any Matrix action. However, it does not have to do so, eg. if it has a better Firewall stat than the controller does.

### WANs

Wide Area Networks - WANs - are very similar to PANs, but the controlling device is a host instead.

Like PANs, WANs only work on the local mesh, so have a restricted range and must be controlled by a local host. Cloud hosts cannot be PAN controllers.

WANs have essentially no limit in how many devices can be attached to them.

It is common for WAN controller hosts used in wageslave offices to be running silent and also protected by RF-blocking building measures. See [spotting]({{< relref "spotting.md" >}}) for more information.

## Access levels

Your persona can have three different access levels to any given device, host, PAN, or WAN on the Matrix:

* **Guest**: the default permission level for persons that are unknown. Sometimes this means you can't access anything, sometimes it means you can go inside a host and interact with some of it. Depends on the host.
* **User**: a normal user's access rights. Can usually read/write files, give standard/routine commands to attached devices. Occasionally very secure devices or files might require Admin access instead.
* **Admin**: full control, can order devices to do anything they can reasonably perform.

These access levels apply to an entire PAN or WAN at once. If you have User access to a PAN, you have User access to every device connected to that PAN. If your persona is running on a device controlling a PAN, then you have always have Admin access to everything in the PAN.

## Direct connection hacking

If an attacker can achieve a direct, physical connection to a device that is part of a PAN or WAN, they can bypass most of the protections. The device must roll its own Device Rating against the hacking attempt, and it is treated as having a Firewall stat of 0.

This is doubly dangerous, as from that compromised device the attacker can move into the rest of the network. Any access levels obtained on the device apply to the entire PAN or WAN.

Direct connections are not always easy to obtain. For many secure devices that use wireless connections to their hosts (eg. an external camera or maglock), they may only be present as physical connection points on the internal mechanisms, hidden behind reinforced casing. These are difficult to jerry-rig.

Some secure devices use wired connections to their WANs instead. These devices are impossible to wirelessly hack, but the tradeoff is that it's much harder to armour their controlling cables and hence a lot easier to attackers to get a physical backdoor.

To achieve a direct connection, roll Hardware + Logic:

* For wirelessly connected devices, use a threshold of (host rating ) / 2 to represent the physical security
* For wired devices, reduce the threshold by 1 (minimum 1) and add +4 to the attacker's roll.

These are not hacking rolls, and there are no implications for OS tracking etc.

## Hacking via Snoop

If a decker is listening in to an active connection (can be a voice call, a video stream, a text message chat, etc) via a Snoop action, they gain extra opportunities to hack remote targets by inserting hacking commands into the datastream.

Unlike other hacking attempts, they do not need to spot their target for this, so they can use this vector to hack one end of a phone call, then hack the device at the other end, even if it not within the decker's local mesh.

* Roll Backdoor Entry or Brute Force (decker's option) as usual.
	* Either action takes 10x longer to perform than usual, because of the need to carefully weave the hacking commands into the datastream; 10 combat turns / 30 seconds.
	* This counts as a directly connected hack, so the device rolls only its Device Rating against the hack attempt, with no Firewall.
	* It is very unlikely the decker will be able to arrange things to make Probe viable due to how long it takes. Remember that Backdoor Entry without Probe first takes a -6 penalty.
	* Brute Force, whether it succeeds or fails, is likely to alert the remote target and cause them to terminate the call.
* Once the decker gains User or Admin access, they can carry out commands as usual and at their usual speed.
	* Trace Icon is a good choice, or Edit File if the decker wants to look around the contents of the device.
* When the call/video stream/etc ends, the decker loses access immediately.