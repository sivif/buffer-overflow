# 📦 Buffer Overflow

[![Godot Engine](https://img.shields.io/badge/Engine-Godot%204.x-EE730A?logo=godot-engine&logoColor=white&style=flat-square)](https://godotengine.org)
[![Platform](https://img.shields.io/badge/Platform-Web%20/%20PC-blue?style=flat-square)]()
[![Live Game](https://img.shields.io/badge/Play%20Now-GitHub%20Pages-brightgreen?style=flat-square)](https://sivif.github.io/buffer-overflow/)

A frantic, high-energy arcade sorting game where you play as **ACES-chan**, a factory automation robot tasked with managing a rapidly accelerating electronics assembly line. Sort hardware, software, and hazardous e-waste into their proper dynamic hoppers before the system suffers a catastrophic buffer overflow!

🎯 **Play the live web build directly in your browser:** [sivif.github.io/buffer-overflow/](https://sivif.github.io/buffer-overflow/)

---

## 🕹️ Gameplay & Core Concept

Items sweep across the factory floor via automated conveyor belts running along the top and bottom of the screen. Your job is to intercept these items, identify their categories, and deposit them into the central dynamic hoppers. 

As time ticks down, the assembly line continuously moves faster. Make too many mistakes, and your penalty meter will max out, destabilizing the sector and sending the engine into a scrambled glitch state!

---

## ⚙️ Game Mechanics

### 🛠️ Sorting Manifest
* **🔵 HARDWARE:** Circuit boards, microchips, and processors ➔ Deposit into the **Blue Hopper**.
* **🟢 SOFTWARE:** CDs, floppy disks, and data storage ➔ Deposit into the **Green Hopper**.
* **🔴 E-WASTE:** Batteries, old monitors, and power cells ➔ Deposit into the **Red Hopper**.

### 🔥 Overdrive: Fever Mode
Achieve **10 consecutive correct sorts** without missing an item or mis-sorting to activate **Fever Mode**!
* **Omni-Sorting:** The category filters drop completely—throw *any* item into *any* hopper for a valid match.
* **Double Tally:** Score values are doubled (**+20 PTS** per item).
* **Maximum Throughput:** The conveyor lines accelerate to absolute peak velocity for extreme scoring potential.

### ❄️ System Modifiers (Power-ups)
Keep an eye out for special modular items gliding down the belts:
* **Freeze (❄️):** Temporarily halts conveyor movement entirely, allowing you to catch up and clear backlogs.
* **Overclock (🔥):** Overcharges ACES-chan's internal actuators, granting a massive movement velocity boost.

### ⚠️ System Overload (Glitch State)
If your penalty meter reaches **100%**, a severe core error triggers. The screen distorts, and your directional movement inputs are **randomly inverted** for 6 seconds. Survive the chaos to reset your penalty stabilizers!

---

## 🎮 Controls

| Action | Keyboard Bindings | Gamepad / Controller |
| :--- | :--- | :--- |
| **Move ACES-chan** | `W, A, S, D` or `Arrow Keys` 
| **Grab / Deposit Item** | `J` 
| **Turbo Dash** | `K` | 

## 🏗️ Technical Development Profile

* **Engine:** Godot Engine 4.x (`@tool` script optimized for viewport asset rendering).
* **Language:** GDScript (Asynchronous async/await tween loops, delta-based power-up state tracking pipelines).
* **Architecture:** Decentralized event/signal pipeline utilizing a centralized `Global.gd` core manager script tracking scores, combo states, power-up timers, and match state variables.

---
*Developed by [@sivif](https://github.com/sivif).*
