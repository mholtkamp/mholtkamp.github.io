---
title: "PCG the TCG"
layout: post
image: https://mholtkamp.github.io/assets/images/Ascent1.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: "An online competitive playing card game for Android."
category: project
author: Martin Holtkamp
externalLink: false
---

## Info

**Game Name:** PCG the TCG  
**Platform:** Android  
**Programming Language:** Java  
**Engine:** LibGDX  
**Genre:** Card Game  
**Team Size:** 1  

---

## How To Play

If hosting, select the "Host" button under the LAN column. If connecting, select the "Connect" button under the LAN column and then type in the host's IP Address. A player will randomly be chosen to go first. If the "End Turn" button is green on your screen, that means it is currently your turn. Refer to the "How To Play" page within the app to learn the gameplay cycle and to see the special abilities of each card.

---

## Links

[APK Download for Android 4.1+](https://drive.google.com/open?id=0Bz6zRTgs-_fBY2llYjNvWUZxU0k)  
[Source Code](https://github.com/mholtkamp/pcgtcg)

---

## Comments

PCG the TCG, which stands for "Playing Cards Game the Trading Card Game" is a casual card game that my friends and I used to play back in high school. The game played similarly to any popular trading card game (Yugioh, Magic, Pokemon, etc) but it only required a normal 52-card deck of playing cards. We normally played PCG the TCG in instances where wanted to play Yugioh, but didn't have our decks with us. The ruleset was developed by my friend Anshul and was slowly modified over time to balance cards that were outrageously overpowered. I created the android adaptation of PCG the TCG so that I could play with my friends online, and also to get some experience with networking.

The game was built originally for LAN only with a rather funky non-authoritative networking model. Messages were sent as character strings containing words like "SUMMON" "KILL" DAMAGE" with a variable number of arguments delimited by periods. This was the most obvious way of encoding messages at the time, but in hindsight, I should have used message IDs and serialized the parameters into binary format, which is how I now prefer to implement networked multiplayer protocols. There's no real reason to parse strings besides the fact that it makes packets more readable when using a TCP sniffer. Oh, and also I used TCP, which was definitely the most approriate choice for a turn based card game.

Eventually I decided to make a "master server" which would allow players to play against each other online, even through a NAT'd network. The same non-authoritative networking architecture was still in place, but there was now a lobby browser where players could see open games (and also games that were already in progress). I learned a lot through this experience, specifically with server configuration and linux. My VPS subscription has expired, however, so the online lobby system no longer works. LAN is the only option for playing.