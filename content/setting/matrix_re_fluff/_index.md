---
title: "The Matrix re-fluff"
linkTitle: "The Matrix re-fluff"
type: docs
---

## Introduction

The Shadowrun Matrix rules have undergone years of patching and re-patching, more so than any other aspect of the system. There are many decisions that are made for good game mechanic reasons but have inadequate explanations within the in-game universe. This makes them confusing and counter-intuitive, as the mechanics and the narrative don't align.

While the rulebooks do a decent job of defining the pieces of the Matrix they don't go into enough detail about how the pieces fit together inside the game universe. Instead, the books mostly go from piecemeal definitions directly into the rules. Players and GMs are left to infer the workings of the game universe from how the rules function, but this isn't always clear or consistent.

I wanted to have a go at cleaning this up for my own game. This document is the result. It attempts to describe the in-universe view of the Matrix and how it works.

Goals of doc:

* To support the classic cyberpunk tropes, such as criminals slicing through seemingly-overwhelming security by finding and exploiting weak points, and of seemingly-impenetrable megacorps undone by their arrogance and laziness.
* To keep as close as reasonably possible to Shadowrun 5/6e rules-as-written.

Non-goals: 

* To consider rule changes as a consequence of this doc (that can come later, if required.)
* To obey established canon (I will deviate or expand wherever I feel necessary).
* To use real life terminology with complete accuracy (I will use computing terms in order to evoke a high-tech future, but not necessarily in perfect accordance with their real definitions.)
* To adhere to a strictly retro-futurism interpretation of cyberpunk; this document will not be designed to support wired networks and neon wireframe virtual realities.

{{% alert title="Notes" %}}
I will occasionally include commentary on my thinking behind certain things. When I do, it'll be formatted like this.
{{% /alert %}}

NB: Although the below is written predominantly for my own Shadowrun campaign, and mostly uses Shadowrun jargon, I hope it might also be of use for other Cyberpunk RPGs that eschew cassette futurism and instead have wireless networks and augmented reality interfaces.

## Major topics discussed so far

*   Why deckers have to be within hacking range of targets
*   What personas are, and why you can only have one at once
*   Why you can’t steal (most people’s) personas to get all their stuff
*   How shadowrunners and other organised criminals can get by in modern society
*   Why you can’t trivially destroy people’s houses by hacking all their stuff when they’re at work
*   Why cyberware and weapons have wireless connections and hence are hackable

## What the Matrix is

### Nuts and bolts of Matrix infrastructure

The Matrix is so far ahead of our current understanding of computing so as to border on magical. Nevertheless, there are some ways in which it resembles the networks we are familiar with today.

*   **Mesh routing**: the Matrix predominantly uses high-bandwidth, high-frequency wireless signals to carry vast amounts of data around. Unfortunately, these are also very short range and are easily blocked by solid matter. To get around this, the Matrix relies on a peer-to-peer mesh network for the “last mile” of connectivity. Matrix devices connect directly to each other, dynamically cooperating to pass data from one to another until it gets to where it needs to be. 
*   The **global grid** aka **the Backbone**: your connection only uses the local mesh until it can reach an **uplink node** and be routed onto the global grid, sometimes called the "backbone" or the **upper grid** by deckers. Once your traffic is on the backbone, it moves to a vast planet-spanning array of fibre optic cables and satellite links; bandwidth and speed are approximately infinite, and distance is no object. 
*   **Cellular networking**: when the local mesh fails you, uplinks can still fall back to early-20th-century style long-range digital radio signals. The bandwidth is feeble and the latencies  are terrible; it’s only enough for text/voice/video comms, or for letting your car check with the cloud that you’re allowed to drive it. But at least it works almost everywhere. Cellular networking is strictly a fallback. If a device has any sort of connection via the local mesh, it won’t power up its cellular radio. (It’s a battery hog.) 
*   **Fog computing**: most Matrix devices have the ability to borrow computing power from other nearby devices. This is baked into the Matrix’s protocols. It allows devices to be relatively small and power-efficient, but still cope with occasional spikes in demand for computation. Taking smaller devices off the Matrix vastly decreases their computing power, however. 
*   **Wireless power delivery**: the Matrix is capable of trickle charging devices attached to it, via near-ubiquitous power points. Most small electronic gadgets (commlinks, sensors, headphones, cyberware) have effectively infinite battery life as long as they remain connected to the Matrix. Devices usually include only small backup batteries to get them through any power outages. Some illegal devices, designed to run disconnected from the Matrix for prolonged periods in order to hide from detection, feature larger batteries to compensate.

#### The local mesh

This is the part of the Matrix that relies on device-to-device connections and is called the **local mesh** or sometimes the **lower grid.** The extreme density of devices in a 2080 city, combined with the ability to seamlessly pass traffic from device to device, can get your signal where it needs to go.

The local mesh has a strictly limited range: too many hops, too much distance, or too much interference and the signal degrades to become useless. Fortunately, for a legitimate user, their network traffic only needs to reach an **uplink node**, so this is rarely an issue.

Any two or more Matrix devices within range of each other will always form a local mesh, even if they cannot route a signal out to the wider Matrix. They will still be able to communicate within themselves as normal. 


#### Uplink nodes

When you want to communicate with a device that’s outside local mesh range, first you need an **uplink node**. These are scattered around major metropolitan areas, typically serving an area of a square kilometer or so. Your device sends traffic along the local mesh until it reaches the nearest or most convenient uplink node. Uplinks serve as the onramps to the rest of the Matrix; they bridge your traffic over to the backbone.

Uplink nodes are sometimes called **beanstalks** by deckers, because they lead to the clouds.[^1] 

#### The backbone

The **backbone**, or the **upper grid**, is the planet-sized interconnected network of fibre cables, satellites, microwave and visible-laser point-to-point communications, and other bleeding-edge-tech ways of getting 1s and 0s from A to B. Once your traffic is on the backbone, distance is no object and bandwidth is almost infinite. 

Security on uplink nodes is fierce, and traffic on the backbone is routinely subjected to deep inspection by GOD. Only the most legendary of novahot deckers have ever managed to smuggle illegal traffic over the backbone, let alone compromise an uplink node entirely.

{{% alert title="Notes" %}}
NB: This document removes the "Foundation" as the main operating medium of the Matrix entirely. The "backbone", as I'm calling it, is its man-made, understandable-tech replacement.

I'm in favour of technomancers; I think the whole concept of "magic"-powered hackers is quintessentially cyberpunk/urban fantasy. But I can't get past the Foundation being this thing that powers the whole Matrix. It can be mysterious or it can be everyday but it can't be both at once. And the lore is hopelessly knotted: hosts are "grown" from the Foundation, but we can't tell you how, and that makes hosts expensive because it's very dangerous, except every Stuffer Shack has one. I can't find a path through this. 

So I say: get rid of it. Keep the Resonance and Dissonance as mysteries-man-was-not-meant-to-know, like metaplanes and whether or not spirits are summoned or created. But make the core Matrix itself entirely technological.

You can easily keep Foundation hosts, however — restricting them to rare, mysterious, and very powerful hosts only. And they can keep their associated weakness to Foundation dives and the plot possibilities they contain.
{{% /alert %}}

#### Dark fibre

The backbone infrastructure is administered and patrolled by GOD, and is theoretically neutral between the megacorps. But the corps didn’t get rich by trusting each other. Where security demands it, it’s not unusual for corporations to run their own private communication lines - eg between a secure, hidden facility and a more public one. This lets the secure facility access the Matrix discreetly without making its location or purpose obvious.

On the local mesh, dark fibre functions like a wormhole. If you can hack the controlling host on one end, you can coerce it to carry your traffic to the other, and suddenly you can "see" a load of devices that could be hundreds of kilometers away. Occasionally, wily shadowrunners use this as part of a smash-and-grab, using a forgotten dark fibre link to hack into a distant host that is too physically well-protected to get near in the physical world.

### Everyday Matrix devices


#### Hosts

Hosts are the servers of the Matrix; they’re the guardians of data, the places you go to get stuff done, and the engines that keep the wheels turning. They come in a few types:


*   **Local hosts** - quite common, these are small, physical servers that are (literally, physically) local to whatever they control. Low to medium rated security systems, building control, stock-keeping, industrial control systems in factories, etc etc. They are only connected to (and can only be reached via) the local mesh, and hence are only usable at relatively short ranges. 

    When viewing the Matrix in VR, local hosts appear down at ground level, at a distinct physical location (unless they are hidden.) Well-funded deckers and other criminals might acquire low-end local hosts for nefarious purposes.
*   **Cloud hosts** - the grown up version of local hosts, used to run services that have to be accessible by people all over the planet. Distributed across lots and lots of physical servers, roughly analogous to a modern day planet-scale website, and directly connected to (and usually only reachable from) the backbone. As such, you can almost always get a good connection to a cloud host, unless your local mesh is being disrupted or you are far from civilisation.
    When viewing the Matrix in VR, cloud hosts float up in the sky.  
    Cloud hosts are enormously expensive to run, both for the hardware required and for the licencing and necessary security to connect to the backbone. 
*   **Offline hosts** - local hosts with no connection to a local mesh. Can be used for cold storage of very valuable files, or wires-only ultramax security systems, or old systems still running in abandoned and forgotten buildings, or things deckers have cobbled together. Typically low rating, as the amount of processing power and hardware becomes very serious for higher ratings; but could in theory be anything. Offline hosts might be connected to online ones via **dark fibre** (see below.)

{{% alert title="Notes" %}}
With the removal of the Foundation as the core technology of the Matrix,. I have also omitted Foundation hosts here, as they are no longer everyday items. You can easily restore them, however — restricting them to rare, mysterious, and very powerful hosts only. And they can keep their associated weakness to Foundation dives and the plot possibilities they contain.
{{% /alert %}}

#### Commlinks

Commlinks are the most visible part of the Matrix - the device most commonly associated with it in people’s minds. They are analogous to modern-day smartphones, and often take the form of a pocket-sized slab covered in a touchscreen (although they can be much smaller if the user forgoes the screen. They can even be wholly implanted, in case you wanted to become an even bigger hacking target than you already are.)

Most people using a commlink do so via a **direct neural interface** and **augmented reality.**


*   DNI gives the user a limited amount of mental control directly over the device, without needing to look at the device or push any buttons. 
    *   DNI is not telepathy. The user can issue simple on/off, less/more, scroll up/down type commands, but not much that is more complicated than that.They can also dictate text, but only at a speed that is a few times faster than talking.
    *   DNI is tiring to use for long periods, as it requires close concentration of a particular kind for the machine to detect the commands. It’s like maintaining a fully spoken inner monologue. Few people can keep that up all day long.
*   Augmented reality means the commlink’s output - mostly visual and audio, some tactile - is projected directly into the user’s consciousness. They see pop-up windows floating in their vision, hear sounds overlaid with the real world, feel the weight and texture of virtual “objects” they touch.
    *   Each distinct element of an augmented reality user interface is called an augmented reality object (ARO), often pronounced “arrow”. AROs can come from your commlink itself, like a messaging window or a control palette. They can be broadcast from nearby devices, like a restaurant displaying a holographic menu outside its door, or a friend showing you a selfie they took. Or they can be sent to you from items you are carrying, such as a smartgun displaying remaining ammunition count in a discreet window in the corner of your eye.
    *   Because pure DNI control requires mental effort, less hardcore users sometimes fall back to either physical controls or (more often) AROs displaying control surfaces. These are less tiring and can be more precise when very delicate control is needed, eg. for piloting a vehicle. User interface AROs accessed via DNI have a tactile component, so the user feels like they are interacting with real physical objects that have weight, texture, and temperature.

Civilians typically get DNI in one of two different ways: either via a datajack, or trodes. Both offer a wireless connection to the commlink, with a wired option as a backup. Trodes are a terrible experience though, with a noticeably poorer AR quality, and a connection that often glitches out unless the user stays quite still (as the trode net can shift around on the head). You can glue it down, but now you have glue in your hair and it’s gonna sting when you take it off. On top of that, they require significantly more concentration to generate DNI signals to interact with the device - they’re just not as sensitive at reading your brainwaves - which gives most people a headache after a few hours. This is why datajacks are heavily preferred and, consequently, extremely common - despite their invasive nature.

(People with more extensive cyberware can get direct neural interfacdes through other options - for example, a rigger’s vehicle control rig includes all the same functionality as a datajack built-in. And some people have commlinks or cyberdecks enitrely implanted, which also give them DNI on demand, without any further hardware.)[^2]

Users who won’t or can’t get DNI can still get a crude form of AR via various pieces of hardware: headphones for audio, plus contacts/glasses/goggles for visual AROs. They can even just about use user interface AROs, although the tactility component is vastly inferior, even if they wear special feedback gloves. It’s a crappy, godawful experience though, and only a Luddite would do this if they had any choice.

Finally, if all else fails, you can always fall back to actually touching the screen on the commlink itself. This still has some usefulness, although in the age of AR it is not most people’s preferred experience. There’s a few reasons people still buy commlinks with screens, though: 

*   People with no form of AR at all can do basic tasks this way - send messages, get directions, order lunch.
*   People might fall back to this at the end of a long day, when they have the stabbing-pain-behind-from-the-eyes feeling from too much DNI. Or their AR interfaces might be glitching out; like all complicated things, they don’t always work like they’re supposed to.
*   If you’re in a heavy spam zone, with swarms of AROs overwhelming your commlink’s filters and filling your vision with distracting or disgusting images, you might have to disable AR entirely until you can get clear (and probably then shop for upgraded spam filtering software.)
*   You also still need the commlink hardware for things like taking pictures or recording video, because even 2080  technology can’t get around the fact you need to point the lens at whatever you want to capture (although high-end commlinks sometimes come with an embedded camera-equipped microdrone that can launch right from the commlink and do that for you...)

Commlinks are the only type of general-purpose computer most people own. With fairly serious onboard compute power, plus the ability to borrow more via fog computing, they can do everything most people need. And through augmented reality, they can expand or contract their interface to fit in the palm of your hand or fill your vision and walls.

#### Tags

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

#### Cyberdecks

Cyberdecks are some of the most complex consumer electronics ever made by mankind. They use dozens of different types of parallel processors, incorporate huge libraries of known vulnerabilities and malware attacks, hundreds of expert systems so advanced as to be bordering on semi-sapient AI, and have nitrogen-cooled quantum computing cores that can break some of the toughest encryption known to metahuman kind in minutes. They have about the same resemblance to commlinks as a variable-geometry VTOL fighter jet does to the Wright Brother’s first plywood-and-canvas airframe.

In other words, they’re kind of a big deal.

## How the Matrix works (for law-abiding wageslaves)

#### Personal area networks (PANs)

One reason commlinks are quite powerful is to protect you against hacking. They dedicate a fair bit of their time to monitoring threats around you, scanning for incoming attacks, and so on. That’s definitely important! But what about the rest of your stuff? Every other Matrix-linked thing you own, from your toaster to your gun to your smartglasses, is vulnerable too - and they don’t have enough CPU to protect themselves. They can borrow some processing on demand, via fog computing, to put up some (feeble) defence. But that won’t protect you from serious hackers.

What you need is a **personal area network**. A PAN connects and merges all your devices into a private little cloud on the local mesh. Your commlink takes charge, and all traffic to and from the mesh goes through it, instead of directly between the device and the mesh. That means it can watch over all traffic, scanning it for attacks, and intervening to defend your devices. Imagine Matrix traffic as acid rain, your commlink as an umbrella, and your devices sheltering safely beneath it.

PANs can be extended and merged, with the most powerful device becoming the one that protects the whole network. When William Wageslave travels to work, he has a PAN, centered on his commlink, protecting his devices. That provides moderate protection against hackers, but not enough for his corp employers to feel good about. So when he arrives at work, the first thing he does is tell his commlink to join the office’s local host. Once the host verifies his persona through a brainwave scan, merges his PAN with the office’s Wide Area Network (WAN), and now all his stuff is even more protected, because all his traffic is going through the company host. At the same time, it grants his persona various permissions to access the company resources William will be using to do his job. These will be revoked automatically when he leaves at the end of the day and disconnects from the WAN.

Note that you can only form PANs or WANs on the local grid. You can’t create a WAN based on a cloud host because the latency is too much.

Megacorps are far too paranoid to anyone to connect to their servers full of secrets with an unprotected commlink. Much too easy for criminals to hack the commlink and use it to get in. So most wageslaves, when working, have to have their commlink connected to a WAN that simultaneously controls their access to work networks and protects them against hacking. This means "working from home" is not a thing that happens in the Sixth World. The user has to be on a device on the company WAN, and that means they have to be within local mesh range of the company host in their office.

Perhaps the corps could solve this, if they care. But they're micromanaging controlling assholes, so they're not trying very hard.

Very important execs might have corporate local hosts installed in their houses so they can work remotely. Everyone else has to suffer a grinding commute and the watchful eye of their bosses.

##### Securing your devices outside the local mesh

What about poor William’s car, out in the parking lot? Or his toaster at home? He’s too far away from them to shelter them in his commlink’s PAN. But a passing hacker could really spoil his day by destroying these devices as they sit naked on the Matrix.

To solve this, at home, people typically use **network defenders**: sort of like cut-down mini-commlinks (or, if you prefer, really really tiny local hosts) whose only job is to maintain a basic protection zone around their stuff. They’re usually a step or two less powerful than a commlink, so they’re far from bulletproof, but they’re better than nothing and will at least keep war-driving script kiddies from destroying your house while you’re at work by reprogramming your soy dispenser to “unending firehose” mode. Hopefully.

{{% alert title="Notes"%}}
Per RAW, an unattended device typically rolls either 2 or 4 dice to resist hack attacks, which is almost the same as being entirely unprotected. The world can't function like this, it would be full-on chaos. I've introduced network defenders as a slightly easier option to rewriting the entire Device Ratings table to give undefended devices more defence out of the box, although that is a viable alternative choice.
{{% /alert %}}

Vehicles get a special firewall package as part of their GridLink subscription. Whenever the vehicle leaves the user’s PAN, it connects itself to a cloud host that defends it against hack attacks. The effectiveness of this defence varies with the user’s GridLink subscription tier.

### Your commlink as the keys to your life

When you boot up your commlink, the first thing you do is sign into it, via some combination of biometrics. This creates your **persona**, your digital mirror-image in the Matrix. The persona runs for as long as your commlink keeps it alive. 

However, like any newborn, your persona comes into the world naked and powerless. So the next thing that happens is your commlink reaches out through the local mesh and up to various cloud hosts that live on the backbone. 

Each of these hosts in turn establishes that the person using your persona matches their fingerprint. For users with direct neural connections, this is carried out as a brainwave challenge/response. The host reaches down through your interface and… pokes… your brain a little, inducing certain patterns. It measures how your brain responds to the poking, and compares it to patterns stored in very secure cloud hosts that were recorded as part of a cryptokey exchange when you created the account. If they match, the host is satisfied you are who you claim to be.

This process is completely safe, or so the corps say. Any resemblance between the transient brainwave states triggered and those recorded in epileptics is purely coincidental.

This process is extremely difficult to fool, particularly for lots of hosts at once; although there are urban legends of particularly wily deckers pulling off successful man-in-the-middle attacks against people using trodes rather than datajacks. 

Unfortunately, users without DNI suffer much lower security. They have to rely on crude biometrics such as fingerprints and retina scans, all of which are much more vulnerable to fakery, even if they use very expensive and high-end scanners.

Once a given host is happy the persona is under your control, it issues your persona with access permissions over whatever it controls. (Deckers call these Access Control Lists, or ACLs - pronounced “ackles”.) One host might belong to Ford, and grant your persona access to drive your Americar. A Horizon host would give you access to your P2.1 social media account. An Ares host, after particularly thorough examination, would enable you to fire your Predator. And so on and so forth - even a low-key user will have hundreds of these permissions.

This all happens in a few seconds.

Personas are ephemeral things. They only last as long as the commlink is running and you are attached to it. (This is particularly irritating for trode users; if the trodes get jostled too much, they can disconnect entirely, and you have to sign in all over again.) Furthermore, to guard against… shenanigans…, the more secure hosts will re-run spot checks of brainwave patterns periodically.

Note also you can never have two personas. The cloud hosts will immediately detect if you attempt to sign in with a second device while the first is still running, and — depending on its paranoia level — either insist one persona is shut down first or completely lock the account down until you contact customer services to get it unlocked.


#### Going off the grid

Only being able to unlock and start your car via a cloud host is fine for a boxed-in ground-down wageslave driving to another 14 hour shift, but it’s not going to work so well for a Knight Errant HTR squad heading into a Barrens deadzone or a long-distance trucking convoy delivering supplies through wildlands. People like these need a fallback for when the signal fails.

Matrix protocols include the ability to offload cryptographic keys directly to your commlink for just such an emergency. For most people, this is nothing but an accident waiting to happen - anyone who hacks their commlink can now steal their stuff with impunity. But if you need to be able to work outside of reliable wireless Matrix access, it’s just what you need. Remember to buy a good commlink and all the security upgrades… and remember to back those keys up to a second device too, just in case. 

Organised criminals like shadowrunners make use of these protocols so they leave less of a datatrail behind them in the Matrix, and so they can still start their cars regardless of which fake SIN they happen to be using right now. Yes, this means a wageslave’s car is a lot harder to steal than a shadowrunner’s, at least based on just the cryptographic security… ain’t irony grand? (Of course, many shadowrunners compensate for this with interesting booby traps, so don’t consider this a declaration of open season on their stuff.)


#### Persona AROs

Most people are broadcasting a few AROs from their commlink at all times. A basic informational ARO contains their SIN and some basic biographic information: their name, gender representation and pronouns, age, and so on. Anything you’d find on a driving licence. Some people might redact all or part of this, for whatever reason; but not broadcasting at least a SIN will attract attention from the authorities in the better parts of town.

Some people also broadcast their persona’s icon at all times, typically scaled to a few inches high and floating over their head or sitting on their shoulder. Customising and sculpting the persona’s icon is a big business, with every kind of lifestyle brand imaginable making virtual accessories for you to play dress-up with on your digital twin, and that’s before you get to the expert artists and modellers who make all sorts of more outre icons than the basic metahuman figures your commlink came with.


### Virtual reality versus augmented reality

Although the Matrix started as a VR-only technology, once ubiquitous AR came along it rapidly fell out of favour. Most people just don’t feel comfortable completely disconnected from their surroundings, particularly if they’re in any sort of public space. Plus, while you can move really fast in VR - with the Matrix flowing as fast as your thoughts - it turns out that’s exhausting if you do it for more than a few hours. VR is now sufficiently uncommon that for most commlinks a SimSense module is an add-on and not a standard feature.

So for most ordinary folk, work time and leisure time that involves computers is mostly done through AR, not VR. They dip into VR now and again -- mostly either for virtual meetings in work with people in different offices or when safe at home -- but that’s all. Extensive time in VR is the domain of serious gamers, the most dedicated sports fans watching live broadcasts, and deckers/spiders/other socially isolated buttonheads.

{{% alert title="Notes"%}}
This is motivated partly by aesthetics - I still want Shadorun to contain offices where people go to work, and I want them to look broadly like you expect offices to. If everyone is in VR all the time, there's no need for huge spaces crammed with tiny desks and beige walls and miserable people. And that aesthetic, to my mind, is an important part of any pan-corporate dystopia. 

I also think it helps make deckers feel distinct from everyday Matrix users. In early SR, VR wasn't ubiquitous (requiring expensive cyberterminals to use), and was mostly only used routinely by hardcore hackers. I want this to still be true.
{{% /alert %}}

### Geography & the grid (VR edition)

Consider the basic, unsculpted Matrix in full VR: how it looks if you disable all visual re-skins normally added by your service provider, your commlink manufacturer, your settings, and so on. Like you’re some sort of 2052-era cave-dwelling metahuman back in the primordial grid. What do you see?

Imagine an infinite plane of black, overlaid with a fine silver grid, stretching to the horizon. This is the **lower grid**. It’s populated with icons for all the devices within local mesh range of your commlink - maybe a few hundred meters, depending on network conditions. Personas are represented by a special icon that is configured according to the user’s wishes. Devices in PANs are hidden, by default, to make the display less cluttered; although you can turn that off if you want to see everything. Devices outside of PANs are represented by icons, typically utilitarian factory-default ones like cartoonishly coloured caricatures of what they are, tiny corporate logos of whoever made it, or eerily photorealistic modelled and rendered versions of whatever the icon represents.

In theory, the lower grid spans the planet - you can zoom your viewpoint up into the “sky” and see a map of the world, with data-sparse areas like the deep sea represented by areas where the silver grid fades out to blank nothingness. But you can’t see icons outside your local mesh, so it’s not that interesting to do so. Most of it would look empty from the perspective of your commlink.

This limited view of the local mesh can be very intense, though, with many hundreds or low thousands of icons - and even more fine filigree lines pulsing between them, representing the data flow from device to device. Even the most hardcore decker can’t do anything with that much information. Normal people run extensive filtering options that remove the clutter and only show the stuff they care about: typically, one icon for each device they are carrying, plus one icon for each PAN they can see.

There may also be local hosts visible in the lower grid. For example, a wageslave arriving at the office would see icons for one or more local hosts associated with the workplace - perhaps the main shared host for files and work, and a few more for security and building control. These are hosts that don’t have a dedicated connection to the backbone and work mostly through the local mesh. They would log on to the shared host at the beginning of their workday, and it wouldn grant them access to the stuff they need to do their job.

Stretching above them is the sky, by default rendered as a very dark blue-grey. Floating within it are icons for all the publicly visible hosts on the Matrix - many hundreds of thousands of them. Again, this is hopelessly cluttered, so people filter their view. You might see the main P2.1 public host, for example, where you can go to read or post social media updates. Your employer’s public host, where you can read PR updates like a good little wageslave. Your commlink fades all the other hosts in the world out, reducing their icons to barely more than a point, and fading all the colour out. The end result is to see perhaps a few dozen icons floating up there, the hosts you care about and use regularly, plus a sprawling constellation of stars representing the rest of the Matrix.

Finally, some cloud hosts like to be associated with particular geographic points. For example, Dante’s Inferno - the famous/infamous Seattle nightspot - has a host that links to the precise location of the club in the real world. Its host icon floats in the sky, as dictated by the rules; it’s a cloud host, not a local host, so it’s in the upper grid. But a thin line of neon pink and blue stretches down from the host to the precise location in the lower grid that corresponds to the club’s address. For hosts like Dante’s Inferno’s one, this is a key part of their branding, and it means when you are close to the club in real life you get a prominent link to the cloud host on the Matrix.

#### Sculpting

Neon-coloured wireframes and faceless chrome figures may have been cool last century, but in 2080, people demand a more _a la mode_ type of chic. Sculpting is the process of making things look different. It’s a combination of artwork, animation, physics modelling; it’s very skilled work; and it’s a lucrative market.

At the big end of the scale, hosts in VR are sculpted to look like… well, anything the owner desires, right down to changing the laws of physics inside the host. Want it to look like infinitely high sky scrapers with the users navigating sections of the host by jumping between them in zero gee? Sure, you can do that. You probably shouldn’t, unless you want to clean a lot of puke off the floors, but you can.

At the small end, people spend _incredible_ amounts of time and nuyen sculpting their persona’s icon. Cosmetic options and add-ons and accessories can be bought from just about any corp on planet Earth, perfect to show your devotion to this or that brand. People often broadcast their persona icon in an ARO, so there’s a lot of pressure to get the look just right.

### How the grid looks in AR

{{% alert title="TODO" color="warning"%}}
stuff
{{% /alert %}}

#### Positioning in AR vs the real world

{{% alert title="TODO" color="warning"%}}
stuff
{{% /alert %}}

### Going offline

https://www.reddit.com/r/Shadowrun/comments/helqt5/matrix_fluff/fvsmhx5/

### Searching the Matrix

There is no Matrix equivalent of Bing or Google Search. Like the political map, the informational one has Balkanised: split up, divided, and almost hopelessly fragmented. To search the Matrix, then, is not to enter some text into a box and get your ranked results in milliseconds. No, it’s a good deal more complicated than that. It often takes between several minutes and double-digit hours. What’s going on during that time?

The Matrix is divided into hosts. In some ways, a host is a little like a modern-day website; you can visit it, and then interact with the content it presents to you. You can go to a screamsheet’s host, for example, and read the current headlines, and search back issues. But unlike a modern-day website, you can’t deep link into a specific file in a host; you can’t build indices that span lots of hosts, and a file on one host can’t directly reference a different file on another host. The divisions between hosts are rigid. Hence: no Google Search.

So the simplest and crudest Matrix search, then, consists of going to a specific, trusted host and searching just that host’s contents using whatever search engine it might present to you. For example, you might go to the public library, and use it to search through reference books. Or to a particular news org’s host and search their historical archives.

Of course, this only gets you one take on the information - and in the Sixth World, most media is dangerously biased. So this isn’t a very good technique. Instead, xxx

The next stage of a Matrix search is sifting the results.  

{{% alert title="TODO" color="warning"%}}
stuff
{{% /alert %}}

## The Matrix and cyberware

### Why cyberware has wireless components

Implanted cyberware always comes with the necessary neural interfaces so the user can make it work without requiring anything else. Nevertheless, legally manufactured cyberware makes heavy use of wireless Matrix networking, for a number of reasons:

*   wireless charging of some components that use too much juice to charge solely via bio-electricity harvested from the host
*   the ability to borrow computing power on demand from nearby devices
*   downloading firmware updates and suchlike
*   broadcasting diagnostics and system status

The most important, however, is for communication between and coordination across different cyberware subsystems. It is quite difficult to run enough cables through squishy flesh to hook up everything to everything else. Plus, different pieces of cyberware from different manufacturers run on a mishmash of semi-incompatible low-level protocols, and that stuff is hard to change when it requires surgery to get at the controls. Instead, commercially available cyberware usually just uses the wireless Matrix as a sort of universal communication bus.

Consider a high-threat response soldier fitted with a smartgun system, cybereyes, and a cyberarm with recoil-compensating gyroscopes. When they fire their weapon, all these systems need to work together in harmony to compute trajectories, display the results of this computation to the user via an ARO, key up the gyros to make just the right motions to counteract the gun’s recoil as they fire, and so on. 

To do all this without the wireless Matrix requires a lot of wires criss-crossing the user’s body plus a coordinating processor to mediate the different protocols used internally on each piece of cyberware. These devices exist - they are called **internal routers** - but they are invasive and expensive and offer limited benefits to legal users. Most people just rely on their devices’ ability to use the standardised protocols of the wireless Matrix to talk to each other.

Besides, the corps like it that way. Most corp security guards are under-trained, under-paid, over-worked, and over-dosed on (at least) stimulants and (quite possibly, at the first sign of trouble) combat drugs. The corps know they can’t be trusted not to wipe each other out in a hail of blue-on-blue gunfire. But proper training costs money, money that goes down the drain when the next shadowrunner team deletes Jimmy; and if there’s one thing the corps hate to do, it’s spend money.

The answer is ubiquitous wireless. Logging of patrol routes so you can be sure they’re not shirking. Inventory tracking of each and every valuable and dangerous item via RFID tags - right down to the bullets in Jimmy’s gun. Remote biometric monitoring, so you know if Jimmy gets jumped, knocked out, or flatlined by intruders. Smartgun fire systems with biometric triggers and linked to friend-or-foe tracking, so the bad guy’s can’t take Jimmy’s gun from him, and so Jimmy can’t get trigger happy and accidentally splatter your star researcher’s expensive brains everywhere.

This isn’t always the case, of course. Elite troopers, from HTR squads on up, are fully trained and perfectly capable of working as a team without the crutch of a wireless network (if they are willing to forgo the benefits of realtime heads-up tactical displays). But Jimmy? Honestly, if you took his wireless away, he’d be a straight-up liability to himself and others. With all this wireless gunk, you barely need the human being to think at all, and that’s the way the corps prefer it. 

### Protecting cyberware against hacking

{{% alert title="TODO" color="warning"%}}
stuff
{{% /alert %}}

## Riggers, drones, PANs, and the Matrix

{{% alert title="TODO" color="warning"%}}
stuff
{{% /alert %}}

### The Rigger Control Console

{{% alert title="TODO" color="warning"%}}
stuff
{{% /alert %}}

### Gridlink

{{% alert title="TODO" color="warning"%}}
stuff
{{% /alert %}}

## Code breakers and thief takers: how the Matrix works for criminals and those who hunt them

“_We must be as stealthy as rats in the wainscoting of their society. It was easier in the old days, of course, and society had more rats when the rules were looser, just as old wooden buildings have more rats than concrete buildings. But there are rats in the building now as well. Now that society is all ferrocrete and stainless steel there are fewer gaps in the joints. It takes a very smart rat indeed to find these openings. Only a stainless steel rat can be at home in this environment..._” — Harry Harrison

All the pervasive Matrix stuff makes the world seem intractable for professional criminals. Surely the second you come out of the Barrens, you’d be revealed six ways to Sunday, right? Fortunately it’s not that bad. Smart bad guys - by which I mean “anyone who’s not a gutter-punk scum” - have some tricks up their sleeves.

### Hiding on the Matrix

Alice is a shadowrunner, walking through a high-end commercial part of town, surrounded by throngs of wageslaves looking to buy lunch or scurrying to meetings. She passes Bob, a Knight Errant beat cop. Alice is up to no good, and therefore carrying a wide range of interesting and potentially illegal items, many of which have Matrix functionality. How does she slip past Bob undetected?

{{% alert title="Notes"%}}
NB: I am removing the Wrapper program, as Shadowrun itself did in 6e. I think it causes an endless hall of mirrors problem, where everyone is constantly running Matrix Perception checks against everything in case it's a Wrapper hiding something dangerous. This slows down play unless you handwave it away, so I'd rather just remove the entire concept instead.
{{% /alert %}}

#### Hiding in plain sight: looking legal

What’s the most fail-safe way to hide? By not having anything to hide in the first place.

If Alice is only lightly armed and has a good fake SIN, she could simply have a legal licence for all her armaments. Her commlink, in addition to her usual SIN and persona icon, will broadcast that she is armed and that she has appropriate licenses. This will probably attract a little attention from Bob; enough to warrant a SIN check, say. But licences to carry firearms are not uncommon so if she’s not doing anything else suspicious and her SIN stands up to scrutiny, Bob will let her pass.

#### Dropouts: going offline 

What constitutes a gun that Bob will ignore and a gun that will attract his attention is very situational, however. Perhaps Alice is carrying more serious firepower than a light pistol: say, a hunting rifle, concealed under a long coat. She might have a licence for it, and it might be perfectly reasonable to be carrying out in the wilds of Snohomish, but that doesn’t mean she can broadcast that she has it now. If he sees that, Bob’s definitely going to know that something is up. Wageslaves don’t take long guns to lunch.

Alice’s next option is to completely disable the wireless features on all the things she wants to hide, while still leaving it enabled on innocuous devices like her commlink (which is still broadcasting her fake SIN, of course.) This means her illegal things can’t be spotted on the Matrix at all. However, it has a few disadvantages:

1. If she needs the gun in a hurry, she may not have time to turn the wireless back on. (For bits of gear, this involves pushing a physical button; for cyberware, giving a mental command. It has to be done one-by-one.) If she gets jumped, she’ll have to do without her smartgun, boosted reflexes, and other toys until she can do that. 
1. If Bob spots the shape of the gun under her coat while she’s not broadcasting an ARO saying she’s armed, he’s going to get really, really interested in Alice. Only criminals would hide that they’re armed. So if you’re going to turn the wireless off on something, you’d better make sure it can’t be spotted.

Obviously, if Alice was trying to sneak into a building in the dead of night, she’d also need to take her commlink offline. It’s pretty hard to sneak into anywhere when you’re broadcasting your Matrix presence to everyone within half a kilometre.

#### Running silent and the art of traffic obfuscation

If she is trying to sneak into somewhere, though, Alice’s third option is to set her entire PAN to run silent. This means all the devices in it minimise their traffic to and from the Matrix, the commlink stops advertising itself as a Matrix node, and she generally disappears from the local grid.

Two downsides here:

1. Walking around downtown, it’s pretty suspicious to not be online. It’d fly in the Barrens, but if Bob notices that Alice doesn’t have any sort of commlink or SIN broadcast, he’s going to assume the worst. (He might not notice, though, as it’s very crowded.) 
1. On the Matrix, spotting a commlink that is running silent is pretty easy for any decker or spider. There’s still some data moving back and forth, and if they know to look for it, they’ll probably find it right away. It gets a lot harder if Alice has a friendly decker who can add Alice’s gear to their PAN and guard her Matrix presence with their cyberdeck, though.

Most of the time, Alice is only going to use running silent if she’s trying to sneak into somewhere. Taking selected devices offline is probably the better option in public spaces.

{{% alert title="Notes"%}}
NB: as in Shadowrun 6e, I am saying that Running Silent is a whole-PAN setting, not a per-device setting. This streamlines decision making and book-keeping.
{{% /alert %}}

#### Having your cake and eating it: internal routers

{{% alert title="TODO" color="warning"%}}
stuff
{{% /alert %}}

### Tag randomisers and scramblers

All those tags in your clothes and equipment, reporting their existence to anyone nearby and their location to servers at all times, would make sneaking around pretty tough. Shadowrunners and other dubious types get around this by scrambling them to destroy their code entirely, or randomising their IDs on a regular basis so no-one can discern any pattern from them.

Normal tags are very easy to mess with and have no countermeasures against this.

{{% alert title="TODO" color="warning"%}}
hardened / stealth tags
{{% /alert %}}

### Local keys

All the clever cloud security stuff described above doesn’t work for squat if you have a low-grade fake SIN or no SIN at all. Fortunately, there’s a fallback mechanism built into the protocols designed to work when the user is off-grid, for example, if there’s another Matrix crash or if you’re way out in the wilds. You can download backup copies of your digital keys and store them on your commlink, then use them to start your car or open your apartment without any hosts  being involved. Bonus: it’s another way of tracking you that no longer works. Only downside is, if your keys get stolen by a script kiddie, so does your stuff - and if your commlink gets trashed, you’d better have backed them up somewhere… Better upgrade from that base model Meta Link, _omae_.

### The difference between legal and illegal cyberdecks

Mass media would like you to believe there’s a world of difference between the tools of the Matrix security specialist and those of the decker. After all, the good guys and the bad guys can’t use the same stuff, right? Otherwise you might question which was which. Well, actually, their ‘decks and their actions are more alike than they are different. Both groups of people need the ability to reach out and hack targets across the local mesh, whether to attack or counter-attack. So both groups need quantum decryption cores to crack encryption and armies of vuln scanners to find exploits on their targets.

What does differ, though, is the degree of monitoring by GOD. Legal cyberdecks are infested at every possible level with stealthmode code and hidden firmware designed to report back to the Grid Overwatch Division at every turn. This code is created by pseudo-AIs, different on each deck manufactured, in an attempt by the corps to stay one step ahead of the streets.

The high price of illegal cyberdecks doesn’t reflect the off-the-shelf hardware so much as the modifications necessary to turn it into a black market cyberdeck. Skilled technicians must labour for many hours to unpick the backdoors and boobytraps built into legal cyberdecks by the manufacturers before they can be used for illicit goals. Processors and memory cores sometimes have to be replaced with custom-manufactured replacements, assembled on nanoforges in anonymous back-alley workshops. An entire cottage industry exists, hidden from view, and the best of their work is always in high demand. 

#### Kitbashed decks

Somewhere in between cyberdecks and commlinks is a broad grey area of kitbashed decks. Usually not much more than a souped-up commlink running some custom software cobbled together by some backroom illicit tech, they are far less capable than even the weakest purpose-built ‘deck. However, they’re also a lot cheaper, and much easier to find on the streets. Many a novahot decker started out with nothing more than a kitbash ‘deck and a datachip full of dreams.

{{% alert title="TODO" color="warning"%}}
These are the dongles in Data Trails / Kill Code that grant commlinks a couple of points in Attack and/or Sleaze. They're of little interest to shadowrunners and are here mainly to explain how low-level criminals can afford any hacking equipment at all, as even the cheapest 'decks are beyond their reach. They can also be used in decker PC's back stories - explaining how they got started without having to afford a full-on deck somehow.
{{% /alert %}}


### How to hack

For legal Matrix users, the local mesh - the wireless peer-to-peer network that gets their data onto the backbone - is just an implementation detail. They rarely even think about it. But for deckers, it’s home.

The corps control and patrol the backbone, and going anywhere near it with an illegal device is begging for trouble. But the local mesh - that’s different. It’s a dizzying mishmash of devices, built up of protocols laid on top of protocols laid on top of protocols, each layer with its own cocktail of security holes. There’s no central control and no central oversight, it’s impossible to secure, and it’s where deckers earn their keep. 


#### Step one: find your target

{{% alert title="TODO" color="warning"%}}
stuff
{{% /alert %}}

#### Step two: reach your target

{{% alert title="TODO" color="warning"%}}
stuff
{{% /alert %}}

#### Step three: hack your target

A decker begins by running routines to poison the local mesh routing protocols. Normally, the grid just passes traffic along to the nearest uplink node. But under the decker’s control, this is corrupted, causing it to pass traffic through the local mesh directly to the target of their hack. Like all local mesh connections, this has a limited range though, so deckers need to be brave enough to get out into the field and within range of the devices they wish to pwn.

{{% alert title="TODO" color="warning"%}}
stuff
{{% /alert %}}

## Appendix: Reddit posts about this document

I’m back with another few excerpts from my Big Ol’ Matrix Re-fluff doc. This time I'm talking about xxx and xxx.

A reminder: my goal here is to re-write the existing fluff to support (my interpretation of) the rules as written. I’m of the opinion that a lot of existing SR material introduces tons of concepts then launches into the rules for how these concepts interact mechanically without first exploring how they interact narratively. So you have to try and reverse-engineer the narrative from the rules, but the rules are complex and sometimes ambiguous, so that’s difficult. I’m trying to bridge over that gap.

Previous posts in this series:

1. [Local mesh & backbone; personas]([https://www.reddit.com/r/Shadowrun/comments/helqt5/matrix_fluff/](https://www.reddit.com/r/Shadowrun/comments/helqt5/matrix_fluff/))
2. [Hosts & commlinks](https://www.reddit.com/r/Shadowrun/comments/hf3dwz/matrix_refluff_hosts_and_commlinks/)


## Appendix: sources of inspiration

I am not the first to attempt something along these lines. Some other sources I have drawn on:

*   [LVN’s The Sane Networked Matrix](https://old.reddit.com/r/Shadowrun/comments/bwwlvb/the_sane_networked_matrix/)
*   [Dethstrobe’s The Matrix](https://docs.google.com/document/d/18__Y0385UauDbH2KPx-YxmDWu96QQV-OU_O1bppsdas/edit#heading=h.thqp862ye4k5)
*   


## Appendix: A typical street scene

Consider a busy street. It’s lunchtime in a commercial district in a decent part of town. The sidewalks are thronged with corp workers looking for lunch, walking past various eateries and cafés. Above them tower offices, scores of stories of chrome and steel. Amongst them pass some less savoury characters: some street rat gangers looking for a score, some shadowrunners up to no good, some Knight Errant beat cops trying to keep the peace. 

What does this scene look like, in augmented reality (AR), for each of the types of people in the scene? What Augmented Reality Objects (AROs) show up, and under what circumstances?


### Civilians 

Let’s start with the corp wageslaves. 

Each of them have a commlink. A bit over half of them have a datajack and are hooked into their ‘link wirelessly; most of the rest are using an image link built into cybereyes, glasses, or contacts. All bar a few of them have an active AR layer. The ones who don’t are usually obvious -- they have to look at the screen of their commlinks to get around, clearly marking them as being too poor to afford even basic amenities. How primitive. 

Each of them has their commlink set to broadcast their System Identification Number (SIN) like all good law-abiding citizens. This takes the form of a small augmented reality object (ARO) that is fixed in position somewhere over their head, moving with them. However, this produces a lot of distracting clutter, so most of the civilians will set their commlinks to filter out these types of objects. They’re there, if they want to look for them: but mostly they’re invisible. 

Similarly, each person is carrying around their personal area network (PAN), consisting of their commlink and all their various items of gear that are slaved behind it (cyberwear, maybe a light pistol, perhaps glasses (or contacts) and earbuds if they don’t have cyberwear, etc etc.) In the Matrix, this appears as an icon for the commlink itself, plus a forest of smaller icons for the devices connected to it. But that’s an awful lot to look at in AR while walking down the street, so most people set their own commlinks to either hide it entirely, or at most show each PAN as a single icon and hide all the connected devices.

The businesses along the street are also broadcasting AROs: menus, flyers, advertising, logos. These vary in size and offensiveness of design. Huge flashing billboards outside a Stuffer Shack proclaim 2-for-1 on Nuke-’Emz Frozen Burritos. Wally and Wendy Wageslave pause to think if they want to partake in them.

Director Dan tuts as he nearly walks into Wally and Wendy. He doesn’t even see the Stuffer Shack promo; although it’s set up to broadcast to everyone, Dan’s high-end commlink treats it as spam and hides it from him. Dan’s eyes are focussed on a discreet, unmarked door up ahead. Unmarked in physical space, anyway. But in AR, Dan can see the logo of the members-only club he’s going to go to for lunch.  This ARO is visible only to a select group of people, identified by their broadcast SIN, and Dan’s on the list.

That’s not the only difference between what Dan sees and what Wally and Wendy see. All up and down the street, advertising AROs are customised to various tracking profiles built from everything they do online and stored against their SIN. When they look at a particular blank piece of wall, Dan sees ads for the newest Ares special edition executive light pistol, with a real mother-of-pearl inlay on the handle. Wally sees a reminder that he won’t want to miss the big Urban Brawl match tonight for his favoured team, the Seattle Screamers. Wendy sees an advert for a new album from Null Shiva, a Doom Arcanometal band she’s been listening to a lot lately. This invasive and systemic tracking is just how the world is run, chummer. Dan’s profiles scream he has money to spend, and the ads adjust accordingly; the stuff is pricier and the ads are classier. Wally and Wendy aren’t so lucky in life, so they see cheaper stuff in garish colours. So it goes.

Overhead, some ARO graffiti (sometimes called “graffitaro” by dorks) lurks; an animation of a swooping dragon in neon colours. It’s being broadcast from a well-hidden data tag stuck behind the facade of the Stuffer Shack. Occasionally, people with cheaper commlinks flinch as the dragon appears to swoop towards them. Those with more expensive commlinks don’t see it, as the ‘link correctly deduces this is graffiti and should not be displayed. The pranking deckers who place these tags are in a constant, unending war with the spam filtering heuristics deployed by commlink manufacturers. 

{{% alert title="TODO" color="warning"%}}
cops, gangers, shadowrunners...
{{% /alert %}}

## Other appendices

Moved to [this doc](https://docs.google.com/document/d/1M8aJSLXBdzviLi_owBaZar1o4-hVrvb8mkQQs2jjqG4) (private.)




[^1]:
     This doesn’t mean I don’t understand the appeal of this. It’s just not what I want in my game, is all.

[^2]:
     credit to u/Finstersang
