---
title: Common Matrix actions & how to do them
linkTitle: How do I...
type: docs
date: 2020-07-19
weight: 500
description: Short examples of common tasks for criminals
aliases: ["/houserules/matrix/how_do_i"]
---

* **Spy on phone calls**: run Snoop while you have spotted one or more personas on the call. Once you run Snoop, you automatically spot all personas on the call, regardless of where they are.
* **Trace phone calls** even if you haven't spotted the icon on the other end of the call:
	1. have Admin access on one of the devices on the call *or* place the call from one of your own devices *or* have successfully Snooped the call
	2. Probe or Brute Force the device at the other end to get Admin access to it
	3. Trace Icon (no test required)
* **Mess with people's cyberware or weapons**: Spoof/Send Command doesn't work against cyberware, as the user's neural commands override any commands send from the Matrix. See instead the options under [Matrix Attacks]({{< relref "shr-matrix-actions.md" >}}).
* **Disable security cameras** if they are wirelessly connected:
	* With Outsider access: Spoof Command
	* With User access: Send Command to loop them
	* With Admin access: Send Command to shut them down
* **Bypass a host's firewall** via a device that is hardwired to the host:
	* Find the port on the device (might be armoured/hidden and require a Hardware roll to open it up)
	* Roll Hacking against the device's own rating, with no Firewall from the Host
	* Any access levels you get from this test are applied to the entire Host WAN
* **Spot icons inside a host**: By default, most personas connected to a secure Host (eg for work) will run silent, so drop off the public grid. Run Matrix Perception test as usual to spot them and initiate a hack.
