---
title: Matrix Actions
linkTitle: Actions
type: docs
description: All kinds of things deckers can do
date: 2021-01-16
weight: 250
---

## Offensive & defensive actions

{{% pageinfo %}} 
Action: **Cybercombat** \
Requires: Fighting utility \
Rolls: Hacking (cybercombat specialisation) vs target firewall \
Use on: s-PANs, PANs, devices, ICE

See [Cybercombat]({{< relref "cybercombat.md" >}}).
{{% /pageinfo %}} 

{{% pageinfo %}} 
Action: **DoS attack** \
Requires: Fighting utility \
Rolls: Hacking (cybercombat specialisation) vs target number \
Use on: devices

See [DoS attacks]({{< relref "combat_decking.md#denial-of-service-attacks" >}}).
{{% /pageinfo %}} 


{{% pageinfo %}} 
Action: **Sleaze** \
Requires: Persuasion utility \
Rolls: Hacking (sleaze specialisation) vs target rating \
Use on: unattended devices, PANs, hosts

Gain access to something, hopefully without anyone noticing. See [Hacking]({{< relref "hacking.md" >}}).
{{% /pageinfo %}} 


{{% pageinfo %}} 
Action: **Hide** \
Requires: Stealth utility \
Rolls: Hacking (sleaze specialisation), maybe vs Notice \
Use on: your own s-PAN on the local mesh, or your own persona a host

Can be used on the local mesh to disguise and hide your s-PAN from observers; see [Matrix Stealth]({{< relref "combat_decking.md#matrix-stealth" >}}) for more. If nobody is actively looking, the target number for this test is 4. If you are being actively hunted by ICE or a persona running the Notice utility, it is opposed by the hunter's Hacking skill.

Can be used within a host to hide your persona from ICE and security spiders, see "Deceive ICE" on Sprawlrunners pg 39 for more.
{{% /pageinfo %}} 


## Configuration commands

{{% pageinfo %}} 
Action: **Improvise utility** \
Rolls: Hacking *(no specialisation)*

See Sprawlrunners pg 43.
{{% /pageinfo %}} 


{{% pageinfo %}} 
Action: **Change utility loadout**

See Sprawlrunners pg 39. Takes a couple of seconds to do outside of combat.
{{% /pageinfo %}} 


{{% pageinfo %}} 
Action: **Jack out**

See Sprawlrunners pg 38. Can be a Free action, but then comes with risk of dumpshock.
{{% /pageinfo %}} 


## File and device actions

{{% pageinfo %}} 
Action: **Manipulate files** \
Rolls: N/A or as required \
Use on: any file(s)

Can be used to copy, edit, erase, or search for files or other data in any kind of store - a host, a node, a commlink, a data chip, etc.

Doesn't usually require a test, but if a series of edits to the files have to fool someone (or the erases to be made are subtle eg. removing entries in an access log) then a test might be needed.

Copying or erasing a very large number of files under time pressure might be a dramatic task.
{{% /pageinfo %}} 

{{% pageinfo %}} 
Action: **Decrypt file** \
Requires: Decryption utility \
Rolls: Hacking *(no specialisation)* vs file encryption rating die type \
Use on: any encrypted file

Decrypting a number of files is usually a dramatic task.
{{% /pageinfo %}} 



{{% pageinfo %}} 
Action: **Manipulate device** \
Rolls: Hacking (sleaze specialisation) or varies \
Use on: any device

Can be used to give commands to a device, or manipulate it in other ways. Maglocks can be told to lock or unlock, cameras can be shut down or told to loop a fragment of footage. Commlink calls in progress can be snooped on. The other end of a commlink call can be traced to a physical location.

If the device is part of a PAN or WAN, the PAN or WAN must be hacked first. If the device is part of an s-PAN, the s-PAN must be crashed first.

In general, the target number for this roll is the target device's Firewall stat.
{{% /pageinfo %}} 


## Rigger & drone actions

{{% pageinfo %}} 
Free action: **Jump in**

Used by a rigger to assume jumped-in control of a drone or vehicle. 

This is a normal action if the rigger is not already connected via a cable or a drone deck's s-PAN.
{{% /pageinfo %}} 



{{% pageinfo %}} 
Free action: **Give command**

Give a one-sentence command to a drone or vehicle autopilot. If the rigger is using a drone deck and has multiple drones/vehicles in its s-PAN, they can issue the same command to any number of the drones/vehicles for a single free action. 
{{% /pageinfo %}} 



## Misc 

{{% pageinfo %}} 
Action: **Enter host/node** \
Rolls: None or as Sleaze, above \
Use on: host/node

Enter a host (from the local mesh) or a node (within a host that has multiple nodes.) Simultaneously switches the decker's mode from AR to VR.

Some hosts/nodes have security checks for access; if so, they must be successfully hacked with a Sleaze roll to enter.

To exit a host/node again, see Jack Out, above.
{{% /pageinfo %}} 


{{% pageinfo %}} 
Action: **Analyse** \
Requires: Notice utility \
Rolls: Hacking *(no specialisation)* \
Use on: any target

Get more information about a persona, ICE, icon, or device.
{{% /pageinfo %}} 