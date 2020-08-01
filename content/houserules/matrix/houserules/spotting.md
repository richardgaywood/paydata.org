---
title: Spotting icons & hiding on the Matrix
linkTitle: Spotting
type: docs
draft: true
date: 2020-07-19
weight: 28
description: How to find things, and avoid being found
---

## Spotting

"Spotting" is the process of your persona device becoming aware of some other device's icon so it can show it to you.

Spotting is an automatic function of basic Matrix protocols within a short horizon; typically around 100 metres, although it can vary with network conditions (more noise = shorter range). Your device is constantly keeping track of these devices as it helps to route traffic around in the local mesh. To detect icons further out, you can instruct your commlink or cyberdeck to actively monitor local mesh connections. See Matrix Perception, below. 

Cloud hosts are always spotted, from anywhere on the planet. Local hosts are spotted the same as any other device.

For more information on the in-universe experience of spotting icons in AR and VR, see [Spotting & Positioning]({{< relref "spotting-and-positioning.md" >}}).

### Hiding



## Running silent

Devices can choose to remove themselves from the local mesh, refusing incoming connections and effectively vanishing from sight. This is called running silent.

A naked device, outside of a PAN or WAN, cannot run silent. A PAN or WAN controller can freely choose to run silent, however this setting applies simultaneously to all devices in the PAN or WAN.

## Matrix Perception