---
title: Alarms
linkTitle: Alarms
type: docs
description: How the authorities catch deckers
date: 2020-11-27
weight: 300
---

Alarms are a game mechanic that simulate how aware the authorities are that there is an intruder, and how close they are to finding them.

Within a host, alarms capture the alert level of both the host's autonomous defenses (ie. ICE) as well as any metahuman sysops. On the local mesh, they measure the alert level of the mesh itself, and local GOD agents guarding the nearest uplink node.

## The alarm clock

There are separate alarm clocks for each host and for different parts of the local mesh. These clocks are typically 12-segment.

## Incrementing alarms

Alarms typically increment by 1 point for each successful hack (0 with a raise) and 2 points for each failed hack.

If a Raise on the hacking roll can be used to make the hack more effective, then the decker can choose to use the Raise to avoid the alarm increment or improve the hack effectiveness, but not both.

## Alarm consequences

Each time the alarm score is incremented, roll a d12. If the result is lower than or equal to the current alarm score, consult the table below to see what happens.

### Local mesh

* 1-3 - no effect
* 4-8 - autonomous tracing persona start to patrol, running on the nearest uplink node. Treat these as Trace ICE. 
* 9-11 - Killer ICE is deployed. 
* 12 - a GOD counter-hacker with at least a d8 in Hacking and a mid-to-high-end 'deck comes to kick ass and take names.

### Hosts

{{% alert title="Notes" %}}TBD, but depends on the host's overall security level.{{% /alert %}}



