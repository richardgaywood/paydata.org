---
title: "How the Matrix works (for law-abiding wageslaves)"
linkTitle: "The legal Matrix"
type: docs
description: How normal people use the Matrix
date: 2020-07-05
weight: 20
---
In the previous sections, I've discussed hosts, commlinks, personas, VR, AR: all the pieces that make up the Matrix. But how do they come together? How do users - normal civilians, now, not criminals - use these pieces to live their lives? 

## Personal area networks (PANs)

One reason commlinks are quite powerful is to protect you against hacking. They dedicate a fair bit of their time to monitoring threats around you, scanning for incoming attacks, and so on. That’s definitely important! But what about the rest of your stuff? Every other Matrix-linked thing you own, from your toaster to your gun to your smartglasses, is vulnerable too - and they don’t have enough CPU to protect themselves. They can borrow some processing on demand, via fog computing, to put up some (feeble) defence. But that won’t protect you from serious hackers.

What you need is a **personal area network**. A PAN connects and merges all your devices into a private little cloud on the local mesh. Your commlink takes charge, and all traffic to and from the mesh goes through it, instead of directly between the device and the mesh. That means it can watch over all traffic, scanning it for attacks, and intervening to defend your devices. Imagine Matrix traffic as acid rain, your commlink as an umbrella, and your devices sheltering safely beneath it.

PANs can be extended and merged, with the most powerful device becoming the one that protects the whole network. When William Wageslave travels to work, he has a PAN, centered on his commlink, protecting his devices. That provides moderate protection against hackers, but not enough for his corp employers to feel good about. So when he arrives at work, the first thing he does is tell his commlink to join the office’s local host. Once the host verifies his persona through a brainwave scan, merges his PAN with the office’s Wide Area Network (WAN), and now all his stuff is even more protected, because all his traffic is going through the company host. At the same time, it grants his persona various permissions to access the company resources William will be using to do his job. These will be revoked automatically when he leaves at the end of the day and disconnects from the WAN.

Note that you can only form PANs or WANs on the local grid. You can’t create a WAN based on a cloud host because the latency is too much.

Megacorps are far too paranoid to anyone to connect to their servers full of secrets with an unprotected commlink. Much too easy for criminals to hack the commlink and use it to get in. So most wageslaves, when working, have to have their commlink connected to a WAN that simultaneously controls their access to work networks and protects them against hacking. This means "working from home" is not a thing that happens in the Sixth World. The user has to be on a device on the company WAN, and that means they have to be within local mesh range of the company host in their office.

Perhaps the corps could solve this, if they care. But they're micromanaging controlling assholes, so they're not trying very hard.

Very important execs might have corporate local hosts installed in their houses so they can work remotely. Everyone else has to suffer a grinding commute and the watchful eye of their bosses.

### Securing your devices outside the local mesh

What about poor William’s car, out in the parking lot? Or his toaster at home? He’s too far away from them to shelter them in his commlink’s PAN. But a passing hacker could really spoil his day by destroying these devices as they sit naked on the Matrix.

To solve this, at home, people typically use **network defenders**: sort of like cut-down mini-commlinks (or, if you prefer, really really tiny local hosts) whose only job is to maintain a basic protection zone around their stuff. They’re usually a step or two less powerful than a commlink, so they’re far from bulletproof, but they’re better than nothing and will at least keep war-driving script kiddies from destroying your house while you’re at work by reprogramming your soy dispenser to “unending firehose” mode. Hopefully.

{{% alert title="Notes"%}}
Per RAW, an unattended device typically rolls either 2 or 4 dice to resist hack attacks, which is almost the same as being entirely unprotected. The world can't function like this, it would be full-on chaos. I've introduced network defenders as a slightly easier option to rewriting the entire Device Ratings table to give undefended devices more defence out of the box, although that is a viable alternative choice.
{{% /alert %}}

Vehicles get a special firewall package as part of their GridLink subscription. Whenever the vehicle leaves the user’s PAN, it connects itself to a cloud host that defends it against hack attacks. The effectiveness of this defence varies with the user’s GridLink subscription tier.

## Personas: your commlink as the keys to your life

When you boot up your commlink, the first thing you do is sign into it, via some combination of biometrics. This creates your **persona**, your digital mirror-image in the Matrix. The persona runs for as long as your commlink keeps it alive. 

However, like any newborn, your persona comes into the world naked and powerless. So the next thing that happens is your commlink reaches out through the local mesh and up to various cloud hosts that live on the backbone. 

Each of these hosts in turn establishes that the person using your persona matches their fingerprint. For users with direct neural connections, this is carried out as a brainwave challenge/response in a process called **DNI-auth**. The host reaches down through your interface and… pokes… your brain a little, inducing certain patterns. It measures how your brain responds to the poking, and compares it to patterns stored in very secure cloud hosts that were recorded as part of a cryptokey exchange when you created the account. If they match, the host is satisfied you are who you claim to be.

Think of it as being like tossing a rock into a lake, and carefully examining the patterns in the ripples.

The corps are very insistent that this process is completely safe. Any resemblance between the transient brainwave states triggered and those recorded in epileptics is purely coincidental. Apparently.

This process is extremely difficult to fool, particularly for lots of hosts at once; although there are urban legends of particularly wily deckers pulling off successful man-in-the-middle attacks against people using trodes rather than datajacks. 

Unfortunately, users without DNI-auth suffer much lower security. They have to rely on crude biometrics such as fingerprints and retina scans, all of which are much more vulnerable to fakery, even if they use very expensive and high-end scanners.

Once a given host is happy the persona is under your control, it issues your persona with access permissions over whatever it controls. (Deckers call these Access Control Lists, or ACLs - pronounced “ackles”.) One host might belong to Ford, and grant your persona access to drive your Americar. A Horizon host would give you access to your P2.1 social media account. An Ares host, after particularly thorough examination, would enable you to fire your Predator. And so on and so forth - even a low-key user will have hundreds of these permissions.

This all happens in a few seconds.

Personas are ephemeral things. They only last as long as the commlink is running and you are attached to it. (This is particularly irritating for trode users; if the trodes get jostled too much, they can disconnect entirely, and you have to sign in all over again.) Furthermore, to guard against… shenanigans…, the more secure hosts will re-run DNI-auth spot checks periodically.

Note also you can never have two personas. The cloud hosts will immediately detect if you attempt to sign in with a second device while the first is still running, and — depending on its paranoia level — either insist one persona is shut down first or completely lock the account down until you contact customer services to get it unlocked. This also works to prevent anyone stealing your persona.

### Going off the grid

Only being able to unlock and start your car via a cloud host is fine for a boxed-in ground-down wageslave driving to another 14 hour shift, but it’s not going to work so well for a Knight Errant HTR squad heading into a Barrens deadzone or a long-distance trucking convoy delivering supplies through wildlands. People like these need a fallback for when the signal fails.

Matrix protocols include the ability to offload cryptographic keys directly to your commlink for just such an emergency. For most people, this is nothing but an accident waiting to happen - anyone who hacks their commlink can now steal their stuff with impunity. But if you need to be able to work outside of reliable wireless Matrix access, it’s just what you need. Remember to buy a good commlink and all the security upgrades… and remember to back those keys up to a second device too, just in case. 

Organised criminals like shadowrunners make use of these protocols so they leave less of a datatrail behind them in the Matrix, and so they can still start their cars regardless of which fake SIN they happen to be using right now. Yes, this means a wageslave’s car is a lot harder to steal than a shadowrunner’s, at least based on just the cryptographic security… ain’t irony grand? (Of course, many shadowrunners compensate for this with interesting booby traps, so don’t consider this a declaration of open season on their stuff.)


### Persona AROs

{{% alert title="TODO" color="warning" %}}
change the below for consistency with the spotting section
{{% /alert %}} 

Most people are broadcasting a few AROs from their commlink at all times. A basic informational ARO contains their SIN and some basic biographic information: their name, gender representation and pronouns, age, and so on. Anything you’d find on a driving licence. Some people might redact all or part of this, for whatever reason; but not broadcasting at least a SIN will attract attention from the authorities in the better parts of town.

Some people also broadcast their persona’s icon at all times, typically scaled to a few inches high and floating over their head or sitting on their shoulder. Customising and sculpting the persona’s icon is a big business, with every kind of lifestyle brand imaginable making virtual accessories for you to play dress-up with on your digital twin, and that’s before you get to the expert artists and modellers who make all sorts of more outre icons than the basic metahuman figures your commlink came with.


## Virtual reality versus augmented reality

Although the Matrix started as a VR-only technology, once ubiquitous AR came along it rapidly fell out of favour. Most people just don’t feel comfortable completely disconnected from their surroundings, particularly if they’re in any sort of public space. Plus, while you can move really fast in VR - with the Matrix flowing as fast as your thoughts - it turns out that’s exhausting if you do it for more than a few hours. VR is now sufficiently uncommon that for most commlinks a SimSense module is an add-on and not a standard feature.

So for most ordinary folk, work time and leisure time that involves computers is mostly done through AR, not VR. They dip into VR now and again -- mostly either for virtual meetings in work with people in different offices or when safe at home -- but that’s all. Extensive time in VR is the domain of serious gamers, the most dedicated sports fans watching live broadcasts, and deckers/spiders/other socially isolated buttonheads.

{{% alert title="Notes"%}}
This is motivated partly by aesthetics - I still want Shadorun to contain offices where people go to work, and I want them to look broadly like you expect offices to. If everyone is in VR all the time, there's no need for huge spaces crammed with tiny desks and beige walls and miserable people. And that aesthetic, to my mind, is an important part of any pan-corporate dystopia. 

I also think it helps make deckers feel distinct from everyday Matrix users. In early SR, VR wasn't ubiquitous (requiring expensive cyberterminals to use), and was mostly only used routinely by hardcore hackers. I want this to still be true.
{{% /alert %}}

## Going offline

https://www.reddit.com/r/Shadowrun/comments/helqt5/matrix\_fluff/fvsmhx5/

## Searching the Matrix

There is no Matrix equivalent of Bing or Google Search. Like the political map, the informational one has Balkanised: split up, divided, and almost hopelessly fragmented. To search the Matrix, then, is not to enter some text into a box and get your ranked results in milliseconds. No, it’s a good deal more complicated than that. It often takes between several minutes and double-digit hours. What’s going on during that time?

The Matrix is divided into hosts. In some ways, a host is a little like a modern-day website; you can visit it, and then interact with the content it presents to you. You can go to a screamsheet’s host, for example, and read the current headlines, and search back issues. But unlike a modern-day website, you can’t deep link into a specific file in a host; you can’t build indices that span lots of hosts, and a file on one host can’t directly reference a different file on another host. The divisions between hosts are rigid. Hence: no Google Search.

So the simplest and crudest Matrix search, then, consists of going to a specific, trusted host and searching just that host’s contents using whatever search engine it might present to you. For example, you might go to the public library, and use it to search through reference books. Or to a particular news org’s host and search their historical archives.

Of course, this only gets you one take on the information - and in the Sixth World, most media is dangerously biased. So this isn’t a very good technique. Instead, xxx

The next stage of a Matrix search is sifting the results.  

{{% alert title="TODO" color="warning"%}}
stuff
{{% /alert %}}