---
title: "Whirly Dragons"
layout: post
image: https://mholtkamp.github.io/assets/images/WhirlyDragons1.PNG
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: "An online multiplayer sports game built for the HTC Vive."
category: project
author: Martin Holtkamp
externalLink: false
---

## Info

**Game Name:** Whirly Dragons  
**Platform:** Windows  
**Programming Language:** C++  
**Engine:** Unreal Engine  
**Genre:** Sports  
**Team Size:** 6  

---

## Teammates 

* Michael Reckoff (Design, Production)
* Michael Vogel (Art)
* Boo Roseman (Art)
* Kay Ghering (Art)
* Travis Fort (Programming)

---

## Links

[Download Windows 32-bit](https://drive.google.com/open?id=0Bz6zRTgs-_fBeDBjTklFT3doNWs)

---


## How To Play

At the menu, use the arrow keys to select whether you would like to host a new game, or connect to a game. If connecting to an open game, the host's IP address can be entered using the buttons on the bottom of the screen.

As the host, press the "P" key to begin the game after all players have connected.

In-game Controls:
**Space Bar:** Fire a fireball. If the fireball hits the ball carrier, they will be forced to drop the ball.
**Left Ctrl:** Stop/Start flying.
**A/D:** Adjust heading of dragon.
**W/S:** Adjust pitch of dragon.
**F:** Pick up/throw the ball.

---

## Comments

Whirly Dragons is a game I worked on in the Rapid Prototyping class at FIEA with a team of 5 others. The requirements for our game were that it needed to use some piece of new technology, so we decided to make a VR game using the HTC Vive.

The idea behind the game was to recreate the feeling of playing "Whirly Ball", a fun sports game played on vehicles similar to bumper cars, but on dragons instead. Ideally the game would be played either 3-on-3 or 4-on-4 with every player using a Vive. Since we only had 2 vives at FIEA, we made the game playable with mouse and keyboard controls as well.

I was in charge of implementing the networking for the game. It was my first time doing networking in Unreal, and I was very happy working with Unreal's networking system. In past networked games, I would use a messaging protocol, but Unreal takes care of all that for you by providing a Replication framework where you can notify what actors to replicate across the network. With replicated variables, server RPCs, and NetMulticast RPCs, implementing gameplay was relatively painless.

This game also sold me on VR. After flying on the dragon myself and passing the ball to my teammates, I could see myself playing similar games for hours on end. The immersion is just incredible.