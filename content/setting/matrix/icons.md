---
title: Matrix icons
linkTitle: Icons
type: docs
description: How things look in the Matrix
date: 2020-12-24
weight: 150
---

When you view the world in AR, your commlink or cyberdeck can overlay [icons]({{< relref "icons.md" >}}) for any (and all) nearby matrix devices onto your vision. This is rather overwhelming - in an urban area, the local mesh can contain thousands of icons. So most people run filtering routines that hide most of them and only show ones deemed important. For example, in a crowded street, you might only show icons for commlinks for people you know, and hide the rest.

The mesh networking routing protocols that keep the wireless matrix working tracks the approximate position and motion of all these devices, so it can predict when devices are about to go out of range of each other and have fallback routes prepared to keep traffic flowing. AR leverages this information to position icons in the user's sensorium in vaguely the correct place, relative to where the device is. 

When the user has line-of-sight to the device, this positioning is quite accurate; glance at a coffee machine in AR and you'll see its glowing matrix icon hovering just over it. When there's no line of sight, position accuracy drifts randomly, often by a few metres. If you are in a shopping mall and your friend is in the store a few doors down from you, you'll see an icon for their commlink, but it'll appear vague and fuzzed-out so you know it's only an approximate position.

When using VR inside a host, there is no need to make things correspond to meatspace. Icon positioning is arbitrary and governed by the sculpting of the host. Some hosts look like glowing neon wireframes, with icons clustered across an infinite 2d plane. Others are painstakingly rendered 3d environments with icons grouped logically and scattered across rooms or areas. The possibilities are limitless.

## Types of icon

* **Tags**: tiny, passive chips; see [Tags]({{< relref "other_stuff.md#tags" >}}).
* **Files**: any type of data (text, audio, video, computer code, ...), stored on any type of medium (in a tag, on a commlink, in a host, on a storage chipdrive, ...).
* **Devices**: toasters, cars, door locks, speakers, cameras, drones, microwaves, etc etc etc. In the Sixth World, near enough everything that has electrons flowing through it also has a functioning Matrix connection of its very own.
	* **Commlinks**: special devices that people use to see and interact with the Matrix.
	* **Cyberdecks**: souped-up commlinks that can be used to bend the rules of the Matrix by hackers and counter-hackers. There are also **drone decks**, specialised variants used by riggers to control drone networks.
* **Hosts**: the "servers" of the Matrix; big computer systems you can go into in VR and do stuff within. Some hosts are so big that internally they are sub-divided into zones called **nodes**.
	* Inside hosts, you can see (lots of!) icons for files and connected devices. 
	* Hosts also contain **personas**, which are VR icons representing people using the host. Personas can be very simple and generic, or highly customised and tailored to the person they represent. See [Personas]({{< relref "other_stuff.md#personas" >}}). 
	* Hosts also contain **ICE**, intrusion countermeasure electronics. These are autonomous software agents that form the first line of defence against hostile deckers.

