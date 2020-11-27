---
title: Making the Matrix
linkTitle: Making the Matrix
type: docs
description: What the Matrix is made of
date: 2020-11-21
weight: 100
---

## The backbone and the local mesh

The third-generation Matrix is a technological marvel, delivering complex AR and VR applications to users wirelessly. But how does it manage such fast connections without requiring the user to physically connect a cable? The answer comes in two parts.

The first part is the *global grid*, also known colloquially as **the backbone**. This is broadly equivalent to what we today call "the cloud"; it's the sum of all the physical infrastructure of fibre trunks, satellite uplinks, and other super-speed connections that connect all the Matrix's hosts together. Within the backbone, speed is functionally infinite, and distance is no issue. But you can only use the backbone if you have a physical, wired connection to it.

Early 21st century cellular wireless standards don't work. The Matrix demands very fast high-frequency ultra-wideband radios, but they are easily blocked by the gleaming steel-and-glass towers of the sprawl. You'd never get a signal. How to square this circle? 

The answer is a *mesh network*. Suppose Alice wants to check the latest updates on her P2.1 social feed. Her commlink sends the request to her neighbour Bob's commlink. From there, it's forwarded to Charlie's commlink. And so it travels, until it reaches an *uplink host* - which has a hardline connection to the backbone. From there, it can whizz off to the right host. The P2.1 host sees the request, and sends the response back down the same link. This all happens in the blink of an eye.

...


But to get traffic from your commlink onto the backbone without a cable, you need the *local mesh*. This is a semi-autonomous mesh network of all nearby devices, co-operating and co-ordinating to route data from device to device until it reaches its destination. This mesh network is crucial, as the connections required for the Matrix need ultra-wideband high frequency radio signals, which only have a range of a few dozen meters. Without the local mesh, you could only get a signal when you were adjacent to an *uplink host*.

Speaking of which: uplink hosts are the third piece of the puzzle; sometimes they are called *beanstalks* (because they lead to the cloud...) Beanstalks are the on-ramps to the global grid; they bridge between the backbone and the local mesh. When you want to check your social media feeds, your connection jumps through the local mesh until it reaches a beanstalk. From there, it moves onto the global grid, and speeds off to whichever host you need to talk to.

## Hosts

Hosts come in a few major types, depending on what kind of connection they have.

The most common type people interact with in their personal lives are *cloud hosts*. These are hosts made up of many physical servers distributed around the planet, all with their own connection to the backbone. They exist everywhere and nowhere at once. Cloud hosts are very powerful and very secure.

However, you can't use cloud hosts for everything. When Wally Wageslave sits working in his office like a good little drone, that office's various systems - heat, light, power, security, Wally's files and emails - are all run by a host located inside the building. These *local hosts* work exclusively on the local mesh, without a backbone connection. Local hosts have one defined place of existence; somewhere, there's some computers in a rack you can point to and say "this is the host for this building." Some of the more prominent and successful hacker groups might run illicit local hosts.

There are other, less common types of host. *Offline hosts* are computers that are totally air-gapped, with no connection to the local mesh or the backbone. The only way to connect to them is directly via a cable. Offline hosts are often used for very important, secret file storage, and are placed in locations that are very physically secure.

## Dark fibre

The backbone infrastructure is administered and patrolled by GOD, and is theoretically neutral between the megacorps. But the corps didn’t get rich by trusting each other. Where security demands it, it’s not unusual for corporations to run their own private communication lines - for example between a secure, hidden facility and a more public one. This lets the secure facility access the Matrix discreetly without making its location or purpose obvious. This is called *dark fibre*.

On the local mesh, dark fibre functions like a wormhole. If you can hack the controlling host on one end, you can coerce it to carry your traffic to the other, and suddenly you can "see" devices that could be hundreds of kilometers away. Occasionally, wily shadowrunners use this as part of a smash-and-grab, using a forgotten dark fibre link to hack into a distant host that is too physically well-protected to get near in the physical world.





