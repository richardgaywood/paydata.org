---
title: "SINs and SINners"
linkTitle: "SINs"
type: docs
description: The ins and outs of proving you are a member of society
date: 2020-08-23
weight: 400
aliases: ["/setting/matrix_re_fluff/SINs"]
categories:
  - archived
---
## What a SIN is

In a society defined by the *haves* and the *have-nots*, the sharpest line between them is the possession of a System Identification Number. A combination of citizenship, a passport, voting rights, and taxation obligations, it guarantees you at least some protection under the law and the chance to work gruelling hundred-hour weeks until you die. What an honour.

SINs are issued by a wide variety of governmental and extra-territorial corporate entities. They can be granted by birth or by a similar process to obtaining citizenship. Sometimes, corps grant them to particularly desirable hires. Often, corps use the threat of revoking someone's SIN to keep their workers in line.

Physically, a SIN is merely a string of alphanumeric characters. The only human-readable part of it is a prefix code indicating the issuing entity - country or corp - who owns and controls the SIN. What counts isn't so much the SIN itself as the data associated with it in various online hosts and datafiles.

SINs have become the *de facto* unique identifier in the Sixth World. They are tracked everywhere, both in person and in the Matrix. Every interaction and transaction you have can be tied to your SIN and tracked in some database - and almost all of them will be. Hence every SIN has, trailing behind it, vast wakes of data, scattered across innumerable databases. 

Those who don't have a SIN - the *SINless* - are condemned to a life of misery. They are locked out of legal employment, of all banking, of reasonable healthcare. They cannot vote and they have no social safety net; even their basic civil rights are reduced almost to nothing. They face a lifetime of grinding for low cash-only wages and paying shady landlords high rent for shitty apartments, and praying that when they get sick there's room at the charity hospital for them. 

This naturally creates a market for fake SINs, anything that might give the hopeless some hope. And, in turn, that creates a market for checking SINs are real.

## Persona SIN broadcasts

The Matrix protocols have baked-in support for all personas to broadcast a SIN in a special sidechannel. This enables pervasive tracking; every interaction you have on the Matrix and in real life can be cross-referenced against your SIN. Everywhere you go, everything you do, there is a data trail left in your wake, extending out behind you. And that trail is scanned and recorded by thousands of corps.

In most parts of the world, SIN broadcasts are not *quite* a legal requirement, but they are certainly strongly enforced. Not broadcasting any SIN in a lower-middle-class-or-better part of town will attract unwelcome attention from the authorities. In high-class areas, you can also expect that SIN to be routinely getting checked for validity against the GSINR (see below). Some public areas will actively alert authorities if you enter without a SIN broadcast, and most legal businesses, from shops to public transport, will refuse to do business with you.

The converse is also true; broadcasting a SIN out in the Barrens can mark you out as a rube and a target.

### SIN-bombing

If the SIN is just a short string, and everyone is broadcasting theirs to the world at all times, why not just take someone else's? Why bother with complicated fake SINs at all?

The first answer is that legal devices can't do this at all. They don't let you set your SIN yourself, nor do they store it anywhere. Instead, when you boot your persona, they query a host belonging to your SIN issuer, which does a [DNI-auth check]({{< relref "personas.md#dni-auth" >}}) of your brainwave patterns before giving your device the SIN it should broadcast. 

Even if you hack your device to broadcast an arbitrary SIN, though, this still doesn't work. The same trackers and profiles that are listening for your SIN will almost immediately notice (a) if two different personas are broadcasting the same SIN at the same time and (b) if a SIN has moved from one persona to another. Either condition will result in them broadcasting an alert that will lock the persona completely out of the Matrix until they reboot their device and sign back in to their account.

This can be used as an attack vector, called "SIN-bombing": deliberately copying someone else's SIN just to get them temporarily booted offline. It's typically little more than a minor inconvenience, though, so of little practical value.

### Why SIN broadcasts are not used for security

If you are a corpsec architect, SIN broadcasts appear to be a very useful tool. It is supremly difficult to spoof or steal either personas or SINs, which means in theory they can provide very strong guarantees that someone trying to get through a security gate is who they say they are. Particularly when the corp in question is also the issuer of the SIN, as is typically the case for its employees, which means they have unfettered access to the SIN biographic and biometric data.

Unfortunately for the corps, it doesn't work that way in practice. Several high-profile data thefts took place in the early 2070s where Shadowrunner teams used a SIN-bombing attack combined with a powerful local jammer to clog up Matrix traffic. The duplicate SIN was noticed and shut down a few seconds later, delayed by the jammers... but during that narrow window, the attackers were able to open doors, shut down security systems, and disable countermeasures. The third or fourth time this happened to any given corp, they quickly switched gears, and pulled SIN scanners out of critical security systems. Today, the state-of-the-art in local security systems consists of biometric scanners coupled with a database of allowed users held locally on a well-secured host.

## Verifying SINs

It is crucial that the *haves* protect their stuff from the *have-nots*. Hence, it is important to be able to verify a given SIN is real and not an imposter. Fortunately for plucky criminals trying to live outside the law, a combination of inter-corp paranoia and mistrust makes checking if a SIN is fake a much more difficult problem than it could be[^dystopia].

[^dystopia]: Shadowrun is a hyper-capitalist corporate dystopia, not a panopticon surveillance dystopia.

There are, broadly, three methods used to verify that someone presenting a SIN is doing so honestly.

### The global SIN registry

The global SIN registry (GSINR) is a fairly simple database of every SIN, world-wide. Each SIN in the database is stored with several additional pieces of data:

1. basic biographical information (eg. name, gender, metahuman race, date of birth)
2. biometrics (eg. retina scan, fingerprints, a DNA profile)
3. special red-flag fields; for example if the SIN was previously discovered to be a fake, if it has a serious criminal record, or if it is currently wanted as part of a criminal investigation (and if so, in which jurisdictions) 

It takes less than a second to look up a given SIN on the registry. The registry is administered by the Corporate Court and access to it is provided fairly cheaply to any interested corp or nation state, although there are additional fees for more detailed information.

For a check against the SIN registry, the querier provides a SIN and, optionally, some biometric data eg. a fingerprint. There are several possible outcomes of a check against the GSINR:

1. the provided SIN does not exist.
2. the provided SIN exists, and here are the values of its red-flag fields.
3. the provided SIN exists, here are its red-flag fields, and here is the associated biographic data (name, date of birth, etc).
4. the provided SIN exists, here are its red-flag fields and biographic data, and it does / does not match the biometric sample provided.

Returning the biographic data or confirming the biometric data (ie (3) and (4) above) incur extra fees for the querier, which quickly add up if scanning SINs routinely, so they tend to be reserved for more detailed checks.

The global registry does not permit "reverse searching" ie. you cannot take a fingerprint and ask the database what the corresponding SIN is, nor can you simply download all the biometric data and scan it yourself. The only type of query is "here is a SIN and some biometrics" with the response of "this does / does not match." Every few years some do-gooder tries to get this changed on the grounds it would help fight crime; the megas that control the Corporate Court always shoot it down. They know that it would make their own staff too easily identified by and spied upon by their competitors.

Unfortunately, the global SIN registry is only as trustworthy as the least secure entity that can access it [^1], and (by definition) data can be added to it by every entity that can issue SINs. It's a relatively trivial process for the purveyors of fake identities to get enough of a hack against some smaller nation-state to insert fake SINs into the global registry. With a bit more effort, they can even get the biometrics to match whoever the user of the fake SIN will be. So, searches against the global SIN registry are a pretty low-grade check, and easy to fool. Still, it provides enough of a verification to keep out the real low-lifes, and is quick and cheap.

In game terms, a check against the global SIN registry is a rating 1-2 check. All purchased fake SINs have at least an entry on the global registry, and all except the very worst of them also have correct biometrics.

[^1]: This is a change from RAW, where the global SIN registry is very secure.

### Be the SIN issuer

If you are the entity that issued the SIN, you have a lot more information about it at your fingertips to perform verifications with. And you can work in the knowledge that your SIN database is held much more securely than the global registry, and so much less likely to be polluted with fakes planted by hackers.

For a start, if a given SIN that claims you issued it is in the global registry but not in your own databases (quite common for low-grade fake SINs), then you've definitely caught a faker. You can flag the fake to the registry and deal with whoever is using it as you wish. Probably painfully.

Fortunately for the kinds of high-end criminals who rely on fake SINs to move through society, if you *aren't* the SIN issuer of a SIN you want to check, you simply can't do any of this. The SIN issuers are either secretive megacorps who compete with each other, or paranoid nation-states that are barely on speaking terms. They don't share their SIN details except under the most exceptional circumstances. So criminals only face these kinds of near-impossible-to-fool checks if they're foolish enough to roll up on (say) an Ares facility toting false Ares SINs. [^2]

[^2]: I don't intend to track/enforce this in practice, unless I want to build a specific plot point around it. I will assume all my PCs' false SINs come from smaller/obscure corps or nation-states.

Note that SIN issuers can also "reverse search" their own databases, ie take a DNA sample or fingerprint and scan for SINs that match it. The capability to do so is carefully controlled, however, and only accessible to people in positions of authority. 

In game terms, a check against the issuer's SIN registry is a rating 6+ check. These checks can take time, particularly if the biometric data being checked requires elaborate procedures (eg. DNA samples.) They might also incur a cost, depending on how byzantine the corp is organised. It is not uncommon for BigCorp Identity Services to only make the SIN database available to BigCorp R&D Subsidiary on a for-profit basis. [^3]

[^3]: If you think this sounds unlikely, I have alarming stories about real-world corporations to tell you.

### Online profiling

If you want more security than a global registry check but you need to check SINs you don't own, then your only option is a verification check with a data profile broker.

Data profiling exists in the Sixth World as it does today. Companies that resemble a high speed collision between Experian and Facebook ingest the data trails people leave behind them - all conveniently tagged and cross-referenced with their SINs - and use pseudo-AIs to build predictive models of each person's interests, desires, and behaviour.

These profilers' primary market is advertising, but they long ago realised that a side effect of their work is spotting fake SINs. Their data analysis is so thorough that any inconsistencies in the data trail attached to a fake SIN stand out like a glowing beacon. A complex marketplace of realtime SIN checks quickly emerged.

Someone wishing to verify a SIN is real can send it to one or more of these brokers. They will look at the data trail associated with the SIN and scan it for gaps and conflicts. If they find any red flags, they will report back to the querier that the SIN looks suspicious, and they can take whatever further actions are appropriate.

In game terms, a check against profile brokers is a rating 3-6 check, depending on the number and quality of brokers involved. These checks become quite expensive to carry out for the querier, particularly at the higher end, so they are not done routinely. These types of test also have a false positive rate; they sometimes flag real SINs as fake, which can irritate VIPs being inconvenienced and get lowly security guards fired.

## Fake SINs

Fake SINs consist of several parts, of escalating levels of quality:

1. A listing on the Global SIN Registry (GSINR), plus plausible biographic information and biometrics. On the crudest fakes, the biographic information might not match the user of the fake SIN at all; these are often recycled SINs for deceased users that were prevented from being marked as inactive. At the higher levels, the fakes will have biometrics that match the bearer of the SIN.
2. As above, plus a realistic "legend", meaning a faked life logged onto tracking services. This is where the SIN creator's skills as a forger are really tested, crafting a historical data trail for the SIN that will fool trackers and profilers. This is where the SIN fakers earn their nuyen.
3. As above, plus entry of the fake SIN into the issuing entity's master SIN database, with matching biometrics. This level of compromise over the SIN registries - whether via bribery or security breach - is extremely difficult (and hence expensive) to pull off.

Lower rating fake SINs are created through a combination of outright hacks against smaller corps or nation-states that have access to the GSINR, coupled with bribery of corrupt insiders, but have no matching entries in the issuing entity's private SIN database. 


## Appendix: references

This section was written based on, in part, the discussion in [this thread](https://forums.shadowruntabletop.com/index.php?topic=31747.0).

<!--
## Appendix: Design notes

This is a tricky one. Per RAW, it seems all of the following are true about SINs:

1. A SIN is a short string of letters and numbers. It contains, encoded within it, your name, date of birth, place of birth, and the nation/corp that issued the SIN. This information can only be decoded by some people. It is typically issued at birth and is immutable. 
2. SINs are associated with stored biometrics - DNA, retinal scan, fingerprints. 
3. SINs and biometrics are stored together in two databases: one run by the entity issuing the SIN and the Global SIN Registry. These are "among the most secure on the planet."
4. SIN broadcasting is close to ubiquitous, especially in civilised parts of town. The SINless are not welcome. A SIN is required to do almost anything - get healthcare, ride public transit, shop.
5. A SIN cannot be spoofed, duplicated, or stolen. There are no rules for this. 
6. Instead, criminals use fake SINs, which are created by hacking the SIN databases to insert new data. These fake SINs might have biometrics data in the database that do not match reality.
7. No employer uses SINs as any sort of identity auth; instead we have numerous rules for keypads, passkeys, swipe badges, etc etc.
8. SINs can be validated but this validation is usually pretty limited (it only says it is/isn't true). You have to get a long way up before SIN verification involves checking for matching biometrics ie that the DNA/fingerprints/etc on file match the subject.
9. SINs cannot be reverse searched for biometrics ie. you can't take someone's fingerprints or blood from a crime scene and link it to a SIN.

Notes:

* (1) and (6) are slightly in conflict. It's secure, but people routinely hack it?  
* (9) makes little sense, why wouldn't it be searchable?
* (5) and (7) are in conflict. If SINs are very secure, why not use them as the basis for security checkpoints?
* Unclear how changes of name are handled (re: (1))
* Unclear how (4) and (5) go together - why can't you just pick up someone else's SIN?
* How does the encoding in (1) work in such a way that the KE beat cop can decode it but your team's decker can't?
-->