---
title: "Mirror World"
layout: post
image: https://mholtkamp.github.io/assets/images/MirrorWorld2.PNG
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: "Game Jam submission to the December 2015 Epic Game Jam."
category: project
author: Martin Holtkamp
externalLink: false
---

## Info

**Game Name:** Mirror World  
**Platform:** Windows  
**Programming Language:** C++  
**Engine:** Unreal Engine  
**Genre:** Sidescrolling Platformer  
**Team Size:** 2  

---

## Teammates 

* Dustin LaMontagne

---

## Links

[Download Windows 32-bit](https://drive.google.com/open?id=0Bz6zRTgs-_fBdklDUnpVSEJJNXM)  
[Source Code](https://github.com/mholtkamp/mirror)

---

## Gameplay Video

<iframe width="560" height="315" src="https://www.youtube.com/embed/7Xs0X6cdi68" frameborder="0" allowfullscreen></iframe>

---

## Comments

Dustin and I had so much fun with the previous month's game jam, so we decided participate in December's game also. The theme for this month was "The Beginning is the End". Unlike our last game jam, we came up with a rather unique concept for this jam. The player would have to traverse through a level and then pass through a mirror that would replicate the same level that was just traversed, except it would be flipped like a mirror image. Thus, when the player reaches the end of the game, they would be at the mirrored version of the beginning of the game. 

One of the challenges that we spent some significant time on was getting the collision right. We didn't want to use Unreal's physics system, as that would be overkill for a simple platformer like this. We ended up using MovementComponent's SlideAlongSurface() method and some sweeping using AActor::SetActorLocation() to get our platforming the way we wanted it. The solutions are rather simple, but it took us time to get to there.

Some of the feedback we got on the game included:  
* **"It's frustrating not being able to control my jump height."** - A valid complaint. If we had time we probably would have added this little mechanic, but it is definitely more challenging when you cannot control your jump height.  
* **"The difficulty curve goes from 0 to 100 real fast."** - We would probably fix this by adding more checkpoints to the mirrored world and also by reworking the third enemy encounter which is way too challenging.  
* **"The music hurts my eyes."** - This comment was referring to the music played in the mirrored world, which is the same background music played in the first half... just reveresed. We would have probably fixed this by composing a detuned, or slower version of the original song instead of playing it backwards.  
