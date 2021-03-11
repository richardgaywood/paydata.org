---
title: "Matrix fundamentals"
linkTitle: "What the Matrix is"
type: docs
description: The devices that make up the Matrix's infrastructure
date: 2020-07-05
weight: 100
aliases: ["/setting/matrix_re_fluff/fundamentals"]
---

## Matrix infrastructure

The Matrix is so far ahead of our current understanding of computing as to border on magical. Nevertheless, there are some ways in which it resembles the networks we are familiar with today.

*   **Mesh routing**: the Matrix predominantly uses high-bandwidth, high-frequency wireless signals to carry vast amounts of data around. Unfortunately, these are also very short range and are easily blocked by solid matter. To get around this, the Matrix relies on a peer-to-peer mesh network for the "last mile" of connectivity. Matrix devices connect directly to each other, dynamically cooperating to pass data from one to another until it gets to where it needs to be. 
*   The **global grid** aka **the Backbone**: your connection only uses the local mesh until it can reach an **uplink node** and be routed onto the global grid, sometimes called the "backbone" or the **upper grid** by deckers. Once your traffic is on the backbone, it moves to a vast planet-spanning array of fibre optic cables and satellite links; bandwidth and speed are approximately infinite, and distance is no object. 
*   **Cellular networking**: when the local mesh fails you, uplinks can still fall back to early-21st-century style long-range digital radio signals. The bandwidth is feeble and the latencies are terrible; it’s only enough for text/voice/video comms, or for letting your car check with the cloud that you’re allowed to drive it. But at least it works almost everywhere. Cellular networking is strictly a fallback. If a device has any sort of connection via the local mesh, it won’t power up its cellular radio. (It’s a battery hog.) 
*   **Fog computing**: most Matrix devices have the ability to borrow computing power from other nearby devices. This is baked into the Matrix’s protocols. It allows devices to be relatively small and power-efficient, but still cope with occasional spikes in demand for computation. Taking smaller devices off the Matrix vastly decreases their computing power, however. 
*   **Wireless power delivery**: the Matrix is capable of trickle charging devices attached to it, via near-ubiquitous power points. Most small electronic gadgets (commlinks, sensors, headphones, cyberware) have effectively infinite battery life as long as they remain connected to the Matrix. Devices usually include only small backup batteries to get them through any power outages. Some illegal devices, designed to run disconnected from the Matrix for prolonged periods in order to hide from detection, feature larger batteries to compensate.

### The local mesh

This is the part of the Matrix that relies on device-to-device connections and is called the **local mesh** or sometimes the **lower grid**. The extreme density of devices in a 2080 city, combined with the ability to seamlessly pass traffic from device to device, can get your signal where it needs to go.

The local mesh has a strictly limited range: too many hops, too much distance, or too much interference and the signal degrades to become useless. Fortunately, for a legitimate user, their network traffic only needs to reach an **uplink node**, so this is rarely an issue.

Any two or more Matrix devices within range of each other will always form a local mesh, even if they cannot route a signal out to the wider Matrix. They will still be able to communicate within themselves as normal. 

### Uplink nodes

When you want to communicate with a device that’s outside local mesh range, first you need an **uplink node**. These are scattered around major metropolitan areas, typically serving an area of a square kilometer or so. Your device sends traffic along the local mesh until it reaches the nearest or most convenient uplink node. Uplinks serve as the onramps to the rest of the Matrix; they bridge your traffic over to the backbone.

Uplink nodes are sometimes called **beanstalks** by deckers, because they lead to the clouds.[^1] 

### The backbone

The **backbone**, or the **upper grid**, is the planet-sized interconnected network of fibre cables, satellites, microwave and visible-laser point-to-point communications, and other bleeding-edge-tech ways of getting 1s and 0s from A to B. Once your traffic is on the backbone, distance is no object and bandwidth is functionally infinite. 

Security on uplink nodes is fierce, and traffic on the backbone is routinely subjected to deep packet inspection by GOD. Only the most legendary of novahot deckers have ever managed to smuggle illegal traffic over the backbone, let alone compromise an uplink node entirely.

{{% alert title="Notes" %}}
*NB: This document removes the "Foundation" as the main operating medium of the Matrix entirely. The "backbone", as I'm calling it, is its man-made, understandable-tech replacement.*

*I'm in favour of technomancers; I think the whole concept of "magic"-powered hackers is quintessentially cyberpunk/urban fantasy. But I can't get past the Foundation being this thing that powers the whole Matrix. It can be mysterious or it can be everyday but it can't be both at once. And the lore is hopelessly knotted: hosts are "grown" from the Foundation, but we can't tell you how, and that makes hosts expensive because it's very dangerous, except every Stuffer Shack has one. I can't find a path through this.* 

*So I say: get rid of it. Keep the Resonance and Dissonance as mysteries-man-was-not-meant-to-know, like metaplanes and whether or not spirits are summoned or created. But make the core Matrix itself entirely technological.*

*You can easily keep Foundation hosts, however — restricting them to rare, mysterious, and very powerful hosts only. And they can keep their associated weakness to Foundation dives and the plot possibilities they contain.*
{{% /alert %}}

### Dark fibre

The backbone infrastructure is administered and patrolled by GOD, and is theoretically neutral between the megacorps. But the corps didn’t get rich by trusting each other. Where security demands it, it’s not unusual for corporations to run their own private communication lines - for example between a secure, hidden facility and a more public one. This lets the secure facility access the Matrix discreetly without making its location or purpose obvious.

On the local mesh, dark fibre functions like a wormhole. If you can hack the controlling host on one end, you can coerce it to carry your traffic to the other, and suddenly you can "see" devices that could be hundreds of kilometers away. Occasionally, wily shadowrunners use this as part of a smash-and-grab, using a forgotten dark fibre link to hack into a distant host that is too physically well-protected to get near in the physical world.

## Everyday Matrix devices

### Hosts

Hosts are the servers of the Matrix; they’re the guardians of data, the places you go to get stuff done, and the engines that keep the wheels turning. They come in a few types:

*   **Local hosts** - quite common, these are small, physical servers that are (literally, physically) local to whatever they control. Low to medium rated security systems, building control, stock-keeping, industrial control systems in factories, etc etc. They are only connected to (and can only be reached via) the local mesh, and hence are only usable at relatively short ranges. 

	When viewing the Matrix in VR, local hosts appear down at ground level, at a distinct physical location (unless they are hidden.) Well-funded deckers and other criminals might acquire low-end local hosts for nefarious purposes.
*   **Cloud hosts** - the grown up version of local hosts, used to run services that have to be accessible by people all over the planet. Distributed across lots and lots of physical servers, roughly analogous to a modern day planet-scale website, and directly connected to (and usually only reachable from) the backbone. As such, you can almost always get a good connection to a cloud host, unless your local mesh is being disrupted or you are far from civilisation.

	When viewing the Matrix in VR, cloud hosts float up in the sky.  
	Cloud hosts are enormously expensive to run, both for the hardware required and for the licencing and necessary security to connect to the backbone. 
*   **Offline hosts** - local hosts with no connection to a local mesh. Can be used for cold storage of very valuable files, or wires-only ultramax security systems, or old systems still running in abandoned and forgotten buildings, or things deckers have cobbled together. Typically low rating, as the amount of processing power and hardware becomes very serious for higher ratings; but could in theory be anything. Offline hosts might be connected to online ones via **dark fibre** (see below.)

{{% alert title="Notes" %}}
*With the removal of the Foundation as the core technology of the Matrix, I have also omitted Foundation hosts here, as they are no longer everyday items. You can easily restore them, however — restricting them to rare, mysterious, and very powerful hosts only. And they can keep their associated weakness to Foundation dives and the plot possibilities they contain.*
{{% /alert %}}

Not every host advertises its existence. So-called **dark hosts** are ones that are running silent on the Matrix. Local dark hosts can be detected by getting close to them and looking for hidden Matrix icons in the usual way. Cloud dark hosts are trickier, however, and can normally only be visited if you have the secret co-ordinates to find it.

### Commlinks

Commlinks are the most visible part of the Matrix - the device most commonly associated with it in people’s minds. They are analogous to modern-day smartphones, and often take the form of a pocket-sized slab covered in a touchscreen (although they can be much smaller if the user forgoes the screen. They can even be wholly implanted, in case you wanted to become an even bigger hacking target than you already are.)

Most people using a commlink do so via a **direct neural interface** and **augmented reality**.

*   DNI gives the user a limited amount of mental control directly over the device, without needing to look at the device or push any buttons. 
	*   DNI is not telepathy. The user can issue simple on/off, less/more, scroll up/down type commands, but not much that is more complicated than that.They can also dictate text, but only at a speed that is a few times faster than talking.
	*   DNI is tiring to use for long periods, as it requires close concentration of a particular kind for the machine to detect the commands. It’s like maintaining a fully spoken inner monologue. Few people can keep that up all day long.
*   Augmented reality means the commlink’s output - mostly visual and audio, some tactile - is projected directly into the user’s consciousness. They see pop-up windows floating in their vision, hear sounds overlaid with the real world, feel the weight and texture of virtual “objects” they touch.
	*   Each distinct element of an augmented reality user interface is called an augmented reality object (ARO), often pronounced “arrow”. AROs can come from your commlink itself, like a messaging window or a control palette. They can be broadcast from nearby devices, like a restaurant displaying a holographic menu outside its door, or a friend showing you a selfie they took. Or they can be sent to you from items you are carrying, such as a smartgun displaying remaining ammunition count in a discreet window in the corner of your eye.
	*   Because pure DNI control requires mental effort, less hardcore users sometimes fall back to either physical controls or (more often) AROs displaying control surfaces. These are less tiring and can be more precise when very delicate control is needed, eg. for piloting a vehicle. User interface AROs accessed via DNI have a tactile component, so the user feels like they are interacting with real physical objects that have weight, texture, and temperature.

Civilians typically get DNI in one of two different ways: either via a datajack, or trodes. Both offer a wireless connection to the commlink, with a wired option as a backup. Trodes are a terrible experience though, with a noticeably poorer AR quality, and a connection that often glitches out unless the user stays quite still (as the trode net can shift around on the head). You can glue it down, but now you have glue in your hair and it’s gonna sting when you take it off. On top of that, they require significantly more concentration to generate DNI signals to interact with the device - they’re just not as sensitive at reading your brainwaves - which gives most people a headache after a few hours. This is why datajacks are heavily preferred and, consequently, extremely common - despite their invasive nature.

(People with more extensive cyberware can get direct neural interfaces through other options - for example, a rigger’s vehicle control rig cyberware includes all the same functionality as a datajack as part of the package. And some people have commlinks or cyberdecks enitrely implanted, which also give them DNI on demand, without any further hardware.)[^1]

Users who won’t or can’t get DNI can still get a crude form of AR via various pieces of hardware: headphones for audio, plus contacts/glasses/goggles for visual AROs. They can even just about use user interface AROs, although the tactility component is vastly inferior, even if they wear special feedback gloves. It’s a crappy, godawful experience though, and only a Luddite would do this if they had any choice.

Finally, if all else fails, you can always fall back to actually touching the screen on the commlink itself. This still has some usefulness, although in the age of AR it is not most people’s preferred experience. There’s a few reasons people still buy commlinks with screens, though: 

*   People with no form of AR at all can do basic tasks this way - send messages, get directions, order lunch.
*   People might fall back to this at the end of a long day, when they have the stabbing-pain-behind-from-the-eyes feeling from too much DNI. Or their AR interfaces might be glitching out; like all complicated things, they don’t always work like they’re supposed to.
*   If you’re in a heavy spam zone, with swarms of AROs overwhelming your commlink’s filters and filling your vision with distracting or disgusting images, you might have to disable AR entirely until you can get clear (and probably then shop for upgraded spam filtering software.)
*   You also still need the commlink hardware for things like taking pictures or recording video, because even 2080 technology can’t get around the fact you need to point the lens at whatever you want to capture. (Although high-end commlinks sometimes come with an embedded camera-equipped microdrone that can launch right from the commlink and do that for you...)

Commlinks are the only type of general-purpose computer most people own. With fairly serious onboard compute power, plus the ability to borrow more via fog computing, they can do everything most people need. And through augmented reality, they can expand or contract their interface to fit in the palm of your hand or fill your vision and walls.

### Tags

Commlinks may be - for most people - the most visible and obvious type of Matrix device, but tags are by far the most common.

"Tag" is a catch-all term for any small, single-purpose device that connects directly to the Matrix. They are often associated with and attached to a single object in the real world, giving that object a presence on the Matrix and a tiny degree of computing smarts.

The most basic kind of tag is a combination of informational and locational, and these are built into almost all durable consumer goods, from socks to jewelry to coffee mugs. 

*   Tags typically broadcast one or more AROs eg. Domestic appliances can broadcast their instruction manual plus the option to purchase consumables (at a premium price, _omae_.)
*   Owners can use them to find where they are if they ever lose them, via a standard Matrix operation called “trace icon.” (More on this below.) 
*   The object can self-report its instructions in a machine-readable form - for example, you can throw a ball of clothes in the washing machine, the clothes can all broadcast their care instructions to the machine, and the machine can select the best program automatically.
*   When shopping, you can pick up whatever you want and just walk out the store - the tags you are carrying will be recorded and your persona will be billed automatically.

{{% alert title="TODO" color="warning"%}}
secure/robust/stealth tags
{{% /alert %}}

Tags have a dark side: for an unmodified tag, there is no guarantee that the data it is logging is staying private. A law-abiding wageslave is typically being tracked by dozens of tags on their body at all times, all of which are uploading location data and contact tracing data to an endless array of overlapping ad tracking networks. The only kind of privacy they can hope to enjoy is through obscurity; by not being interesting enough to ever be noticed in the sea of data, and by relying on the fact that the data is gathered by competing corps so no-one ever puts the full picture together.

### Cyberdecks

Cyberdecks are some of the most complex consumer electronics ever made by mankind. They use dozens of different types of parallel processors, incorporate huge libraries of known vulnerabilities and malware attacks, hundreds of expert systems so advanced as to be bordering on semi-sapient AI, and have nitrogen-cooled quantum computing cores that can break some of the toughest encryption known to metahuman kind in minutes. They have about the same resemblance to commlinks as a variable-geometry VTOL fighter jet does to the Wright Brother’s first plywood-and-canvas airframe.

In other words, they’re kind of a big deal.

[^1]:	credit to u/Finstersang