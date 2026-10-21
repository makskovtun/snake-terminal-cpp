# 🐍 Terminal Snake

Classic **Snake** game that runs right in your terminal — written in **C++** as a university coursework project.

![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white)
![macOS](https://img.shields.io/badge/macOS-000000?style=flat&logo=apple&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)

```
######################
#                    #
#    ooooO           #
#                    #
#             F      #
#                    #
######################
Score: 40
```

## ✨ Features

- Real-time controls — keys are read instantly, no Enter needed (`termios` + non-blocking input)
- Wrap-around walls — the snake passes through the borders
- Growing tail and self-collision detection
- Score counter

## 🎮 Controls

| Key | Action |
|:---:|--------|
| `W` | Move up |
| `A` | Move left |
| `S` | Move down |
| `D` | Move right |
| `X` | Quit |

## 🚀 Build & Run

Works on **macOS** and **Linux**.

```bash
git clone https://github.com/makskovtun/snake-terminal-cpp.git
cd snake-terminal-cpp
g++ -std=c++17 -o snake main.cpp
./snake
```

## 🧠 How it works

The game runs in a classic loop every 100 ms:

| Function | What it does |
|----------|--------------|
| `Setup()` | Places the snake and the first fruit |
| `Draw()` | Renders the field using ANSI escape codes |
| `Input()` | Reads the pressed key without blocking |
| `Logic()` | Moves the snake, handles collisions and eating |

## 🛠 Tech

C++ · POSIX `termios` / `fcntl` · ANSI escape codes

---

Made by [Maks](https://github.com/makskovtun)
