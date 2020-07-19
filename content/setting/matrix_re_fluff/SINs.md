---
title: "SINs and SINners"
linkTitle: "SINs"
type: docs
description: The ins and outs of proving you are a member of society
date: 2020-07-09
weight: 19
---

## What a SIN is

In a society defined by the haves and the have-nots, the sharpest line between them is the possession of a System Identification Number. A combination of citizenship, a passport, voting rights, and taxation obligations, it guarantees you at least some protection under the law and the chance to work gruelling 100 hours weeks until you die. What an honour.

SINs are issued by a wide variety of governmental and extra-territorial corporate entities. They can be granted by birth or by a similar process to obtaining citizenship. Sometimes, corps grant them to particularly desirable hires. Often, corps use the threat of revoking someone's SIN to keep their workers in line.

Physically, a SIN is string of alphanumeric characters. Part of this contains the issuing entity - country or corp - who ultimately controls the SIN. What counts is the data associated with those numbers in various online hosts and datafiles.

SINs have become the *de facto* unique identifier in the Sixth World. They are tracked everywhere, both in person and in the Matrix. Every interaction and transaction you have can be tied to your SIN and tracked in some database - and almost all of them will be. Hence every SIN has, trailing behind it, wakes of data, scattered across thousands of databases. 

The SINless are condemned to a life of misery. They are locked out of legal employment, of reasonable healthcare, even their basic civil rights are reduced. They face a lifetime of grinding for low cash-only wages and paying shady landlords high rent for shitty apartments, and preying that when they get sick there's room at the charity hospital for them. 

This naturally creates a market for fake SINs, anything that might give the hopeless some hope. And, in turn, that creates a market for checking SINs are real.

## Legal SIN verification

It is crucial that the haves protect their stuff from the have-nots. Hence, it is important to be able to verify a given SIN is real and not an imposter. Fortunately for plucky criminals trying to live outside the law, a combination of inter-corp paranoia and mistrust makes checking if a SIN is fake a much more difficult problem than it could be.

There are three broad methods used to verify SINs.

### The global SIN registry

The global SIN registry is a fairly simple database of every SIN, world-wide, attached to some basic biographical information: name, gender, metahuman race, date of birth, and the issuing authority to which the SIN is attached. It takes a few seconds to look up a given SIN on the registry.

The outcome of a check against the SIN registry is either:

1. the provided SIN does not exist or
2. the provided SIN exists or
3. the provided SIN exists, and here is the associated biographic data. There is a small fee charged for this service, which means it is not done as often as the simple "does/does not exist" check.

Unfortunately, the global SIN registry is only as trustworthy as the least secure entity that can access it, and (by definition) it has to be writable by every entity that can issue SINs. It's a relatively trivial process for the purveyors of fake identities to get enough of a hack against some smaller nation-state to insert fake SINs into the global registry. So, this is a pretty low-grade check, and easy to fool. Still, it provides enough of a verification to keep out the real low-lifes.

{{% alert title="Notes"%}}
*This is a change from RAW, where the global SIN registry is very secure and has stored biometric data against each SIN. In game terms, a check against the global SIN registry is a rating 1-2 check.* 
{{% /alert %}}

### Be the SIN issuer

If you are the entity that issued the SIN, you have a lot more information about it at your fingertips to perform verifications with.

For a start, if a given SIN that claims you issued it is in the global registry but not in your own databases (quite common for low-grade fake SINs), then you've caught a faker.

Creating a fake SIN that can fool this kind of check is a deep hack against much more secure systems than the global SIN registry, and even then, it won't be permanent. Sooner or later, system integrity checks will find the fake and delete it.

Of course, if you aren't the SIN issuer of a SIN you want to check, you can't do this. The SIN issuers are often secretive megacorps who compete with each other, or paranoid nation-states that are barely on speaking terms with each other. They don't share their SIN details except under exceptional circumstances.

The SIN issuer databases also contain biometric data for each SIN - retina scans, fingerprints, DNA samples. As such, if they are willing to take the time to gather that information from an individual, they can apply a very high standard of verification. This typically takes at least several minutes, however, so can be impractical in many circumstances.

SIN issuers can also "reverse search" their own databases, ie take a DNA sample or fingerprint and scan for SINs that match it.

### Online profiling

This is the middle ground.



## Persona SIN broadcasts



## Fake SINs

**legend**





{{% alert title="Design notes" %}}

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

{{% /alert %}}
