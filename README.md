# 🐍 Snake and Ladder Game

A simple two-player **Snake and Ladder** game built in Python, played in the terminal with a visual board image shown at the start.

## 📋 About

This is a classic implementation of the Snake and Ladder board game for two players. Players take turns rolling a dice, moving along a 100-square board, climbing ladders, and avoiding snake bites — first to reach square 100 wins!

## 📁 Files

| File | Description |
|------|--------------|
| `snake.py` | Main game logic and gameplay loop |
| `board_image.png` | Image of the game board, displayed at the start of the game |
| `user_config.yml` | Configuration file |

## 🛠️ Requirements

- Python 3.x
- [Pillow](https://pypi.org/project/Pillow/) (for displaying the board image)

Install the dependency with:

```bash
pip install Pillow
```

## ▶️ How to Run

1. Clone the repository:
```bash
   git clone https://github.com/Gunalm232/SNAKE-LADDER.git
   cd SNAKE-LADDER
```
2. Make sure `board_image.png` is in the same folder as `snake.py`.
3. Run the game:
```bash
   python snake.py
```

## 🎮 How to Play

1. When the game starts, the board image opens for reference.
2. Enter the names of Player 1 and Player 2.
3. Players take turns:
   - Press `1` to roll the dice and continue.
   - Press `0` to exit the game.
4. A dice value (1–6) is randomly generated and added to the player's score.
5. **Ladders** move you up to a higher square. **Snakes** send you back down.
6. The first player to reach square **100** wins the game!

### 🪜 Ladder positions
| From | To |
|------|----|
| 1 | 38 |
| 4 | 14 |
| 8 | 30 |
| 21 | 42 |
| 28 | 74 |
| 50 | 67 |
| 71 | 92 |
| 88 | 99 |

### 🐍 Snake positions
| From | To |
|------|----|
| 32 | 10 |
| 34 | 6 |
| 48 | 26 |
| 62 | 18 |
| 88 | 89 |
| 95 | 56 |
| 97 | 78 |

## ⚠️ Known Issues

- In the current `play()` logic, Player 2's ladder/snake checks reference `pp1` instead of `pp2`, which affects Player 2's score calculation. This may need a fix in a future update.

## 📄 License

No license specified yet — consider adding one (e.g., MIT) if you plan to share or accept contributions.
