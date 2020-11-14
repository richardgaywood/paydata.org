---
title: Dice probabilities reference
linkTitle: Dice reference
type: docs
description: The chances of beating certain target numbers in Savage Worlds
date: 2020-07-05
weight: 1000
---

The core dice mechanic in Savage Worlds is simple to explain, but not always easy to reason about: roll your attribute or skill dice (a d4, d6, d8, d10, or d12), plus your Wild Dice. Each dice explodes, ie. if you roll the maximum, you re-roll, and add on; repeat as needed. Once you've finished exploding each dice, take the highest of the two numbers.

Below are tables of the chances of hitting at least a given target number, for each type of attribute or skill dice.

For brevity, I have omitted "unskilled" (d4-2) and dice beyond d12, as well as any rolled total above 20.

{{< imgproc "d4.png" Resize "600x" >}}{{< /imgproc >}}

{{< imgproc "d6.png" Resize "600x" >}}{{< /imgproc >}}

{{< imgproc "d8.png" Resize "600x" >}}{{< /imgproc >}}

{{< imgproc "d10.png" Resize "600x" >}}{{< /imgproc >}}

{{< imgproc "d12.png" Resize "600x" >}}{{< /imgproc >}}


NB you can generate the above tables using anydice.com and the following script:

```
output [highest of [explode 1d4] and [explode 1d6]] named "d4"
output [highest of [explode 1d6] and [explode 1d6]] named "d6"
output [highest of [explode 1d8] and [explode 1d6]] named "d8"
output [highest of [explode 1d10] and [explode 1d6]] named "d10"
output [highest of [explode 1d12] and [explode 1d6]] named "d12"
```
