# CS310H Unreal Engine HW1 Project

## Student Information
* **Name:** Kaitlyn Jones
* **Course:** CS310H

---

## Deliverables
* **GitHub Repository:** https://github.com/KatieJones13/CS310H
* **Video Demonstration:** https://youtu.be/ulvx-DYmek4

---

## Features & Implementation

### 1. Level Design & Navigation
* **Main Menu (`Level_Menu`):** Interactive UI widget featuring **Start Game** and **Quit Game** buttons with proper mouse cursor control and UI-only input mode.
* **Level 1 (`Level_One`):** First gameplay level featuring static geometry, static materials, 3 targets, 3 hazards, and pickups. 
* **Level 2 (`Level_Two`):** Second gameplay level with a unique layout, static geometry, 3 targets, 3 hazards, and pickups.

### 2. Targets & Progression Tracking
* Each non-menu level contains at least 3 target actors (`BP_Target`) with an initial health pool of **100**.
* Targets take damage when hit by player projectiles, destroying themselves when health drops to $\le 0$.
* Automatically queries remaining target actors using `Get All Actors of Class` upon target destruction; once all targets are cleared, the game automatically transitions to the next level (Level 1 $\rightarrow$ Level 2 $\rightarrow$ Main Menu).


