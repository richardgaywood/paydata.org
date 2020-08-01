---
title: Access, getting it, and protecting against hacking
linkTitle: Hacking
type: docs
draft: true
date: 2020-07-26
weight: 30
---

## Networks

"Naked" devices - low-end things connected directly to the Matrix - are notoriously at risk of being hacked. Most people therefore protect their stuff by creating a Personal Area Network (PAN) and using their commlink as a shield against incoming hacking attempts.

### PANs

Personal Area Networks - PANs - are local networks of devices all sheltered under a controller. The controller must be a device running a persona, so a commlink, cyberdeck, or RCC. The controller monitors all traffic within the PAN and between the PAN and the public Matrix, guarding against hack attacks.

PANs always run across the local mesh part of the Matrix, and have a restricted range to around 500 metres, depending on local network conditions (it gets smaller if the area is noisy). Devices that pass out of range will drop off the PAN. (Note that riggers can extend their PAN to greater ranges for drone control, as their RCCs have heavy-duty antennas.)

PANs can have dozens of devices attached to them; for most game purposes it isn't worth keeping track of.

A device in a PAN can choose to roll the PAN controller's ASDF stats instead of its own to defend against any Matrix action. However, it does not have to do so, eg. if it has a better Firewall stat than the controller does.

### WANs

Wide Area Networks - WANs - are very similar to PANs, but the controlling device is a host instead.

Like PANs, WANs only work on the local mesh, so have a restricted range and must be controlled by a local host. Cloud hosts cannot be PAN controllers.

WANs have essentially no limit in how many devices can be attached to them.

It is common for WAN controller hosts used in wageslave offices to be running silent and also protected by RF-blocking building measures. See [spotting]({{< relref "spotting.md" >}}) for more information.

## Access levels

Your persona can have three different access levels to stuff on the Matrix:

* **Guest**: the default permission level for persons that are unknown. Sometimes this means you can't access anything, sometimes it means you can go inside a host and interact with some of it. Depends on the host.
* **User**: a normal user's access rights. Can usually read/write files, give standard commands to attached devices.
* **Admin**: full control, can order devices to do anything they reasonably can perform.

These access levels apply to an entire PAN or WAN at once. If you have User access to a PAN, you have User access to every device connected to that PAN.
