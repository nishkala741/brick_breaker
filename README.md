# 🧱 Brick Breaker Game

A classic Brick Breaker arcade game built with **Python** and **Object-Oriented Programming (OOP)** principles using the **Pygame** library. Features real-time ball physics, collision detection, paddle controls, and a complete scoring system.

---

## 📸 Demo

> *Add a gameplay screenshot or GIF here*

---

## 🚀 Features

- 🎮 **Smooth Paddle Controls** — Responsive keyboard-based paddle movement
- ⚽ **Real-Time Ball Physics** — Dynamic ball movement with angle-based reflections
- 💥 **Collision Detection** — Accurate ball-brick and ball-paddle collision logic
- 🧱 **Brick Grid System** — Structured brick layout with configurable rows and columns
- 🏆 **Scoring System** — Points awarded on every brick destroyed
- 🎯 **Win / Lose Conditions** — Clear end-game states with restart support
- 🔄 **Efficient Game Loop** — Frame-rate-controlled loop using Pygame's clock system

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python 3.x | Core programming language |
| Pygame | Game rendering and event handling |
| OOP (Classes) | Modular design for game entities |

---

## 🗂️ Project Structure

```
brick-breaker-game/
│
├── main.py               # Entry point — initializes and runs the game loop
├── ball.py               # Ball class — movement, speed, and collision logic
├── paddle.py             # Paddle class — player-controlled movement
├── brick.py              # Brick class — individual brick properties and state
├── game.py               # Game class — overall state, scoring, win/lose logic
├── constants.py          # Screen dimensions, colors, speed settings
├── assets/               # (Optional) Sounds, fonts, images
└── README.md
```

---

## 🧩 OOP Design

| Class | Responsibility |
|---|---|
| `Ball` | Handles position, velocity, and bounce logic |
| `Paddle` | Manages horizontal movement and boundary limits |
| `Brick` | Represents each brick's position, color, and hit state |
| `Game` | Orchestrates game state, score, level, and loop |

---

## ⚙️ Installation & Setup

### Prerequisites

- Python 3.7+
- pip

### Steps

```bash
# 1. Clone the repository
git clone https://github.com/your-username/brick-breaker-game.git
cd brick-breaker-game

# 2. Install dependencies
pip install pygame

# 3. Run the game
python main.py
```

---

## 🎮 Controls

| Key | Action |
|---|---|
| `←` Arrow | Move paddle left |
| `→` Arrow | Move paddle right |
| `Space` | Launch ball / Restart |
| `Q` or `Esc` | Quit the game |

---

## 📐 Game Logic Overview

```
Game Loop
│
├── Handle Events (keypress, quit)
├── Update
│   ├── Move ball (velocity-based)
│   ├── Check wall collisions (left, right, top)
│   ├── Check paddle collision → reverse Y velocity
│   ├── Check brick collisions → destroy brick, update score
│   └── Check win/lose condition
└── Render
    ├── Draw background
    ├── Draw bricks
    ├── Draw paddle
    ├── Draw ball
    └── Display score / HUD
```

---

## 🔮 Future Enhancements

- [ ] Multiple difficulty levels (speed scaling)
- [ ] Power-ups (multi-ball, wide paddle, laser)
- [ ] Sound effects and background music
- [ ] High score leaderboard (local storage)
- [ ] Level progression with new brick patterns

---


<p align="center">Built with ❤️ using Python & Pygame</p>
