# 🧱 Breakout Game

A faithful recreation of the 1980s arcade classic "Breakout," built entirely in Python using the Turtle graphics library.

## 📝 Project Overview

This project brings the nostalgia of retro arcade gaming to your desktop. Players control a sliding paddle to bounce a ball into a wall of bricks, destroying them one by one. It features a complete game loop with collision physics, score tracking, and win/loss conditions, all running natively in Python without needing external game engines.

## 🚀 Features

- **Classic Arcade Action**: Authentic paddle-and-ball mechanics with four colorful rows of bricks.
- **Smooth Controls**: Responsive keyboard inputs for precise paddle movement.
- **Scoring System**: Real-time score tracking (10 points per brick) with a high-contrast HUD.
- **Physics Engine**: Accurate collision detection for walls, the paddle, and individual bricks.
- **Game States**: Distinct "YOU WIN!" and "GAME OVER" screens.
- **Instant Restart**: Clickable on-screen reset button (↻) to start a new game immediately without closing the app.
- **Zero Dependencies**: Runs on the standard library's `turtle` module—no `pip install` required.

## 💻 Installation & Usage

### Prerequisites
- Python 3.6+
- (Note: The `turtle` module is included with standard Python installations on Windows and macOS. On some Linux distributions, you may need to install `python3-tk`.)

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/DavitEgoian/Breakout-Game.git
   cd Breakout-Game
   ```

2. **Run the game**
   ```bash
   python main.py
   ```

3. **Controls**
   - **Left Arrow / 'A'**: Move Paddle Left
   - **Right Arrow / 'D'**: Move Paddle Right
   - **Reset Icon (↻)**: Click to restart the game

## 📂 Project Structure

```text
Breakout-Game/
├── main.py         # Core game loop, screen setup, and input handling
├── ball.py         # Ball logic: handles movement speed and bounce physics
├── paddle.py       # Paddle logic: handles player movement and boundary checks
├── brick.py        # Brick logic: manages grid generation and destruction
└── scoreboard.py   # UI logic: handles score updates and text rendering
```

## ⚙️ Customization

The object-oriented design makes it easy to mod the game:

- **Difficulty**: Increase ball speed by modifying the `move_speed` attribute in `ball.py`.
- **Level Design**: Change colors or add more rows by editing the `COLORS` list and loops in `main.py`.
- **Paddle Size**: Adjust the `shapesize` stretch factor in `paddle.py` to make the game easier or harder.
- **Screen Resolution**: Tweak the `screen.setup()` parameters in `main.py` for different window sizes.

## 📄 License

This project is open source and available for personal and educational use.
