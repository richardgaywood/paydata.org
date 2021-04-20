
---
title: Additional rules
linkTitle: Additional rules
type: docs
description: Extra bits and pieces
date: 2020-11-27
weight: 800
aliases: ["sprawlrunners/deckers/additional_rules.md"]
---

## Commlink defence programs

Occasionally, particularly cautious people might spend some extra cash on defences for their commlink. These all require a commlink of d6 rating or higher; lesser devices don't have the processing power required. Only one of the following options can be used.

* **Active integrity checking**: the commlink devotes a significant portion of its processing power to conducting internal scans, and a significant portion of its storage to storing known-good states that it can roll back to in an emergency. This provides a measure of defence against cybercombat. The device can use its Hardening stat in place of its Firewall stat.
* **Encrypted storage**: all files in the commlink's storage are encrypted, with a rating equal to the commlink's dice rating.
* **Parabellum**: the commlink runs a limited form of the Killer ICE. Each time a decker fails a Sleaze Hack or attempts a Cybercombat or DoS Hack against the commlink, the ICE will automatically respond with a counterattack, rolling the commlink's Rating vs the cyberdeck's Firewall. If it hits, it deals Rating+d4 matrix damage (+d6 on a raise).

## Back doors

If a decker can get physical access to debug ports on a device, they can get easier access to hack into it. They take +2 on the Sleaze Hacking roll.

This can be used when hacking unattended devices or commlink networks but it becomes particularly potent when hacking networks controlled by hosts. The bonus applies if the decker can access *any device in the host's network*, as well as any ports that are part of the host infrastructure itself.

To hack a host through a network device, the decker usually requires a toolkit and a roll of the lower of their Electronics and Repair to open up the device and hook up the necessary connections. If the decker succeeds, they take +2 on all actions in the connected host node.

Host sysadmins are aware of this weakness, and do not usually put external devices like cameras or maglocks onto networks for that reason. Security networks tend to be reserved for more serious defences that are harder to get near, like turrets or security guard's weapons.
