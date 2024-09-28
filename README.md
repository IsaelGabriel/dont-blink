# dont-blink

| Engine | Genre  | Platform |
|--------|--------|----------|
| Unity  | Horror |    PC    |

# Introduction

This is a horror game project, inspired by the [Wheeping Angels](https://tardis.fandom.com/wiki/Weeping_Angel), from the british TV show [Doctor Who](https://pt.wikipedia.org/wiki/Doctor_Who).

This project serves as a challenge both in programming and game design, as the main concept is to create a 2D Top-Down horror game with an enemy that doesn't move until out of sight.

## Wheeping Angels (from [Doctor Who](https://pt.wikipedia.org/wiki/Doctor_Who))

![Wheeping Angel](https://static.wikia.nocookie.net/tardis/images/b/be/Series5weepingangels.jpg/revision/latest?cb=20240127230056)

> "The Weeping Angels were an incredibly powerful species of quantum-locked humanoids, so called because their unique nature necessitated that they often covered their faces with their hands to prevent trapping each other in petrified form for eternity by looking at one another. They were known for being "kind" murderous psychopaths, eradicating their victims "mercifully" by dropping them into the past and letting them live out their full lives, just in a different time period. This, in turn, allowed them to live off the remaining time energy of the victim's life. [...]" - Source: [Tardis Wiki](https://tardis.fandom.com/wiki/Weeping_Angel).

Having these beings as the main villain of a 3D game is fairly easy to envision, but the fun lies in making a 2D game with them. This decision, of course, creates a few game design questions, such as:

> How to limit a player vision and get away with it in a 2D world?

> How to portray the horror of having a Wheeping Angel in your face as you turn in 2D?

# Gameplay

The core gameplay loop consists on having the player explore their setting and avoid getting caught by enemies in the way.

The player character has their movement controled via keyboard or joystick, in any angle.

The player view is cone-shaped and points to the mouse or joystick direction. Everything outside that cone is not visible to the player.

## Enemies

This game's enemies only move when they are not in the player character sight. If they reach the player while not visible, the game is over.

During the "unseen" state of the enemies, they move by turning to the player's direction and moving in a straight line to it. They accelerate after starting movement and only come to a full stop if seen by the player.
