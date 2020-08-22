---
title: Icons, spotting, and positioning
linkTitle: Iconography
type: docs
description: How your commlink decides what to show you and where to put it
date: 2020-07-13
weight: 300
---

## Spotting

Everything on the Matrix is represented by an icon. Each device -- your commlink, your car, your toaster - has a corresponding icon, and each icon has a corresponding device. Mostly, these icons are set by the manufacturer and look like the device in question, although the art style can vary from photo-realistic to cartoonish to stylised. People can change them, but generally don't for boring stuff like their toaster. Personas, however, have special icons that the owners can change to look however they want, within some limits. People spend many hours and many nuyen playing virtual dress-up with the personas.

So: suppose Wally Wageslave is using his commlink to view the Matrix. **Spotting** is the process by which his commlink discovers there's an icon to show him. Spotting is tied to the local mesh, the part of the Matrix that runs on device-to-device connections. You can consider spotting range as a sort of short-range horizon, it's the distance around you that you device is actively keeping track of so it can keep your connection going.

Wally's commlink doesn't concern itself too much with devices that aren't really nearby, as it's really only trying to keep its connection alive. By default, the spotting horizon extends to about a hundred metres or so (the exact amount can vary with network conditions.) If he wants - although he probably doesn't - Wally can tell his commlink to look further than that, and show him all the devices it can find at a larger range, up to the limits of the local mesh.

## Invisible icons

There are some circumstances in which Wally might not see an icon for a nearby Matrix device.

1. If the icon is part of a PAN, it won't show up, at least by default. He'll just see the icon of the device running the PAN instead (ie. the owner's persona). This is because the PAN's controlling device is running all the Matrix traffic, so the child devices in the PAN aren't participating in the mesh network, so Wally's commlink isn't interested in them. 
2. Persona icons subsume devices they are controlling. Your commlink doesn't have its own icon distinct from your persona. If a rigger jumps into a drone, the drone's icon is replaced by the rigger's persona.
3. Devices can deliberately hide themselves from the public Matrix, which is commonly called **running silent.** This involves carefully minimising the flow of traffic back and forth and refusing all incoming network requests. Careful analysis can still reveal them though by the footprint of data connections they still have.

## How mesh routing works & what it means

The Matrix, or at least the local grid part of it, is a *decentralised peer-to-peer mesh network*. Previous Matrix crashes have taught the corps the value of robustness and the dangers of single points of failure, so there is no reliance on a controlling host to make the wheels turn. Toss a handful of Matrix 2.0 devices inside a Faraday cage and they'll form a network automatically, without needing anything external to direct them.

Down at the device level, this is quite a complicated process. Each device has to be aware of the position and movements of all the other devices nearby, so it can make smart decisions about where to send its traffic. If Wally wants to send a message to his colleague Wanda, but she's too far away to send it to directly, it doesn't make any sense to send it via a nearby commlink belonging to someone in a car that's about to move out of range. Better to pick a different intermediate that's somewhere inbetween Wally and Wanda and isn't moving.

The mesh network itself resolves this problem without any user intervention. In a fiercely complicated bit of co-ordination, each device uses signal strength measurements and triangulation to estimate the positions of every other device within spotting range. So for every device within spotting range, Wally's commlink has an approximate location - usually plus or minus a few meters, maybe quite a bit more than that if the network is very quiet (not enough devices around to do triangulation) or very noisy (too much to keep track of.)

## Positioning

Devices do not usually broadcast their precise location publicly. Even the most naive Sixth World resident knows it is not a good idea to constantly tell every potential mugger within a few blocks exactly where you are. So the mesh network's approximate position is all Wally's commlink has to go on when trying to line up the icons it sees on the Matrix with the matching devices in the real world.

Positioning is the process by which Wally's commlink decides where to put a device's icon when Wally looks around in AR or VR.

### Icon positioning in VR

In many ways the problem is easier in VR, because the commlink doesn't need to line anything up with the real world. It can place icons for devices in places corresponding to its best guess, and if there's a dense collection of overlapping icons in one place it can artificially spread them out so Wally can see them all individually. After all, if he's in VR, Wally probably isn't overly concerned with exactly where these devices are, he just wants to be able to see them all and interact with them all as easily as possible.

### In AR

In AR, commlinks struggle. By default, they rarely show more than a fraction of nearby device icons anyway, lest they become distracting to the point of uselessness. But if Wally tells it to do so, it'll dutifully have its best guess and place icons around him at some location that might or might not align with reality. This can make some funny things happen, like if Wally is talking to one other person somewhere and that person's icon is shown as being ten metres off to one side.  

This has consequences for, eg., beat cops on patrol. They might pass a crowd of 20 people, where one of the crowd is a SINless criminal scum. But unless they are very sharp-eyed and quick-witted, they are unlikely to notice that the crowd of 20 people only has 19 device icons floating around them. And even if they do, they can't tell who is the odd one out.

## AROs and icons that have positioning information

Public augmented reality displays wouldn't make a lot of sense if different people saw them in different places, so the Matrix protocols also have the ability for any ARO or icon to **anchor** its precise location and orientation. This anchoring be part of the public broadcast -- in which case everyone will see the ARO at the exact same point. Examples include ARO adverts, signage, restaurant menus, art installations, and so forth. Or, it can be private -- Wally can share his commlink's location with his family so they can find him at the mall. Everyone else at the mall can see his commlink icon but not the location information.

## SIN broadcasts & nameplates

Commlink icons have a special sidechannel that usually broadcast the owner's SIN at all times. This isn't quite mandatory, but will certainly prompt investigation from the cops if it's turned off in most parts of town.

**Nameplates** are a sort of beefed-up public version of this. They are an ARO display that people can enable on their commlinks that shows their name, gender pronouns, P2.1 profile link, and other biographic information. People turn these on in situations where they'll be useful, eg when they meeting new people. Some people spend quite a lot of time customising their nameplate AROs to reflect their personalty. These are also the kind of people that will have an obnoxiously over-the-top persona icon.

The etiquette around when it is and isn't polite to show a nameplate is complicated and -- frankly -- still being worked out by society at large. Most people don't walk around in public with one on, although some extroverts might. Most people would turn them on for a business meeting, to facilitate introductions. But turning it on at a private dinner party with people who know you can be considered rude because it implies you think other people there might have forgotten who you are. 
