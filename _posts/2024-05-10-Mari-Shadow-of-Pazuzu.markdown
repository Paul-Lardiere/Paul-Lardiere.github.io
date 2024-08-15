---
layout: post
title:  Mari Shadows of Pazuzu
date:   2024-05-10 15:01:35 +0300
image:  Mari.png
tags:   Third-Person PvE Roguelike
---
Mari: Shadows of Pazuzu is a cooperative roguelike in which you team up with up to 3 friends to advance through the city of Mari and gain powerful spells and upgrades to defeat your enemies. Combine powerful abilities with your friends to create even more powerful spells and save the city!

***
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/ynAOt49ZM-E?si=gMcPnnuyp8IRYoSn&rel=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
---
This game was developed on Unreal engine 5, mostly in C++, we used The Gameplay ability system (GAS) for spells, AI attacks, effects, health etc. 
Game developed as a School project at DDJV, Université de Sherbrooke, Longueuil.

* Antoine Girard
* Gras Yael
* Larsonneur Ugo
* Wyss Matthias
* Sénéchal Erwan
* Richard Paul
* Lardiere Paul

I mostly worked on building the AI systems and behavior, integrating them with the Gameplay Ability System (GAS) for handling attacks and health management, as well as ensuring proper replication.

***
## Spells

Combat revolves around spells: players can gain a new spell with each room cleared or level up an existing one. Spells can be cast individually, but they become incredibly powerful when combined. For example, if one player summons a tornado and another casts a fireball into it, the result is a devastating fire tornado. You can even combine more than two spells for even greater effects!

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/CCl7MC0zK88?si=vsjv_ysciPU0oYVZ&rel=0&amp;controls=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin"></iframe>

***
### AI

Enemies are grouped into squads and will patrol the area when they don't have a player in sight.
  <img src="{{site.baseurl}}/images/Golem.gif" alt="">


AI was a major focus for this project, given that it's a PvE game. We designed our architecture to be highly scalable, allowing us to easily create a variety of squads. Each squad is composed of subsquads, which in turn are made up of individual enemies. Squads, subsquads, and individual enemies each have a controller that can assign simple commands like "ATTACK," "MOVE," "PATROL," etc., to a behavior tree.

Individuals handle perception, relaying their information to the squad. Decisions are made at the squad level, which then issues orders to the subsquads. The subsquads, in turn, command the individuals. The same order can produce different outcomes depending on the behavior tree associated with it, enabling us to create squads of mixed individuals that work together sharing the squad's information. This design allow us to reuse a lot of small behavior trees for multiple enemies.

---

We put significant effort into refining our group movement mechanics, ensuring that our squads move in a logical and realistic manner.
<img src="{{site.baseurl}}/images/Orc.gif" alt="">

---

Our melee enemies are designed to surround the player(s) and launch coordinated attacks. 
<img src="{{site.baseurl}}/images/Surround.gif" alt="">

--- 

They also strategically position themselves to avoid being hit by their own casters' attacks.
<img src="{{site.baseurl}}/images/Avoiding.gif" alt="">

--- 

Finally, our game features four bosses, each utilizing a more straightforward AI implemented through Unreal Engine's Behavior Trees. These bosses are designed around patterns of powerful attacks, forcing players to dodge and use defensive spells.
<img src="{{site.baseurl}}/images/Pazuzu.gif" alt="">

***

### Data driven

Given the vast number of spells, upgrades, and enemies in the game, we concentrated on making our structure highly scalable and data-driven. All spell synergies, player stats, and enemy stats are modifiable through .csv files that can be directly imported into UE5. This system allows for easy adjustments to any spell statistics, synergy behaviors, or enemy stats, providing flexibility and efficiency in tweaking game mechanics.

***

### Debug Tools

Debugging our spell and AI systems was crucial to the development of this game, so we created a number of debugging tools to help us, here are just a few:

##### Spell visual debug tool :

This tool allows us to view who cast the spell, the spell level and any effects added to the spell.
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/P6ViERZS-7g?si=1LzaSck8CBqerLZI&rel=0" title="Spell debug tool" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/xFaRjyye4ak?si=CaD4NY6Jg7Pd69Ty&rel=0" title="Spell debug tool" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

