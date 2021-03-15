---
title: Symmetric entropy pools
linkTitle: Entropy pools
type: docs
description: Hack-proof encrypted comms... with a twist
date: 2021-03-15
weight: 1000
---

{{% alert title="Notes" %}}Symmetric entropy pools are intended to be used only as a plot device. No game mechanics are given for them.{{% /alert %}} 

Quantum processors used in cyberdecks for hacking and code-breaking can shred almost any known cryptography, given enough time; but they are not omnipotent. If you really, *really* need a secure communications channel, and are prepared to jump through hoops for it, there is something you can do.

Ancient cryptographers would sometimes use *[one-time pads](https://en.wikipedia.org/wiki/One-time_pad)* to encode messages in a way that was nearly unbreakable. The 207x equivalent is a *symmetric entropy pool*. Two parties share a massive pool of carefully generated, thoroughly randomised data. The pool is used to encrypt all communications between them before they are sent via the public Matrix. The other party uses their matching copy of the pool to decrypt the message again. In theory, this cannot be decrypted by attackers, as it appears to be completely random noise.

Shared entropy pools come with some significant downsides, however:

1. The entropy pool has to be kept absolutely secure and private, so the parties usually have to meet face to face to set the pool up, or the data has to be sent via eg. a trustworthy data courier.
1. Physical access to one copy of a shared entropy pool for a few minutes is enough time to duplicate it. If you possess a copy of someone else's pool, you can undetectably spy on their communications. This makes copies of established pools extremely high-value targets for espionage.  
1. Due to an interaction between the [Roper-Eld quantum computational limit](https://shadowrun.fandom.com/wiki/Echo_Mirage) and the [Shannon-Hartley theorem](https://en.wikipedia.org/wiki/Shannon%E2%80%93Hartley_theorem), the size of the entropy pool required to securely encrypt a channel increases with the *square* of the data being sent along it. This quickly becomes very difficult to manage if the intention is to use it for long-term communications. The pools have to regularly be recreated and re-copied between users.
1. SEPs can be used for realtime audio or (at a push) video, but cannot support the data rates necessary for AR or VR traffic.

## SEP hardware

Most users of entropy pools use specialised hardware to store and work with them. This is a credstick-sized device that plugs into a standard dataport on a commlink or cyberdeck. The commlink sends the encrypted data stream into the device, and decrypted data comes back. The main advantage of this is that when being used normally the entropy pool cannot be hacked even if you hack the commlink, as the commlink cannot read the pool directly.

However, by flicking a recessed switch, the device can be put into setup mode; this is designed to allow pools to be created, synchonised, and copied. Hence, with physical access to any device for a minute or two, an attacker can easily duplicate the pool.


<!--
Software-only pools

Very small entropy pools, suitable for a few dozen short text messages, can be created and managed on commodity hardware, such as that available to the PCs. 
-->