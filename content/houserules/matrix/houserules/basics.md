---
title: Matrix basics
linkTitle: Basics
type: docs
draft: true
date: 2020-07-19
weight: 20
description: Matrix attributes, damage
---

{{% pageinfo %}} 
These rules are *not yet* canon for my current campaign.
{{% /pageinfo %}}

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

## Matrix damage

* Each device has (Device Rating / 2) boxes of Matrix damage.
* Matrix damage is resisted with Device Rating + Firewall.
* Tests using the device take a -1 penalty per 3 boxes of incurred Matrix damage.
