---
title: Key differences between Matrix rules in SR5e to SR6e
linkTitle: Comparison of 5e and 6e
type: docs
draft: true
date: 2020-07-19
weight: 100
description: Line-by-line comparison of the Matrix rulesets
---

I will ignore here the wider changes to SR6e that the decker rules fall into line with, eg. attack-rating-vs-defence-rating, Edge, and so forth. I’m concentrating on Matrix rules.

*   **Decker action economy is simplified:** mostly by making deckers able to do more with a single action and single test then they could in SR5e, where they'd often have to roll to get marks then roll again to achieve goals. This could be particularly difficult during combat, where the decker might target one opponent to get marks against, only for that opponent to be killed by other team-mates before the decker could exploit the marks. 
    *   **Hack on the Fly:** this is the stealth-orientated method for deckers to get access to things they shouldn't. In 6e, it is replaced by two separate actions: Probe[^2], which is slow but establishes backdoors, and can be done hours ahead of time. And then Backdoor Entry[^3], which exploits weaknesses found earlier by Probe to give the decker access as they need it during the run. 

<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "See more here"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[See more here](#heading=h.hi9vkszacpz3).


	*   In SR6e, **Spoof Command** can be used by a decker to send a single command to a device _without _first getting any marks/access levels on anything. In SR5e, the decker would first need a mark on a device that can control the target device to do this. Again, this gives deckers more ability to be useful in the field and react to dynamic situations. 

<p id="gdcalert2" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "See more here"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert3">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[See more here](#heading=h.w1bh1cq8pwvd).
*   **Marks have been replaced by Access Levels**, which helps reduce book-keeping slightly. There are fewer access levels than there were mark levels, and they’re easier to remember. 

<p id="gdcalert3" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "See more here"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert4">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[See more here](#heading=h.g1635x2xhawn).
*   **Overwatch Score (OS) accumulation is different**. Instead of getting 2d6 every 15 minutes, as happens in 5e, in 6e the decker accumulates OS as they remain connected to compromised systems or use hacking programs. They continue to get OS from dice rolled against them in opposed hacking tests. 

<p id="gdcalert4" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "See more here"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert5">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[See more here](#heading=h.d2qldtph72sf).
*   **Matrix damage gives penalties to dice pools** just like physical and stun damage; ie -1 per 3 boxes. This makes Data Spike deckers more dangerous, as even if they don’t do enough damage to take a device offline, they can still damage it. 

<p id="gdcalert5" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "See more here"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert6">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[See more here](#heading=h.pk9pqsaxi54g).
*   **Grids**: in SR6e, grids no longer have any mechanical effect. They are kept only as cosmetic fluff. Every host/device is equally accessible on every grid. Players never need to hop grids to get to targets[^4].


## Comparing SR5e and SR6e

What follows in this section is a line-by-line comparison of the 5e and 6e Matrix rules. I wrote this section first, to make sure I understood the changes across the two systems. I’ve kept it here in case you are interested but you shouldn’t need to read this to use the houserules presented above.


### Matrix fundamentals 


<table>
  <tr>
   <td>
   </td>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>Matrix attributes
   </td>
   <td>There are four attributes (ASDF.) These are intrinsic to the deck the decker is using.  \
 \
They act as limits on most skill checks.
   </td>
   <td>The same four attributes are intrinsic to the deck and cyberjack the decker is using.  \
 \

<p>
They are used to calculate Attack and Defence Ratings, which in turn grant Edge on Matrix actions.
   </td>
  </tr>
  <tr>
   <td>Matrix condition monitor
   </td>
   <td>8 + (Device Rating / 2) boxes \
 \
No penalties to actions from accumulated damage
   </td>
   <td>Same. \
 \
-1 to all tests per three boxes of damage
   </td>
  </tr>
  <tr>
   <td>Data Spike damage
   </td>
   <td>Persona’s Attack rating
   </td>
   <td>(Persona’s Attack rating) / 2
   </td>
  </tr>
  <tr>
   <td>Matrix damage resistance
   </td>
   <td>Device Rating + Firewall
   </td>
   <td>Firewall 
   </td>
  </tr>
  <tr>
   <td>Dumpshock
   </td>
   <td>6S if in cold-sim \
6P if in hot-sim \
 \
Resisted with Willpower + Firewall \
(if deck just got bricked, Firewall is 0) \
 \
-2 dicepool on everything for (10-Willpower) minutes
   </td>
   <td>3S if in cold-sim \
3P if in hot-sim \
 \
Resisted with Willpower only \
 \
 \

<p>
Cannot gain or use Edge on any actions for (10-Willpower) minutes
   </td>
  </tr>
  <tr>
   <td>Link-locking
   </td>
   <td>Cannot use Switch Interface Mode, Enter/Exit Host, or Reboot on the device your persona is using. \
 \
Defeated with a successful opposed Jack Out action. (But will give dump shock.)
   </td>
   <td>Same. \
 \
 \
 \
 \
Same.
   </td>
  </tr>
  <tr>
   <td>Repairing Matrix damage
   </td>
   <td>Straight test:
<p>
Hardware + Logic [Mental] \
 \
Takes 1 hour \
 \
Each hit = 1 box repaired <em>or</em> cut time in half
   </td>
   <td>Extended test: \
Engineering + Logic (num_box_damage / 1 hour) 
   </td>
  </tr>
  <tr>
   <td>Overwatch score (OS)
   </td>
   <td>
<ul>

<li>+1 OS per hit on opposing roll for any Attack or Sleaze action

<li>+2d6 (rolled in secret) every 15 minutes after OS first starts accumulating
</li>
</ul>
   </td>
   <td>
<ul>

<li>+1 OS per hit on opposing roll for any illegal action

<li>+1 for each Matrix action modified by a hacking program

<li>+1/+3 per round for each host to which you are maintaining illegal User/Admin level access
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td>Convergence
   </td>
   <td>When OS reaches 40
<p>
Not in a host:
<p>
Device takes 12 DV Matrix damage
<p>
User dumped (w/dumpshock)
<p>
Physical location reported
<p>
In a host:
<p>
Host gets three marks on deck
<p>
IC is deployed
   </td>
   <td>When OS reaches 40 \
 \
Bricks device
<p>
User dumped (w/ dumpshock)
<p>
Physical location reported
<p>
No special rules for convergence in a host.
   </td>
  </tr>
  <tr>
   <td>Matrix initiative
   </td>
   <td>AR: physical init \
 \
VR cold sim:  \
Data Processing + Int + 3d6 \
 \
VR hot sim:  \
Data Processing + Int + 4d6 \
+2 dice pool to all actions
   </td>
   <td>AR: physical init \
 \
VR cold sim:  \
Data Processing + Int + 2d6 \
 \
VR hot sim:  \
Data Processing + Int + 3d6 \

   </td>
  </tr>
</table>



### 


### Skills

There is no major difference in skills between 5e and 6e, other than the fact that the 5e Skill Groups become Skills in 6e. The way the skills are used are the same however.


<table>
  <tr>
   <td><strong>5e skill</strong>
   </td>
   <td><strong>5e skill group / 6e skill</strong>
   </td>
  </tr>
  <tr>
   <td>Cybercombat
   </td>
   <td rowspan="3" >Cracking <em>(illegal)</em>
   </td>
  </tr>
  <tr>
   <td>Electronic Warfare
   </td>
  </tr>
  <tr>
   <td>Hacking
   </td>
  </tr>
  <tr>
   <td>Computer
   </td>
   <td rowspan="3" >Electronics <em>(legal)</em>
   </td>
  </tr>
  <tr>
   <td>Hardware
   </td>
  </tr>
  <tr>
   <td>Software
   </td>
  </tr>
  <tr>
   <td>Compiling
   </td>
   <td rowspan="3" >Tasking <em>(Resonance - Technomancers only)</em>
   </td>
  </tr>
  <tr>
   <td>Decompiling
   </td>
  </tr>
  <tr>
   <td>Registering
   </td>
  </tr>
</table>



### Any action using any skill in the Cracking group - so any action that uses the Cybercombat, Electronic Warfare, or Hacking skills - is considered to be illegal by the Grid Overwatch Division. These actions will increase a decker’s overwatch score when used.


### Security & bypassing it


<table>
  <tr>
   <td>
   </td>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>Getting into a Host \

   </td>
   <td>
<ul>

<li>Legit: Invite Mark

<li>Forceful: Brute Force

<li>Sneaky: Hack on the Fly			
</li>
</ul>
   </td>
   <td>
<ul>

<li>Just go in without any access level (if the host allows it)

<li>Brute force

<li>Probe -> backdoor	
		
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td>Getting more than one level at once
   </td>
   <td>On Brute Force or Hack on the Fly:
<p>
By default, they only grant one mark. Decker can shoot for two marks at a -4 dice penalty, or three marks at a -10 penalty.
   </td>
   <td>Backdoor: always grants Admin access.
<p>
Brute Force: normally grants User access. Decker can opt to attempt for Admin access, but target gets +2 dice pool and +4 Defence Rating in their test.
   </td>
  </tr>
  <tr>
   <td>Legitimate access to public Hosts
   </td>
   <td>The host sends Invite Mark to let users get one mark. The user does that, then uses Enter Host.
   </td>
   <td>The host can be configured to allow access to users with Outsider access level.
   </td>
  </tr>
</table>



### 


### Actions


<table>
  <tr>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>

<p id="gdcalert11" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image1.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert12">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


<img src="images/image1.png" width="" alt="alt_text" title="image_tooltip">

   </td>
   <td>

<p id="gdcalert12" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image2.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert13">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


<img src="images/image2.png" width="" alt="alt_text" title="image_tooltip">

<p>


<p id="gdcalert13" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image3.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert14">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


<img src="images/image3.png" width="" alt="alt_text" title="image_tooltip">

   </td>
  </tr>
</table>



#### Getting in / Mark manipulation

Where I list the 6e mechanics as “same” below, what I mean is:



*   The 6e skill is the same as the 5e skill’s corresponding skill group; so, for example, if the 5e skill is Software and the 6e skill is Electronics, then these are the same.
*   A 5e Simple action is the same as a 6e Minor action, and likewise for Complex / Major.
*   I will highlight key differences in the actions, to make them easier to spot.

<table>
  <tr>
   <td>
   </td>
   <td>
<strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>Brute Force \
<em>(illegal)</em> \

   </td>
   <td><em>roll: </em>Cybercombat + Logic [Attack] \
<em>resist: </em>Willpower + Firewall \
<em>action:</em> Complex
<p>
<em>requires: </em>no marks
<p>
Gain one mark on target per net hit.  \

<p>
Every two net hits optionally also does 1 DV or Matrix damage, resisted with Device Rating + Firewall.
<p>
Can attempt to get two marks in one go at -4 dice pool, or three marks in one go at -10.
<p>
Can also use this action to hop grids.
   </td>
   <td><em>roll: </em>same \
<em>resist: </em>same \
<em>action:</em> same \
<em>requires: </em>same
<p>
Gain User or Admin access on the target if the test succeeds.
<p>
No mechanic for doing Matrix damage.
<p>
Can attempt to get Admin access from Outsider, at a cost of +2 dice on the resistance test and +4 bonus to target’s Defence Rating.
<p>
No mechanics for grid hopping.
   </td>
  </tr>
  <tr>
   <td>Hack on the Fly (5e) \

<p>
Probe /  \
Backdoor Entry (6e)
<p>
<em>(illegal)</em>
   </td>
   <td><strong>Hack on the Fly:</strong>
<p>
<em>roll: </em>Hacking + Logic [Sleaze] \
<em>resist: </em>Intuition + Firewall \
<em>action:</em> Complex
<p>
<em>requires: </em>no marks
<p>
Gain one mark on target per net hit.  \

<p>
Every two net hits also counts as a one hit on a Matrix Perception test, so you get some information too.
<p>
Can attempt to get two marks in one go at -4 dice pool, or three marks in one go at -10.
<p>
Can also use this action to hop grids.
   </td>
   <td><strong>Probe:</strong>
<p>
<em>roll: </em>same \
<em>resist: </em>Willpower + Firewall or Firewall x2 \
<em>action:</em> <em>Extended, 1 minute</em>[^12] \
<em>requires: </em>no access
<p>
<strong>Backdoor Entry:</strong>
<p>
<em>roll: </em>same \
<em>resist: </em>Willpower + Firewall \
<em>action:</em> Major Action \
<em>requires: </em>no access
<p>
See 

<p id="gdcalert14" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "above"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert15">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.hi9vkszacpz3">above</a> for a discussion of these actions.
<p>
No mechanics for grids.
   </td>
  </tr>
  <tr>
   <td>Erase Matrix Signature
<p>
<em>(illegal)</em> \
 \

   </td>
   <td><em>roll: </em>Computer + Resonance [Attack]
<p>
<em>resist: </em>Signature Rating x 2
<p>
<em>action:</em> Complex Action
<p>
<em>requires: </em>No marks
<p>
If the test is successful, the signature dissipates.
<p>
Character must have a Resonance rating to attempt this action. This is a real Matrix Action, and illegal, so risks Matrix damage and Overwatch Score when done.
   </td>
   <td><em>roll: </em>Electronics + Logic
<p>
<em>resist: </em>Willpower + Firewall or Firewall x2
<p>
<em>action:</em> same
<p>
<em>requires: </em>User/Admin
<p>
Same.
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Invite Mark
<p>
<em>(legal)</em>
   </td>
   <td>No test
   </td>
   <td>N/A
   </td>
  </tr>
  <tr>
   <td>Erase Mark
<p>
<em>(illegal)</em>
   </td>
   <td><em>roll: </em>Computer + Logic [Attack]
<p>
<em>resist: </em>Willpower + Firewall
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>3 marks
   </td>
   <td>N/A
   </td>
  </tr>
</table>



### 


#### Device Manipulation


<table>
  <tr>
   <td>
   </td>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>Control Device
<p>
<em>(legal)</em>
   </td>
   <td><em>roll: </em>varies <em>or</em>
<p>
<em>    </em>Electronic Warfare + Intuition [Sleaze]
<p>
<em>resist: </em>Intuition + Firewall
<p>
<em>action:</em> varies
<p>
<em>requires: </em>varies
<p>
Perform an action through a device you control.
<p>
Test is usually determined by the device you are controlling eg. a turret would be Gunnery+Agility.
<p>
All tests are limited by [Data Processing] if that is lower than the limit you’d normally have.
<p>
If there is no test associated with an action, use the test above.
<p>
Can use this against multiple targets. If you are the Owner of them all and it’s the same command, no penalty. Otherwise, have to split your dice pool.
<p>
Free/Simple/Complex is determined by the command given, as is the access level required (1/2/3 marks.)
<p>
This is a Sleaze action, so OS accumulates.
   </td>
   <td><em>roll: </em>varies <em>or</em>
<p>
<em>    </em>change stat to Logic
<p>
<em>resist: </em>Willpower + Firewall
<p>
<em>action:</em> Major
<p>
<em>requires: </em>User/Admin
<p>
Same.
<p>
Same.
<p>
N/A.
<p>
Same.
<p>
Not mentioned.
<p>
Always a Major action. Requirement for User or Admin access determined by GM fiat.
<p>
This is a legal action.
<p>
If in AR, use normal physical stats. If in VR, use mental stats (Body->Willpower, Agility->Logic, Reaction->Intuition,. Strength->Charisma.)
   </td>
  </tr>
  <tr>
   <td>Format Device  \
<em>(illegal in 5e)</em>
<p>
<em>(legal in 6e)</em>
   </td>
   <td><em>roll: </em>Computer + Logic [Sleaze]
<p>
<em>resist: </em>Willpower + Firewall
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>3 marks
<p>
Next time device reboots, it fails to restart until repaired.
<p>
Repair is an extended Software+Logic [Mental] (12, 1 hour) test.
   </td>
   <td><em>roll: </em>same \
<em>resist: </em>Willpower + Firewall or Firewall x2 \
<em>action:</em> same \
<em>requires: </em>same (Admin)
<p>
Same.
<p>
Repair is the same as a bricked device, requiring number of hits equal to the devices Device Rating.
   </td>
  </tr>
  <tr>
   <td>Reboot Device
<p>
<em>(legal)</em>
   </td>
   <td><em>roll: </em>Computer + Logic [Data Processing]
<p>
<em>resist: </em>Willpower + Firewall
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>3 marks
<p>
Can’t be linked-locked, suffer dumpshock, reset OS. Comes back online at end of next Combat Turn.
   </td>
   <td><em>roll: </em>same \
<em>resist: </em>Willpower + Firewall or Firewall x2 \
<em>action:</em> same \
<em>requires: </em>same (Admin)
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Spoof Command
<p>
<em>(illegal)</em>
   </td>
   <td><em>roll: </em>Hacking + Intuition [Sleaze]
<p>
<em>resist: </em>Logic + Firewall
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>1 mark, on some other device
<p>
Give device or agent command.
<p>
Need mark on owner you are imitating.
<p>
<em>“You spoof a device’s owner’s identity, making the device think that your command is a legitimate one from its owner. You need one mark on the icon you are imitating; you do not need a mark on the target. The opposing dice roll is still based on the target, though. This trick only works on devices and agents, not IC, sprites, hosts, personas, or any other icons.“ </em>
   </td>
   <td><em>roll: </em>Cracking + Logic \
<em>resist: </em>Firewall + (Data Processing or Pilot) \
<em>action:</em> same \
<em>requires: </em>none
<p>
Same.
<p>
No access needed on anything.
<p>
<em>“You send a signal to a device with a command the target perceives as coming from its owner. The device then automatically attempts to perform the action as its next available major action.”</em>
   </td>
  </tr>
</table>



#### File Manipulation


<table>
  <tr>
   <td>
   </td>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>Crack File
<p>
<em>(illegal)</em>
   </td>
   <td><em>roll: </em>Hacking + Logic [Attack]
<p>
<em>resist: </em>Protection Rating x2
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>1 mark
<p>
Remove encryption on a file.
   </td>
   <td><em>roll: </em>same \
<em>resist: </em>same \
<em>action:</em> same \
<em>requires: </em>same
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Disarm Data Bomb \

<p>
<em>(illegal</em>[^13]<em>)</em>
   </td>
   <td><em>roll: </em>Software + Intuition [Firewall]
<p>
<em>resist: </em>Data Bomb Rating x2
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>no marks
<p>
Attempt to disarm a data bomb. Bomb deleted if you get any net hits. If not, data bomb activates, damaging file it was attached to.
   </td>
   <td><em>roll: </em>Cracking + Logic \
<em>resist: </em>same \
<em>action:</em> same \
<em>requires: </em>User or Admin
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Edit File
<p>
<em>(legal)</em>
   </td>
   <td><em>roll: </em>Computer + Logic [Data Processing]
<p>
<em>resist: </em>Intuition + Firewall
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>1 mark
<p>
Create, change, copy, delete file.
<p>
Defender is either the host holding the file or the owner of the file if it’s not on a host.
   </td>
   <td><em>roll: </em>same \
<em>resist: </em>same <em>or </em>Intuition + Sleaze[^14] \
<em>action:</em> same \
<em>requires: </em>same
<p>
Same.
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Set Data Bomb
<p>
<em>illegal</em>
   </td>
   <td><em>roll: </em>Software + Logic [Sleaze]
<p>
<em>resist: </em>Device Rating x2
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>no marks
<p>
Player chooses: 
<ul>

<li>Rating of data bomb (up to net hits on test)

<li>Effect (delete file or not?)

<li>Passcode to access file

<p>
A file can only have one data bomb on it at any one time.
<p>
Bomb triggers when anyone tries to read, edit, copy, protect, delete, or put another bomb on the file without using the passcode.
<p>
It does (Rating)D6 Matrix damage to the icon that tripped it.
<p>
Bomb can be detected with Matrix Perception and then removed with Disarm Data Bomb action.
</li>
</ul>
   </td>
   <td><em>roll: </em>same \
<em>resist: </em>same \
<em>action:</em> same \
<em>requires: </em>same
<p>
Same
<p>
Same
<p>
Same
<p>
Does (Rating x 4) Matrix damage.
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Encrypt File 
<p>
<em>(legal)</em>
   </td>
   <td>N/A
   </td>
   <td><em>roll: </em>Electronics + Logic \
<em>action:</em> Major \
<em>requires: </em>User/Admin
<p>
Number of hits is the Encryption Rating on the file.
   </td>
  </tr>
</table>



### 


#### Information Gathering


<table>
  <tr>
   <td>
   </td>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>Check Overwatch Score \

<p>
<em>(illegal)</em>
   </td>
   <td><em>roll: </em>Electronic Warfare + Logic [Sleaze]
<p>
<em>resist: </em>6 dice
<p>
<em>action:</em> Simple
<p>
<em>requires: </em>no marks
<p>
Find out your own Overwatch Score.
<p>
The 6 dice rolled against this increases your score, and the player finds the score <em>before</em> they are (secretly) added, not afterward.
   </td>
   <td><em>roll: </em>Same
<p>
<em>resist: </em>threshold 4
<p>
<em>resist: </em>10 dice (if target is a stealth tag)
<p>
<em>action:</em> Major
<p>
<em>requires: </em>Admin[^15]
<p>
Same.
<p>
Doesn’t seem to increase your OS…?
   </td>
  </tr>
  <tr>
   <td>Matrix Perception
<p>
<em>(legal)</em>
   </td>
   <td><em>roll: </em>Computer + Intuition [Data Processing]
<p>
<em>resist: (if opposed) </em>Logic + Sleaze
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>no marks
<p>
Simple test when used to analyze a Matrix object or scan for silent running icons. For each net hit, get an answer to one question on the table below.
<p>
If trying to spot icons further than 100 m away, take a simple test: first hit spots target, then additional hits reveal things as above.
<p>
To spot an icon running silent, make an opposed test as above. First hit spots it, other hits can be used for more information.
<p>


<p id="gdcalert15" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image4.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert16">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


<img src="images/image4.png" width="" alt="alt_text" title="image_tooltip">

   </td>
   <td><em>roll: </em>same
<p>
<em>resist: </em>same
<p>
<em>action:</em> Major; Minor if user has ‘deck or Resonance
<p>
<em>requires: </em>no access
<p>
“A successful test gives you information about the target[^16]. With a tie, you can perceive the item’s icon. A single net hit will give you basic information, such as device rating, or whatever name the device or icon
<p>
calls itself. Two net hits will give you more specific information, including individual attribute ratings, and what programs it is currently running. Additional hits will give you more information based on what
<p>
the gamemaster wishes to reveal.
<p>
This test can also be used to attempt to spot any icons in the vicinity that are running silent.”
   </td>
  </tr>
  <tr>
   <td>Matrix Search
<p>
(legal)
   </td>
   <td><em>roll: </em>Computer + Intuition [Data Processing]
<p>
<em>resist: </em>threshold; see below
<p>
<em>action:</em> special
<p>
<em>requires: </em>no marks
<p>
Search the Matrix for information about a subject.
<p>
Threshold determined by table below.
<p>
Hit beyond the threshold can be used to reduce the time taken (divide the time by the number of net hits.) If you fail the test, still spend the entire base time looking.
<p>
Can also use Matrix Search while inside a host. Always has a base time of 1 minute. Only works if the information is online within the host; some is in cold (offline) storage.
<p>


<p id="gdcalert16" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image5.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert17">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


<img src="images/image5.png" width="" alt="alt_text" title="image_tooltip">

   </td>
   <td><em>roll: </em>same
<p>
<em>resist: </em>none
<p>
<em>action:</em> “extended, 10 minutes”
<p>
<em>requires: </em>same
<p>
Same.
<p>
Threshold determined by Legwork Table (see below.)
<p>
N/A. 
<p>
Replaced by the Hash Search action (see below.)
<p>


<p id="gdcalert17" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image6.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert18">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


<img src="images/image6.png" width="" alt="alt_text" title="image_tooltip">

   </td>
  </tr>
  <tr>
   <td>Snoop
<p>
<em>(illegal)</em>
   </td>
   <td><em>roll: </em>Electronic Warfare + Intuition [Sleaze]
<p>
<em>resist: </em>Logic + Firewall
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>1 mark
<p>
Intercept traffic sent to and from target. Listen to, view, or read data live, or save it to storage.
   </td>
   <td><em>roll: </em>stat changes to Logic \
<em>resist: </em>same <em>or </em>Data Processing + Firewall[^17] \
<em>action:</em> same \
<em>requires: </em>Admin access
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Trace Icon
<p>
 \
<em>(illegal but I think should be legal)</em>
   </td>
   <td><em>roll: </em>Computer + Intuition [Data Processing]
<p>
<em>resist: </em>Willpower + Sleaze
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>2 marks
<p>
Find the physical location of a device or persona. 
<p>
After succeeding with this action, you know the target;’s location as long as you have at least one mark. 
<p>
Doens’t work on hosts (as they have no physical location), or IC programs (as they live inside hosts.)
   </td>
   <td><em>roll: </em>same \
<em>resist: </em>same <em>or</em> Firewall + Sleaze[^18] \
<em>action:</em> same \
<em>requires: </em>Admin access
<p>
Same.
<p>
You know the location “as long as you can detect the target.”
<p>
Same, but it does work on offline hosts with physical hardware. (But you likely know where the are already.)
   </td>
  </tr>
  <tr>
   <td>Hash Check[^19] \
 \
(illegal)
   </td>
   <td>N/A
   </td>
   <td><em>roll: </em>Electronics + Logic (1 or 4) \
<em>resist: </em>threshold 1 or 4 \
<em>action:</em>Major \
<em>requires: </em>User access
<p>
Search for a file on a host or device based on known metadata. Threshold is 1 if the hash data was known (eg. given to them by Mr Johnson), 4 otherwise.
<p>
Passing the test narrows the number of possible files down to 32. For every net hit, that number is divided in half. So 5 net hits in total will narrow it down to a single file.
<p>
If the number of matches is too large after the first test, can repeat, with the usual -2 dice pool penalty. Again, each net hit reduces the number of possible files by 2.
   </td>
  </tr>
</table>



### 


#### Matrix Combat


<table>
  <tr>
   <td>
   </td>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>Crash Program  \
(illegal)
   </td>
   <td><em>roll: </em>Cybercombat + Logic [Attack]
<p>
<em>resist: </em>Intuition + Firewall
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>1 mark
<p>
Overload a chosen program on a chosen target, crashing it. Can use Matrix Perception first to figure out what programs are running, or can observe its effects. Device has to reboot to use the program again.
   </td>
   <td><em>roll: </em>same \
<em>resist: </em>Data Processing + Device Rating \
<em>action: </em>same \
<em>requires: </em>Admin access
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Data Spike  \
(illegal)
   </td>
   <td><em>roll: </em>Cybercombat + Logic [Attack]
<p>
<em>resist: </em>Intuition + Firewall
<p>
<em>damage resist: </em>Device Rating + Firewall
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>no marks
<p>
Does Matrix damage.  \
 \
DV = persona’s Attack rating
<p>
...plus one box of damage per net hit
<p>
...plus two additional boxes of damage for each mark you have on the target
   </td>
   <td><em>roll: </em>same \
<em>resist: </em>Data Processing + Firewall
<p>
<em>damage resist: </em>Firewall \
<em>action: </em>same \
<em>requires: </em>same
<p>
Same.
<p>
DV = persona’s Attack rating / 2 (round up)
<p>
...same
<p>
...no additional damage from access levels
   </td>
  </tr>
  <tr>
   <td>Full Matrix Defence (legal)
   </td>
   <td><em>action:</em> Interrupt (-10 init)
<p>
<em>requires: </em>4 marks (owner)[^20]
<p>
Adds Willpower to defence pool against all Matrix Attack actions for the rest of the Combat Turn.
   </td>
   <td><em>action: </em>Major \
<em>requires: </em>any access level
<p>
Add Firewall to the “next time you are attacked in the Matrix.”[^21]
   </td>
  </tr>
  <tr>
   <td>Tarpit
   </td>
   <td>N/A
   </td>
   <td>

<p id="gdcalert18" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "See above"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert19">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.w1bh1cq8pwvd">See above</a>.
<p>
Tarpit is a sort of stun-damage analog to the Matrix damage attack of Data Spike.
   </td>
  </tr>
</table>



### 


#### Miscellaneous


<table>
  <tr>
   <td>
   </td>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>Change Icon 
<p>
<em>(legal)</em>
   </td>
   <td><em>action:</em> Simple
<p>
<em>requires: </em>4 marks
<p>
Change target’s icon to one you have a copy of or have designed yourself. This doesn’t change the results of a Matrix Perception action, but might fool a cursory inspection. You can target your own icon.
   </td>
   <td><em>action:</em> same
<p>
<em>requires: </em>User/Admin
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Enter/Exit Host 
<p>
<em>(legal)</em>
   </td>
   <td><em>action:</em> Simple
<p>
<em>requires: </em>1 mark on host
   </td>
   <td><em>action:</em> same
<p>
<em>requires: </em>depends on host
   </td>
  </tr>
  <tr>
   <td>Grid hop
<p>
<em>(legal)</em>
   </td>
   <td><em>action:</em> Complex
<p>
<em>requires: </em>no marks
<p>
Can only do this if you have access to the target grid. If you don’t have legal access, can use Brute Force or Hack on the Fly. 
<p>
Can’t hop grids inside a host.
   </td>
   <td>N/A (removed)
   </td>
  </tr>
  <tr>
   <td>Hide
<p>
(<em>illegal)</em>
   </td>
   <td><em>roll: </em>Electronic Warfare + Intuition [Sleaze]
<p>
<em>resist: </em>Intuition + Data Processing
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>no marks
<p>
If test succeeds, target has to do a new Matrix Perception test to find you again.
<p>
Cannot hide from a target that has a mark on you.
   </td>
   <td><em>roll: </em>same \
<em>resist: </em>same <em>or</em> Data Processing + Sleaze \
<em>action: </em>same \
<em>requires: </em>same
<p>
Same.
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Jack Out
<p>
(<em>legal)</em>
   </td>
   <td><em>roll: </em>Hardware + Willpower [Firewall]
<p>
<em>resist: </em>Logic + Attack (only if link-locked)
<p>
<em>action:</em> Simple
<p>
<em>requires: </em>4 marks
<p>
Jacks out, reboots device being used.
<p>
Suffer dumpshock if in VR.
<p>
Defence pool only applies if persona is link-locked and comes from the persona that link-locked you; if multiple you have to roll against them all. 
<p>
Can only Jack Out to yourself.
   </td>
   <td><em>roll: </em>same \
<em>resist: </em>Charisma[^22] + Data Processing <em>or</em>
<p>
            Attack + Data Processing \
<em>action: </em>Major \
<em>requires: </em>any
<p>
Same.
<p>
Same.
<p>
Same.
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Jam Signals
<p>
<em>(illegal)</em>
   </td>
   <td><em>roll: </em>Electronic Warfare + Logic [Attack]
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>4 marks
<p>
Turns device into jammer. 
<p>
Range: 100m
<p>
Jam rating: hits on test
<p>
Cannot use it for anything else while it is being a jammer.
   </td>
   <td><em>roll: </em>same \
<em>action: </em>same \
<em>requires: </em>Admin[^23]
<p>
Same.
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Jump In
<p>
<em>(legal)</em>
   </td>
   <td><em>roll: </em>Electronic Warfare + Logic [Data Proc]
<p>
<em>resist: </em>Willpower + Firewall
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>3 marks
<p>
Jump into vehicle, drone, or other device.
<p>
Requirements:
<ol>

<li>Have 3+ marks

<li>Be in VR

<li>Device has to have rigger adaptation

<li>Have to have a control rig

<p>
If you are device owner or you have permission from device owner, no test is necessary.
<p>
Cannot jump in if someone else is already jumped in to it.
</li>
</ol>
   </td>
   <td><em>roll: </em>Electronics + Logic \
<em>resist: </em>same <em>or</em> Firewall x2 \
<em>action: </em>same \
<em>requires: </em>User/Admin
<p>
Same.
<p>
Same.
<p>
Same.
<p>
Same.
<p>
When jumped in, the device’s icon becomes part of your persona.
   </td>
  </tr>
  <tr>
   <td>Send Message
<p>
<em>(legal)</em>
   </td>
   <td><em>action:</em> Simple
<p>
<em>requires: </em>no marks
<p>
Send a message to a commcode: a short sentence, or an image, or a single file. If you’re using the Matrix through DNI (even if via AR), can send a longer message (about a paragraph.) Can also use this to open a live feed (audio/video/whatever) to one or more recipients.
   </td>
   <td><em>action: </em>same \
<em>requires: </em>same
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Switch Interface Mode
<p>
<em>(legal)</em>
   </td>
   <td><em>action:</em> Simple
<p>
<em>requires: </em>no marks
<p>
Switch from AR to VR, or vice versa. Cannot do this if you are link-locked. Can’t do it to other people.
   </td>
   <td><em>action: </em>same \
<em>requires: </em>same
<p>
Same.
<p>
 \

<p>
Can also turn silent running on or off.
   </td>
  </tr>
</table>



### 


### PANs & WANs


<table>
  <tr>
   <td>
   </td>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>Firewall & hacking in
   </td>
   <td>All devices inside the PAN can use the commlink, deck, or host’s Firewall stat to make Matrix defence tests, unless it is being hacked via a direct cable connection.
<p>
If you get a mark on any slave, you also get a mark on the master.
   </td>
   <td>All devices inside the PAN can use the master commlink or deck’s Firewall stat and the master device’s owner’s Willpower attribute to make Matrix defence tests.
<p>
Deckers attempting to gain access levels to a device inside the PAN must first compromise the PAN. They cannot Hack on the Fly or Probe devices within a PAN directly. Once they get a level of access against the PAN (User or Admin), they have that level of access for every device on the PAN. \
 \
However, Data Spike, Tarpit, and Spoof Command can be used against any device a decker can see on the Matrix, regardless of its PAN status, and without hacking the PAN first.[^24]
   </td>
  </tr>
  <tr>
   <td>Direct connections
   </td>
   <td>If you are directly connected to a device inside a PAN or WAN, you bypass the cyberdeck or host’s Firewall stat.
<p>
Remember that if you get a mark on a slave, you also get a mark on the host.
   </td>
   <td>No specific rules. Getting a direct connection to a device still rolls the PAN/WAN’s full Firewall stat.
   </td>
  </tr>
  <tr>
   <td>Maximum size & nesting PANs
   </td>
   <td>A commlink or deck can slave up to (Device Rating x3) devices. PANs cannot be nested.
   </td>
   <td>RAW: A commlink or deck can slave up to (Device Rating) devices.[^25]
   </td>
  </tr>
  <tr>
   <td>Iconography
   </td>
   <td>
   </td>
   <td>“The PAN is the primary means of displaying the persona, or the icon of the user. Programs and devices attached to the PAN appear as smaller representations of their normal icons, carried by the persona.”
   </td>
  </tr>
  <tr>
   <td>WANs
   </td>
   <td>Same as a PAN, but slaved to a host instead of a commlink or cyberdeck
<p>
If you are inside a host with a WAN, you are considered to be directly connected to all devices in the WAN
   </td>
   <td>Not explicitly mentioned.
   </td>
  </tr>
</table>



### Noise

Nose is the same in 5e and 6e: the same numeric values, under the same conditions, and with the same mechanical effect.


### 


### Running silent & Matrix Perception


<table>
  <tr>
   <td>
   </td>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>Basics
   </td>
   <td>Switching to silent running is a Simple Action. 
<p>
Running silent imposes a –2 dice pool modifier to all of your Matrix actions due to “the processing power needed to cover your tracks.”
<p>
Silent running is switched on/off on a per-device basis.
   </td>
   <td>Switching to silent running is the “Change Device Mode” Minor Action.
<p>
No dice pool penalty. 
<p>
Silent running is applied to an entire PAN at once (say, a user’s commlink and all their devices.)
   </td>
  </tr>
  <tr>
   <td>Matrix Perception
<p>
<em>(legal)</em>
   </td>
   <td><em>roll: </em>Computer + Intuition [Data Processing]
<p>
<em>resist: (if opposed) </em>Logic + Sleaze
<p>
<em>action:</em> Complex
<p>
<em>requires: </em>no marks
<p>
Simple test when used to analyze a Matrix object or scan for silent running icons. For each net hit, get an answer to one question on the table below.
<p>
If trying to spot icons further than 100 m away, take a simple test: first hit spots target, then additional hits reveal things as above.
<p>
To spot an icon running silent, make an opposed test as above. First hit spots it, other hits can be used for more information.
   </td>
   <td><em>roll: </em>same
<p>
<em>resist: </em>same
<p>
<em>action:</em> Major; Minor if user has ‘deck or Resonance
<p>
<em>requires: </em>no access
<p>
“A successful test gives you information about the target[^26]. With a tie, you can perceive the item’s icon. A single net hit will give you basic information, such as device rating, or whatever name the device or icon
<p>
calls itself. Two net hits will give you more specific information, including individual attribute ratings, and what programs it is currently running. Additional hits will give you more information based on what
<p>
the gamemaster wishes to reveal.
<p>
This test can also be used to attempt to spot any icons in the vicinity that are running silent.”
   </td>
  </tr>
  <tr>
   <td>Silent running vs Matrix Perception
   </td>
   <td>If there are multiple icons running silent, user has to pick icons (at random) to be revealed.
   </td>
   <td>User can reveal all icons that fail the Matrix perception resistance test in one go.
   </td>
  </tr>
  <tr>
   <td>Range for automatically spotting icons
   </td>
   <td>Everything not running silent within 100 m of your deck or commlink is always considered spotted.
   </td>
   <td>No defined concept of “spotting.”
   </td>
  </tr>
</table>



### Hosts & intrusion countermeasures


<table>
  <tr>
   <td>
   </td>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>Host stats
   </td>
   <td>Host Rating, HR+1, HR+2, HR+3 \

<p>
Distributed across ASDF similarly to how cyberdecks work
   </td>
   <td>Same.
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Launching IC
   </td>
   <td>Launch 1 IC per Combat Turn (at the beginning of the turn). Can run up to (Host Rating) IC simultaneously. Can only run 1 copy of any given IC at once. Can restart “bricked” IC next turn
   </td>
   <td>Same.
   </td>
  </tr>
  <tr>
   <td>IC stats
   </td>
   <td>(Host Rating x 2) for IC Attack Rating (limited by hosts’s [Attack]).
<p>
Initiative: Host Rating + Data Processing + 4D6.  \

<p>
Condition monitor: 8+(Host Rating /2)[^27]
<p>
 \
Defensive rolls and effects vary by IC type.
   </td>
   <td>(Host Rating x 2) for Attack Rating, Condition Monitor, and most rolls. \

<p>
Initiative: (Data Processing x 2) + 3D6.  \

<p>
Condition monitor: (Host Rating x2)
<p>
Same.
   </td>
  </tr>
</table>



### IC


<table>
  <tr>
   <td>
   </td>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>All IC rolls the same attack roll:
<p>
<em>roll: </em>(Host Rating x 2) [Attack]
<p>
<em>action:</em> Complex
   </td>
   <td>All IC rolls the same attack roll:
<p>
<em>roll: </em>(Host Rating x 2)
<p>
<em>attack rating:</em> Host Attack Rating
<p>
<em>action:</em> Complex
   </td>
  </tr>
  <tr>
   <td>Acid
   </td>
   <td><em>resist: </em>Willpower + Firewall
<p>
If it gets 1 or more net hits, reduces target’s Firewall by 1. 
<p>
If Firewall is 0, causes 1 DV Matrix damage per net hit. 
<p>
Firewall stat cannot be restored until you reboot.
   </td>
   <td><em>resist: </em>same
<p>
Firewall attribute reduced by number of net hits.
<p>
Does not cause Matrix damage.
<p>
Firewall stat restores itself after you leave the host, at the rate of 1 point per minute.
   </td>
  </tr>
  <tr>
   <td>Binder
   </td>
   <td><em>resist: </em>Willpower + Data Processing
<p>
Same as Acid, above, but affecting Data Processing.
   </td>
   <td><em>resist: </em>same
<p>
Same.
<p>
If Data Processing is reduced to 0, no Matrix actions can be taken at all.
   </td>
  </tr>
  <tr>
   <td>Black IC
   </td>
   <td><em>resist: </em>Intuition + Firewall
<p>
If get 1+ hits, target is link-locked.
<p>
(Attack) DV Matrix damage
<p>
…+1 DV per net hit
<p>
…+2 DV per mark on target
<p>
Plus the same amount of biofeedback damage
   </td>
   <td><em>resist: </em>same
<p>
Doesn’t mention link-locking.[^28]
<p>
Deals (host rating + net hits) in Matrix damage and biofeedback damage.
   </td>
  </tr>
  <tr>
   <td>Blaster
   </td>
   <td><em>resist: </em>Logic + Firewall
<p>
As Black IC but only causes Stun biofeedback damage.
   </td>
   <td><em>resist: </em>same
<p>
(Host rating[^29]) Matrix  damage and link-locks target.
   </td>
  </tr>
  <tr>
   <td>Crash
   </td>
   <td><em>resist: </em>Intuition + Firewall
<p>
If Crash IC (or its host) has a mark on you, a random one of your programs crashes. It cannot be run again without a deck reboot.
   </td>
   <td><em>resist: </em>same
<p>
Same. Doesn’t need a mark on you, though.
   </td>
  </tr>
  <tr>
   <td>Jammer
   </td>
   <td><em>resist: </em>Intuition + Firewall
<p>
Same as Acid, above, but affecting Firewall.
   </td>
   <td><em>resist: </em>Willpower + Attack
<p>
Same as Acid, above, but affecting Firewall.
<p>
No Attack actions can be used if your attack rating is 0.
   </td>
  </tr>
  <tr>
   <td>Killer 
   </td>
   <td><em>resist: </em>Intuition + Firewall
<p>
(Attack) DV Matrix damage
<p>
…+1 DV per net hit
<p>
…+2 DV per mark on target
   </td>
   <td><em>resist: </em>same
<p>
Deals (host rating + net hits) in Matrix damage.
   </td>
  </tr>
  <tr>
   <td>Marker
   </td>
   <td><em>resist: </em>Willpower + Sleaze
<p>
Same as Acid, above, but affecting the Sleaze attribute.
   </td>
   <td><em>resist: </em>same
<p>
Same.
   </td>
  </tr>
  <tr>
   <td>Patrol
   </td>
   <td>Patrols a host, regularly using Matrix Perception actions on all icons within it.
   </td>
   <td>Rolls Matrix Perception once per minute.
   </td>
  </tr>
  <tr>
   <td>Scramble
   </td>
   <td><em>resist: </em>Willpower + Firewall
<p>
If the host has three marks on you and you are hit by this, it immediately reboots your deck, hitting you with dumpshock.
   </td>
   <td><em>resist: </em>same
<p>
If it hits, it forces you to reboot on your next turn, unless you are link-locked. (No marks required.)
   </td>
  </tr>
  <tr>
   <td>Sparky
   </td>
   <td><em>resist: </em>Intuition + Firewall
<p>
(Attack) DV Matrix damage
<p>
…+1 DV per net hit
<p>
…+2 DV per mark on target
<p>
Plus the same amount of biofeedback damage.
   </td>
   <td><em>resist: </em>same
<p>
Deals (host rating + net hits) in biofeedback damage.
   </td>
  </tr>
  <tr>
   <td>Tar baby
   </td>
   <td><em>resist: </em>Logic + Firewall
<p>
If it hits, you are link-locked. 
<p>
If you’re already link-locked, it puts a mark on you.
   </td>
   <td><em>resist: </em>same
<p>
Same.
<p>
Does not change access levels.
   </td>
  </tr>
  <tr>
   <td>Track 
   </td>
   <td><em>resist: </em>Willpower + Firewall
<p>
If this IC hits and the host has 2+ marks on you, the host (and its owners) discover your real-world location.
   </td>
   <td><em>resist: </em>Willpower + Firewall
<p>
Same, but does not require any access levels / marks on the target. The location is revealed if it hits, regardless.
   </td>
  </tr>
</table>



### 


### Programs


#### Common programs


<table>
  <tr>
   <td>
   </td>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>Baby Monitor
   </td>
   <td><em>N/A; Baby Monitor is a “hacking  program” in 5e</em>
   </td>
   <td>Make user aware of their Overwatch Score at all times.[^30]
   </td>
  </tr>
  <tr>
   <td>Browse
   </td>
   <td>Cuts time for Matrix Search actions in half.
   </td>
   <td>Grants 1 Edge to be used on the Matrix Search roll.
   </td>
  </tr>
  <tr>
   <td>Configurator
   </td>
   <td>Store a deck config (ASDF allocation & program load.) Swap the entire config for a Free action, rather than a single pair of stats. 
   </td>
   <td>Same.
   </td>
  </tr>
  <tr>
   <td>Edit
   </td>
   <td>+2 to [Data Processing] limit for Edit tests.
   </td>
   <td>1 Edge on Edit File actions.
   </td>
  </tr>
  <tr>
   <td>Encryption
   </td>
   <td>+1 to Firewall.
   </td>
   <td>+2 dice pool when using Encrypt File actions.
   </td>
  </tr>
  <tr>
   <td>Signal Scrub
   </td>
   <td>Rating 2 noise reduction.
   </td>
   <td>Same.
   </td>
  </tr>
  <tr>
   <td>Toolbox
   </td>
   <td>+1 to Data Processing.
   </td>
   <td>Same.
   </td>
  </tr>
  <tr>
   <td>Virtual Machine
   </td>
   <td>+2 program slots, but whenever your persona takes Matrix damage, it incurs an additional box that cannot be resisted.
   </td>
   <td>Same.
   </td>
  </tr>
</table>



#### Hacking programs


<table>
  <tr>
   <td>
   </td>
   <td><strong>5e</strong>
   </td>
   <td><strong>6e</strong>
   </td>
  </tr>
  <tr>
   <td>Armor
   </td>
   <td>+2 dice to resist Matrix damage.
   </td>
   <td>+2 to matrix Defense Rating.
   </td>
  </tr>
  <tr>
   <td>Baby Monitor
   </td>
   <td>Always know your current Overwatch Score.
   </td>
   <td><em>N/A; Baby Monitor is a “common program” in 6e</em>
   </td>
  </tr>
  <tr>
   <td>Biofeedback
   </td>
   <td>When you attack a persona that’s backed by a biological entity (eg. a decker), the character takes Stun or Physical damage equal to the Matrix damage you do (depending on if they are in cold sim or hot sim.) 
<p>
 
<p>
Damage is resisted with Willpower + Firewall, as usual.
   </td>
   <td>Same.
<p>
Damage is resisted with Willpower alone, as usual.
   </td>
  </tr>
  <tr>
   <td>Biofeedback filter
   </td>
   <td>+2 dice pool to resist biofeedback damage.
   </td>
   <td>Allow Device Rating or Body to soak Matrix damage.
   </td>
  </tr>
  <tr>
   <td>Blackout
   </td>
   <td>As Biofeedback, but only ever causes Stun damage.
   </td>
   <td>Same.
   </td>
  </tr>
  <tr>
   <td>Decryption
   </td>
   <td>+1 to Attack.
   </td>
   <td>+2 dice on Crack File action.
   </td>
  </tr>
  <tr>
   <td>Defuse
   </td>
   <td>+4 dice pool modifier to resist damage from Data Bombs.
   </td>
   <td>Allow Device Rating or Body to soak damage from Data Bomb.
   </td>
  </tr>
  <tr>
   <td>Demolition
   </td>
   <td>+1 rating to any Data Bombs you create.
   </td>
   <td><em>N/A</em>
   </td>
  </tr>
  <tr>
   <td>Exploit
   </td>
   <td>+2 to Sleaze attribute when attempting Hack on the Fly.
   </td>
   <td>Reduce defense rating of hacking targets by 2.
   </td>
  </tr>
  <tr>
   <td>Fork
   </td>
   <td>Can perform a single Matrix action against two targets without splitting your dice pool - make one test, and each target defends separately against the test result.
   </td>
   <td>Same.
   </td>
  </tr>
  <tr>
   <td>Guard
   </td>
   <td>Reduces the extra damage you take from marks against you by 1 DV per mark.
   </td>
   <td><em>N/A</em>
   </td>
  </tr>
  <tr>
   <td>Hammer
   </td>
   <td>+2DV to all Matrix damage dealt.
   </td>
   <td><em>N/A</em>
   </td>
  </tr>
  <tr>
   <td>Lockdown
   </td>
   <td>When you cause Matrix damage, link-locks your target until you stop running Lockdown or they Jack Out.
   </td>
   <td>Same.
   </td>
  </tr>
  <tr>
   <td>Mugger
   </td>
   <td>Bonus Matrix damage from having a mark on your target is increased by 1 DV per mark.
   </td>
   <td><em>N/A</em>
   </td>
  </tr>
  <tr>
   <td>Overclock
   </td>
   <td><em>N/A</em>
   </td>
   <td>Add two dice to a Matrix action; one must be the wild die.
   </td>
  </tr>
  <tr>
   <td>Shell
   </td>
   <td>+1 dice pool to resist Matrix damage and biofeedback damage. Stacks with similar modifiers from other programs.
   </td>
   <td><em>N/A</em>
   </td>
  </tr>
  <tr>
   <td>Sneak
   </td>
   <td>+2 dice pool to resist Trace User.
<p>
If you are Converged on, GOD don’t get your physical location.
   </td>
   <td><em>N/A</em>
   </td>
  </tr>
  <tr>
   <td>Stealth
   </td>
   <td>+1 to Sleaze.
   </td>
   <td>Gain 1 Edge when doing the Hide action.
   </td>
  </tr>
  <tr>
   <td>Track/Trace
   </td>
   <td>+2 to Data processing when doing Trace User tests, or negate the +2 bonus from Sneak if your target is using that.
   </td>
   <td>Gain 1 Edge when doing the Trace Icon action.
   </td>
  </tr>
  <tr>
   <td>Wrapper
   </td>
   <td>Change icon of something to look like a different sort of icon entirely. Can be penetrated by Matrix Perception.
   </td>
   <td><em>N/A</em>
   </td>
  </tr>
</table>



### 


### Device specs (cyberdecks, cyberjacks)

SR5e:



<p id="gdcalert19" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image7.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert20">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image7.png "image_tooltip")


SR6e:

<p id="gdcalert20" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image8.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert21">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image8.png "image_tooltip")


<p id="gdcalert21" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image9.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert22">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image9.png "image_tooltip")







<!-- Footnotes themselves at the bottom. -->
## Notes

[^1]:
     Your delight is not guaranteed. 

[^2]:

     Snigger.

[^3]:
     Snigger. Again.

[^4]:

     This showed up in 5e as an optional rule in Kill Code.

[^5]:

     “PAN's were not originally meant to be as restrictive on number of devices as they ended up (if errata does not get approved to change it a good house rule would be to make it Device Rating x3 for max number of devices)” [source](https://forums.shadowruntabletop.com/index.php?topic=30059.msg524805;topicseen#msg524805)

[^6]:

     This is a housrule; in 6e RAW, direct connection doesn’t grant the firewall bypass.

[^7]:
     I have little love for the extended test mechanic in general. It’s good in theory, but it simply takes too long to roll 50-100 dice and count the hits.

[^8]:

     This is the rule in 5e, also, as of Kill Code (see page 32.)

[^9]:
      Confirmed by Banshee (Matrix rules author) as his intention [here](https://forums.shadowruntabletop.com/index.php?topic=30891.msg533892#msg533892).

[^10]:

     RAW is one minute; [Banshee originally intended it to be an hour](https://forums.shadowruntabletop.com/index.php?topic=30918.msg534063#msg534063). I prefer his version.

[^11]:

     Note I have removed the word “extended” here -- see the note below.

[^12]:
<p>
     6e RAW is “unless major mistakes are made”, I have changed this to “glitch” which is what the German CRB uses.

[^13]:
<p>
     This is a deviation from SR6e RAW, which imposes a -2 dice pool penalty plus gives the defender +4 Defence Rating on the test (which makes them more likely to earn Edge.) These mechanics don’t work in 5e unless you backport the entire Edge system (which I don’t want to do.) I made up this -6/-4.

[^14]:
<p>
     This is my houserule, not a 6e thing.

[^15]:
<p>
     See <a href="https://forums.shadowruntabletop.com/index.php?topic=30394.0">this thread</a> for details.

[^16]:
<p>
     see Banshee’s posts about Probe’s nature as an extended test <a href="https://forums.shadowruntabletop.com/index.php?topic=30383.msg528689#msg528689">here</a>.

[^17]:
<p>
     The 6e CRB lists this as a legal action, but it uses the Cracking skill so I am going to decide it is illegal.

[^18]:
<p>
     The 6e CRB doesn’t seem to tell you when you’d roll Intuition + Sleaze for this action, though. Unattended devices maybe?

[^19]:
<p>
     It’s not clear exactly what you need Admin access to. I guess it’s if you want to use this to check someone else’s Overwatch Score…?

[^20]:
<p>
     This sounds to me like Matrix Perception in 6e is intended to always be opposed.

[^21]:
<p>
     It’s not clear to me when you use the second resistance roll.

[^22]:
<p>
     It’s not clear to me when you use the second resistance roll.

[^23]:
<p>
     I would suggest renaming this to “Metadata Search”. If only because of the mode where you can use it to search for files when you don’t know the hash...

[^24]:
<p>
     Bit weird, that one. It’s not like you can do Full Matrix defence to anyone else.

[^25]:
<p>
     It’s weird this doesn’t last the rest of the turn. The meatspace version of Full Defense does, in both 5e and 6e. Perhaps a mistake.

[^26]:
<p>
     Wait, what?!

[^27]:
<p>
     Hmm. So can I hack a security spider’s deck, get Admin access, then turn it into a jammer to knock them offline? ;)

[^28]:
<p>
     I <em>think</em> this is consistent with SR6e RAW, although it’s a little convoluted here so I might be accidentally houseruling. 

[^29]:
<p>
     However, this was <a href="https://forums.shadowruntabletop.com/index.php?topic=30059.msg524805#msg524805">refuted</a> by the lead author of the Matrix rules section. His intention was to have a much higher restriction, and for each member of a runner team to have their own PAN, then put that under the umbrella of the decker’s PAN.

[^30]:
<p>
     This sounds to me like Matrix Perception in 6e is intended to always be opposed.
