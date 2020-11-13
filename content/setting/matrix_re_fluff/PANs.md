---
title: Personal Area Networks (PANs)
linkTitle: PANs
type: docs
description: How normal people protect their Matrix stuff
date: 2020-08-23
weight: 500
---

One reason commlinks are quite powerful is to protect you against hacking. They dedicate a fair bit of their time to monitoring threats around you, scanning for incoming attacks, and so on. That’s definitely important! But what about the rest of your stuff? Every other Matrix-linked thing you own, from your toaster to your gun to your smartglasses, is vulnerable too - and they don’t have enough CPU to protect themselves. They can borrow some processing on demand, via fog computing, to put up some (feeble) defence. But that won’t protect you from serious hackers.

What you need is a **personal area network**. A PAN connects and merges all your devices into a private little cloud on the local mesh. Your commlink takes charge, and all traffic to and from the mesh goes through it, instead of directly between the device and the mesh. That means it can watch over all traffic, scanning it for attacks, and intervening to defend your devices. Imagine Matrix traffic as acid rain, your commlink as an umbrella, and your devices sheltering safely beneath it.

PANs can be extended and merged, with the most powerful device becoming the one that protects the whole network. When William Wageslave travels to work, he has a PAN, centered on his commlink, protecting his devices. That provides moderate protection against hackers, but not enough for his corp employers to feel good about. So when he arrives at work, the first thing he does is tell his commlink to join the office’s local host. Once the host verifies his persona through DNI-auth it merges his PAN with the office’s Wide Area Network (WAN) and now all his stuff is even more protected, because all his traffic is going through the company host. At the same time, it grants his persona various permissions to access the company resources William will be using to do his job. These will be revoked automatically when he leaves at the end of the day and disconnects from the WAN.

Note that you can only form PANs or WANs on the local grid. You can’t create a WAN based on a cloud host because the latency is too great.

Megacorps are far too paranoid to allow their employees to connect to their servers full of secrets with an unprotected commlink. It would be much too easy for criminals to hack the commlink and use it to get in. So most wageslaves, when working, have to have their commlink connected to a WAN that simultaneously controls their access to work networks and protects them against hacking. This means "working from home" is not a thing that happens in the Sixth World. The user has to be using a device that is part of the company WAN, and that means they have to be within local mesh range of the company host in their office.

Perhaps the corps could solve this, if they cared to. But they're micromanaging controlling assholes who like being able to watch their wageslaves, so they're not trying very hard. Very important execs might have corporate local hosts installed in their houses so they can work remotely. Everyone else has to suffer a grinding commute and the watchful eye of their bosses.

### Securing your devices outside the local mesh

What about poor William’s car, out in the parking lot? Or his toaster at home? He’s too far away from them to shelter them in his commlink’s PAN. But a passing hacker could really spoil his day by destroying these devices as they sit naked on the Matrix.

To solve this, at home, people typically use **network defenders**[^1]: sort of like cut-down mini-commlinks (or, if you prefer, really really tiny local hosts) whose only job is to maintain a basic protection zone around their stuff. They’re usually a step or two less powerful than a commlink, so they’re far from bulletproof, but they’re better than nothing and will at least keep war-driving script kiddies from destroying your house while you’re at work by reprogramming your soy dispenser to "unending firehose" mode. Hopefully.

[^1]: Per RAW, an unattended device typically rolls either 2 or 4 dice to resist hack attacks, which is almost the same as being entirely unprotected. The world can't function like this, it would be full-on chaos. I've introduced network defenders as a slightly easier option to rewriting the entire Device Ratings table to give undefended devices more defence out of the box, although that is a viable alternative choice.

Vehicles get a special firewall package as part of their GridLink subscription. Whenever the vehicle leaves the user’s PAN, it connects itself to a cloud host that defends it against hack attacks. The effectiveness of this defence varies with the user’s GridLink subscription tier.