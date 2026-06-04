---
layout: post
title: Designing a sump from first principles
tags:
  - sump
  - filtration
---

<div class="message-info">Under construction.
</div>

### Overview

In my [fishroom in a rack build](https://tmaquaponics.github.io/2026/04/03/Building-RAS.html){:target="_blank"}, the cornerstone piece of the design is the sump. It serves the role of a settling chamber and a central filtration system. In this post, I will discuss the different designs I drew and consider the pros and cons of each model. Each design is imagined from first principles. Finally, I will document how I built the design I went with and the difficulties I encountered. Though the design I chose is simple, it serves its purpose quite well and offers me plenty of space and possibilities for upgrades and modifications.

### Introduction

A sump is a central filtration system where water is filtered from chamber to chamber. Usually, a it contains at least 3 chambers. 

The first chamber is for mechanical filtration. Most often this is done using filter floss or filter socks. Beneath that filter floss are coarse sponges that act as mechanical and biological filtration. The role of the first chamber is to protect the static media and equipment from particles in the water. 

The second chamber usually contains static media or moving biopellets. The role of this chamber is purely biological. 

The third chamber is for equipment and water conditioning. This last chamber hosts the return pump, heating elements and maybe some crushed corals for pH.

The number one benefit of a sump is the huge filtration capacity it brings compared to canister filters. The downside is that you have to do a lot of plumbing. If that plumbing is not done right, you could end up with leaks and water accidents. For our specific purpose, the tanks in the rack overflow to the sump by gravity and not by siphon, so there's no risk of the sump overflowing (when the main pump stops, the circuit stops instantly and no water is purring in the sump anymore).

In my ras setup, I decided to implement a central filtration system in the form of a &80 Liters sump. Since space is of utmost importance in a breeding setup, the sump needed to be versatile enough to be converted into a grow-out tank while serving as a central filtration most of the time. Essentially, I needed the sump to be demountable without requiring me to take apart the glass. It also needed to be a settling chamber where water can be drawn without requiring me to constantly do top-offs.

Let's first lay out the requirements of the sump to have something we can ponder against later on:

- Should be a central filtration system.
- Can be converted into a grow-out tank.
- Serves as a reservoir of water: the volume of evaporated water must be taken out from the sump. 
- Easy to maintain and clean.
- Allow modifications and upgrades.
- Achieve a full filtration cycle.

From these requirements I sketched out the following designs :

**Design 1: The sump has three equal chambers**

In this design I considered the sump to be composed of three chambers of 60 liters each. Each chamber is depth-wise to the sump with clear access for me. Each dividing baffle has three holes for the water to circulate from chamber to chamber. The gutter pours in water in the front of the first chamber. Water circulates to the back of the first chamber passing through different filtration media, then enters the second chamber from the side through the three holes in the first baffle. In the second chamber, water flows from the back of the chamber to the front passing through the moving biopellets to enter the third chamber through the three holes on the side of the second baffle. In that last chamber, water flows from the front to the back of chamber and finally to the return pump. Two heaters are placed in that last chamber.

Pretty simple design, easy to clean and operate. 

<ins>Negative aspects:</ins>
- Can't be converted to a grow-out tank.
- Upgrades only possible in the last chamber.
- Does not achieve a full filtration cycle (The nitrates and phosphates are not removed).

**Design 2: The sump is just one big chamber**

In this design the 180 Liters aquarium is left as is. The only filtration are moving biopellets that fill up the entire sump. Filter floss is placed at the end of the in-flow gutter to catch particles before they enter the sump.

This is just a big MBBR. No baffles, easy access to the entire sump, plenty of room for upgrades and equipment.

<ins>Negative aspects:</ins>
- If converted to a grow-out tank we loose the filtration.
- Does not achieve a full filtration cycle (The nitrates and phosphates are not removed).
- Need to often clean the filter floss.

**Design 3: Elaborate sump**

In this design, the sump has four chambers. The first chamber if 15 by 60 cm. This first chamber is further divided into 4 compartments. The First three hold moving sand filter while the last compartment at the front glass remains empty. On the sides of that last compartment are three holes for water to pass to the second chamber.

The second chamber is 45 by 60 cm and has a deep sand bed of 12 to 15 cm. From this chamber, water passes through three holes on the back side of the baffle to the third chamber where reside moving biopellets. Water then passes to the last chamber, where the return pump and a heater are placed. The moving sand filter is run by an additional pump placed in the last chamber.

This design does not hold static media at all but the combined moving sand and biopellets are significantly more effective. The role of the moving sand filter is more than filtration. Moving sand grains break particulates from the tanks into finer sized particles that feed the deep sand bed and provide a carbon source for the anaerobic bacteria. Thanks to the deep sand bed, this design can potentially achieve a full cycle and get rid or at least reduce nitrates.

<ins>Negative aspects:</ins>
- Can't be converted to a grow-out tank.
- Costs more to run the additional pump.
- No room for upgrades.
- Difficulty in getting rid of the sand if I drop the sand filtration feature (I would need to empty the sump and take it out from the rack).

**Design 4: Convertible sump**

The sump has three chambers. The first one is 60 by 60 cm and will host an MBBR. The remaining space in the 180 Liters aquarium is divided in two. A small 20 by 30 cm chamber where are placed filter floss, sponge mats and static media, and a big chamber of 40 by 30 cm where are placed heaters and the return pump. Water flows into the small chamber through four holes on the side, then passes underneath the divider baffle to the big chamber, and finally flows to the return pump.

The first divider has a bulkhead on the side to the last chamber for overflow. When the static media in the second chamber is clogged, water starts rising in the MBBR compartment and overflows into the last chamber bypassing the second chamber. When the water starts overflowing, it means it is time to clean the filter floss and the sponge mats in the second chamber.

This design is simple, holds static media that is easy to access and clean and has an MBBR that can be converted to a grow-out tank. Similarly to design 2, and to protect the MBBR, an additional filter floss is put at the end of the gutter to catch particles from the tanks. Unlike design 3, it uses only one pump to return water to the tanks.

<ins>Negative aspects:</ins>
- Does not achieve a full filtration cycle (The nitrates and phosphates are not removed).
- Requires cleaning the filter floss from time to time.

**Design 5: Good enough sump**

This design is similar to design 4 but has an additional chamber of 15 by 60 cm where the gutter pours in water. This chamber is divided into 4 compartments where water flows beneath or above each baffle to reach the second chamber. The second chamber, now of size 45 by 60 cm, holds the MBBR.

<ins>Negative aspects:</ins>
- Does not achieve a full filtration cycle (The nitrates and phosphates are not removed).
- Like in design 3, it is difficult to access the static media if the sides of the rack are out of reach.

**Design 6: Regular sump**

In this design the sump has 4 chambers. The chambers are separated depth-wise by baffles where water goes beneath or above each baffle. The first chamber is 15 by 60 cm, it holds filter floss and sponge mats. The second chamber is 15 by 60 cm and holds the static media. The third chamber holds the moving biopellets and is 30 by 60 cm. The last chamber is 30 by 60 cm and holds the heaters and the return pump.

This design is simple and gives clear access to all the chambers from the front of the rack.

<ins>Negative aspects:</ins>
- Does not achieve a full filtration cycle (The nitrates and phosphates are not removed).
- No room for upgrades except in the last chamber.
- Can't be converted into a grow-out tank.

**Design 7: Divider sump**

This design is similar to design 2 except there are two dividers held by suction cups. This means I can resize the MBBR chamber as I want, create a grow-out space of variable size and still have a 180 L tank in case I want to convert the sump into a settling or full breeding/grow-out tank. This design is the most versatile since it can be converted at any time into any other design.

<ins>Negative aspects:</ins>
- Does not achieve a full filtration cycle (The nitrates and phosphates are not removed).
- Need to often clean the filter floss at the end of the gutter.

### Final design

