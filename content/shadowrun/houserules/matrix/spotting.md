---
title: Spotting icons & hiding on the Matrix
linkTitle: Spotting
type: docs
date: 2020-07-19
weight: 25
description: How to find things, and avoid being found
aliases: ["/houserules/matrix/spotting"]
---

## Spotting

"Spotting" is the process of your persona device becoming aware of some other device's icon so it can show it to you.

Spotting is an automatic function of basic Matrix protocols within a short horizon; typically around 100 metres, although it can vary with network conditions (more noise = shorter range). Your device is constantly keeping track of these devices as it helps to route traffic around in the local mesh. To detect icons further out, you can instruct your commlink or cyberdeck to actively monitor local mesh connections. See Matrix Perception, below. 

Cloud hosts are always spotted, from anywhere on the planet. Local hosts are spotted the same as any other device.

Once your persona has spotted an icon, it receives an approximate physical location and direction of travel for it, typically accurate to a couple of metres but can randomly vary. In AR, this positioning information is used by your commlink/deck/etc to decide where in your vision to place the icon. In VR, your device will probably play a little looser with reality, and icon positions will be optimised for usability (for example, overlapping icons will be spread out a bit to make them easier to see.)

For more information on the in-universe experience of spotting icons in AR and VR, see [Spotting & Positioning]({{< relref "spotting_and_positioning.md" >}}).

### Hiding

Once a persona has spotted an icon, they can keep track of it as long as it is within local mesh range. They will automatically get an approximate physical location and direction of travel, and if they also have (hacked or legitimate) access they can make that perfectly accurate via Trace Icon actions. If someone knows or suspects they are being tracked this way, they have a few options to escape:

* Try to shake the tail by moving to within range of a different uplink node, so as to break the local mesh range. The tracker can attempt to re-establish contact (via another Matrix perception action) if they can get back within range.
* Run a succesful Hide action (opposed test) to confuse the tracker and lose their attention.
 
 Note that rebooting your device is not enough to break spotting, but the persona being tracked could turn all their devices off completely instead.

## Running silent

Devices can choose to remove themselves from the local mesh, refusing incoming connections and effectively vanishing from sight. This is called running silent.

A naked device, outside of a PAN or WAN, cannot run silent. Any PAN or WAN can freely choose to run silent, however this setting applies simultaneously to all devices in the PAN or WAN. If the PAN controller is a commlink, without a Sleaze stat, it will remain very easy to detect.

## Matrix Perception

**TODO**