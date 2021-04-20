---
title: Hacking the Matrix
linkTitle: Hacking the Matrix
type: docs
description: Bending the Matrix to your will
date: 2020-11-21
lastmod: 2020-12-24
weight: 500
---

## The end of encryption

The incorporation of early quantum processors into the first cyberdecks sent an earthquake through the tech world from which it never recovered. Even the strongest, best designed encryption of the day fell before it in fractions of a second. There could be no more secrets. 

Today, things have improved only slightly; the most advanced encryption in the world still cannot hold up to sustained assault from a skilled hacker with high-end cyberdeck.

This single innovation has reshaped the world.

## Rise of the spiders

Faced with the total loss of passive defence - ie. strong encryption of data - the megacorps had to pivot to active defence. 

First, they built high walls around their kingdoms. Some of the most sophisticated pseudo-AI on the planet exists to run ICE: Intrusion Countermeasure Electronics. ICE patrols and defends the megacorp's hosts tirelessly, rooting out invading hackers and - sometimes - frying their brains.

But ICE isn't all-powerful, so the corps also set people to guard those walls. These counter-hackers, called *spiders* in the language of the street, sit in the middle of sprawling webs of sensors and alarms. Attract their attention, and they are swiftly dispatched to deal with you. And they are *good*, with all the equipment and training of their deep-pocketed masters.

## The Grid Overwatch Division (GOD)

Each megacorp can hire its own security staff to patrol its own hosts, but that leaves the backbone itself vulnerable to attacks. It's too important to leave undefended, so the Corporate Court formed the Grid Overwatch Division (GOD). GOD is a semi-autonomous organisation, tasked with defending public grid infrastructure, staffed by spiders and technicians loaned from the AA and AAA megacorps.

## How to hack

Sending hacking traffic over the backbone is near-impossible. The uplink nodes are equipped with powerful coprocessors that carry out deep packet inspection, scanning for anything out of the ordinary. At the first sign of trouble, aggressive autonomous agents are deployed, rapidly followed by elite GOD spiders.

It is on the local mesh where the deckers can bring their powers to bear. Hampered by the need to maintain backwards compatibility with millions of devices that have fallen into planned obsolescence, and with even small changes to the protocols requiring dozens of squabbling corps to agree, the local mesh is... well, it's a mess. Deckers exploit this ruthlessly, using vast databases of known vulnerabilities to carve through the laughable defences that devices rely on.

There is an obvious problem, though - the local mesh is small, typically extending only 50-100 metres. With the wireless matrix, Deckers need to get close to their targets. They can no longer sit in the safety of armoured bunkers, hundreds of miles from danger.

## What to hack

{{% alert title="TODO" color="warning" %}}*below contains obsolete references to PANs/s-PANs/WANs; I've dropped this terminology in the latest iteration of these houserules*{{% /alert %}} 

Any device that is attached directly to the matrix is considered to be *unattended*. Civilian and even security grade unattended devices have very weak defences against hacking. 

Most ordinary people will arrange all of their various matrix gadgets into a personal area network (PAN.) A PAN is controlled and monitored by their commlink, which routes all matrix traffic through itself. Devices in a PAN cannot be hacked individually; instead, the decker must hack the commlink instead. PANs are a little bit more difficult to hack than an unattended device, but the main benefit is that if the commlink notices the hack attempt it can alert the owner at once. They can then take action, such as shutting down their devices.

The corporate grown-up version of a PAN is a wide area network, or WAN. WANs are very similar but instead of a commlink they are controlled and monitored by a host. As with a PAN, you cannot hack individual devices in a WAN; you have to enter VR and hack the host directly. If you can get a direct cabled connection to a device that is part of the WAN, you can exploit that to more easily hack the host. For this reason, corps tend not to put easily-accessed exterior building defences like cameras or maglocks on their primary security WANs.

Finally, there are also secure PANs, or s-PANs. S-PANs are PANs that are run from a cyberdeck or drone deck and are being actively monitored by a decker or rigger. S-PANs cannot be hacked at all, as their admin will swiftly notice any hack attempts and take defensive action. They can only be knocked offline via cybercombat.

{{% alert title="A note about hosts" %}}*Sprawlrunners RAW describes very large hosts that are made up of many, many nodes, arranged in sprawling, labyrinthian structures. I do not plan to use this (typically, at least). Most hosts in my game will either have a single node that takes care of everything; or they will be divided into a handful of nodes, each dedicated to a task (eg. file storage, building system control, security.) Each node can typically be accessed from any other node; there is no internal "map" as such.*{{% /alert %}} 

## Alarms

The local mesh protocols specify that all devices monitor all the traffic they can see to scan for hack attempts. This isn't hard to avoid in the short term, but as a decker carries out more and more hacks using the local mesh against devices and PANs, it gradually becomes more and more difficult to hide. Once it reaches a critical level, GOD will deploy autonomous agents to hunt the decker down; if they are unsuccessful, a GOD spider will reinforce them. A skilled decker relies on speed and stealth to achieve their goals before this happens.

Hosts maintain their own alarm state, separate from the local mesh one as they are outside of GOD's jurisdiction. They react to alarms by deploying ICE and security counter-hackers, as well as alerting security personnel in meatspace that a possible intrusion is underway.