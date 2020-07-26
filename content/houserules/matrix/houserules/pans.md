---
title: PANs & WANs
linkTitle: PANs
type: docs
draft: true
date: 2020-07-19
weight: 27
---

{{% pageinfo %}} 
These rules are *not yet* canon for my current campaign.
{{% /pageinfo %}}

Personal Area Networks - PANs - are local networks of devices all sheltered under a controller device. The controller must be a device running a persona, so a commlink, cyberdeck, or RCC. The controller monitors all traffic within the PAN and between the PAN and the public Matrix, guarding against hack attacks.

PANs always run across the local mesh part of the Matrix, so have a restricted range to around 100 metres. Devices that pass out of range will drop off the PAN.

PANs have essentially no limit in how many devices can be within them.

A device in a PAN can choose to roll the PAN controller's ASDF stats instead of its own to defend against any Matrix action. However, it does not have to do so, eg. if it has a better Firewall stat than the controller does.

### WANs

Wide Area Networks - WANs - are very similar to PANs, but the controlling device is a host instead.

Like PANs, WANs only work on the local mesh, so have a restricted range and must be controlled by a local host. Cloud hosts cannot be PAN controllers.

It is common for PAN controller hosts to be running silent. See [spotting]({{< relref "spotting.md" >}}) for more information.
