---
title: Matrix Actions
linkTitle: Actions
type: docs
description: All kinds of things deckers can do
date: 2021-01-16
lastmod: 2021-03-25
weight: 250
aliases: ["sprawlrunners/deckers/matrix_actions.md"]
---

## Offensive & defensive actions

{{% pageinfo %}} 
### Cybercombat Hack
Requires: Fighting utility \
Rolls: Hacking vs target Firewall \
Use on: s-PANs, PANs, standalone devices, ICE

See [Cybercombat]({{< relref "cybercombat.md" >}}).
{{% /pageinfo %}} 

{{% pageinfo %}} 
### Sleaze Hack
Requires: Persuasion utility \
Rolls: Hacking vs target Hardening \
Use on: unattended devices, PANs, hosts, ICE

Gain access to something, hopefully without anyone noticing. See [Hacking]({{< relref "hacking.md" >}}).
{{% /pageinfo %}} 


{{% pageinfo %}} 
### DoS Hack
Requires: Fighting utility \
Rolls: Hacking vs target's Smarts attribute \
Use on: devices

Flood a Matrix target with bad traffic to impede its functionality. See [DoS attacks]({{< relref "combat_decking.md#denial-of-service-attacks" >}}).
{{% /pageinfo %}} 



{{% pageinfo %}} 
### Hide (on local mesh)
Requires: Stealth utility \
Rolls: Hacking, maybe vs Notice \
Use on: your own s-PAN

Can be used on the local mesh to disguise and hide your s-PAN from observers; see [Matrix Stealth]({{< relref "combat_decking.md#matrix-stealth" >}}) for more. If nobody is actively looking, the target number for this test is 4. If you are being actively hunted (eg by a persona running the Notice utility) it is opposed by the hunter's Hacking skill.

Can be used within a host to hide your persona from ICE and security spiders, see "Deceive ICE" on Sprawlrunners pg 39 for more.
{{% /pageinfo %}} 


{{% pageinfo %}} 
### Hide (in host)
Requires: Stealth utility \
Rolls: Hacking, maybe vs Notice \
Use on: your persona

Used within a host to hide your persona from ICE and security spiders, see "Deceive ICE" on Sprawlrunners pg 39 for more.
{{% /pageinfo %}} 



## Configuration commands

{{% pageinfo %}} 
### Improvise utility
Rolls: Hacking

See Sprawlrunners pg 43.
{{% /pageinfo %}} 


{{% pageinfo %}} 
### Change utility loadout

See Sprawlrunners pg 39. Takes a couple of seconds to do outside of combat.
{{% /pageinfo %}} 


{{% pageinfo %}} 
### Jack out

See Sprawlrunners pg 38. Can be a Free action, but then comes with risk of dumpshock.
{{% /pageinfo %}} 


## File and device actions

{{% pageinfo %}} 
### Manipulate files
Rolls: N/A or as required \
Use on: any file(s)

Can be used to copy, edit, erase, or search for files or other data in any kind of store - a host, a node, a commlink, a data chip, etc. Obviously the decker has to have access to the store first, either legitimately or via a hacking action.

The actual file manipulations do not usually require a test. However, if the purpose of the edits requires skill - eg. they are intended to forge credentials, hide suspicious entries in an access log - then a test may be required to see how that goes.

Copying or erasing a very large number of files under time pressure might be a dramatic task.
{{% /pageinfo %}} 



{{% pageinfo %}} 
### Decrypt file
Requires: Decryption utility \
Rolls: Hacking vs file encryption rating die type \
Use on: any encrypted file

Decrypting a number of files under time pressure is usually a dramatic task.
{{% /pageinfo %}} 



{{% pageinfo %}} 
### Manipulate device
Rolls: Hacking or varies, usually vs target's Hardening \
Use on: any device

Can be used to give commands to a device, or manipulate it in other ways. Maglocks can be told to lock or unlock, cameras can be shut down or told to loop a fragment of footage. Commlink calls in progress can be snooped on. The other end of a commlink call can be traced to a physical location.

If the device is part of a PAN or WAN, the PAN or WAN must be hacked first. If the device is part of an s-PAN, the s-PAN must be crashed first, then the (now unattended) device must be hacked.
{{% /pageinfo %}} 


## Rigger & drone actions

{{% pageinfo %}} 
### Jump in

Used by a rigger to assume jumped-in control of a drone or vehicle. 

* If the rigger does not own the vehicle or drone, they'll need to make a Sleaze Hacking roll to Jump In to it. 
* Jump In can be done wirelessly or over a wired connection, but to do it wirelessly, the rigger must be using a dronedeck.
* This is a free action if the rigger is already connected to the target via a cable or an s-PAN via their dronedeck. Otherwise, it's a normal action.
{{% /pageinfo %}} 



{{% pageinfo %}} 
### Command Autopilot

Free action. Give a one-sentence command to a drone or vehicle autopilot. This can be combined with a Sleaze Hack to target drones or vehicles the actor does not own or control.

If a rigger is using a dronedeck that has multiple drones/vehicles in its s-PAN, they can issue the same command to any number of the drones/vehicles for a single free action. 
{{% /pageinfo %}} 



## Misc 

{{% pageinfo %}} 
### Enter host/node
Rolls: None or as Sleaze Hacking, above \
Use on: host/node

Enter a host (from the local mesh) or a node (within a host that has multiple nodes.) When entering a node from the local mesh, this also switches the decker's interface from AR to VR.

Some hosts/nodes have security checks for access; if so, they must be successfully hacked with a Sleaze Hacking roll to enter.

To exit a host/node again, see Jack Out, above.
{{% /pageinfo %}} 


{{% pageinfo %}} 
### Analyse
Requires: Notice utility \
Rolls: Hacking \
Use on: any target

Get more information about a persona, ICE, icon, or device.
{{% /pageinfo %}} 