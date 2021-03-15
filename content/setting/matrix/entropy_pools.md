---
title: Symmetric entropy pools
linkTitle: Entropy pools
type: docs
description: Hack-proof encrypted comms... with a twist
date: 2021-03-14
weight: 1000
draft: true
---

{{% alert title="Notes" %}}Symmetric entropy pools are intended to be used only as a plot device. No game mechanics are given for them.{{% /alert %}} 

Quantum processors used in cyberdecks for hacking and code-breaking can shred almost any known cryptography, given enough time; but they are not omnipotent. If you really, *really* need a secure communications channel, and are prepared to pay big nuyen for it, there is something you can do.

Ancient cryptographers would sometimes use *[one-time pads](https://en.wikipedia.org/wiki/One-time_pad)* to encode messages in a way that was nearly unbreakable. The 207x equivalent is a *symmetric entropy pool*. Two parties exchange a massive pool of randomised data. The data is used to encrypt all communications between them before they are sent onto the public Matrix. In theory, this cannot be decrypted by attackers, as it appears to be completely random noise.

Shared entropy pools come with some significant downsides, however:

1. The entropy pool has to be kept absolutely secure and private, so the parties usually have to meet face to face to set the pool up, or the data has to be sent via eg. a trustworthy data courier.
1. Due to an interaction between the [Roper-Eld quantum computational limit](https://shadowrun.fandom.com/wiki/Echo_Mirage) and the [Shannon-Hartley theorem](https://en.wikipedia.org/wiki/Shannon%E2%80%93Hartley_theorem), the size of the entropy pool required to securely encrypt a channel increases with the *square* of the data being sent along it. This quickly becomes very difficult to manage if the intention is to use it for long-term communications.
1. Physical access to one copy of a shared entropy pool for a few minutes is enough time to duplicate it. If you possess a copy of someone else's pool, you can undetectably spy on their communications. This makes copies of established pools extremely high-value targets for espionage.  

Large entropy pools, suitable for encrypting realtime audio or video data, require specialised hardware to create and encode/decode. This hardware is heavily restricted and difficult to acquire. Even then, the volume of data it can encrypt cannot support more than video calls - Matrix traffic, AR or VR, simply cannot be protected. 

Very small entropy pools, suitable for a few dozen short text messages, can be created and managed on commodity hardware, such as that available to the PCs. 
