## 📸 Screenshots / 游戏截图

### Title Screen / 标题界面
![Title Screen](https://github.com/user-attachments/assets/94f5223c-5f24-463b-9b09-9ba48efaea1c)

### Identity Reveal / 身份揭示界面
![Identity Screen](https://github.com/user-attachments/assets/f243047d-2470-4400-90e8-15cc085c2d72)

### Gameplay / 游戏主界面
![Gameplay](https://github.com/user-attachments/assets/d8764fc3-2f75-4652-b71a-fc11cdea285e)

### Guess Phase / 猜身份阶段
![Guess Phase](https://github.com/user-attachments/assets/5de6ec05-3694-4b20-bfa4-288118eaf68a)

### End Game / 游戏结束界面
![End Game](https://github.com/user-attachments/assets/14c06016-9813-4633-a6ac-fac277b76ea9)

A social deduction card game where you don't know your own identity. Playable in browser with AI opponents. Built with vanilla HTML/CSS/JS.
# 🎭 Shadow Council / 暗影议会

> A social deduction card game where you don't know your own identity. / 一款社交推理卡牌游戏，玩家不知道自己真正的阵营身份。

[**Play Online / 在线试玩**](https://Ganeeeee.github.io/shadow-council-card-game/) | [**Game Manual / 游戏说明书**](./manual.html)

---

## 📖 English | 英文

### About

**Shadow Council** is a browser-based card game inspired by social deduction games like *Avalon* and *Werewolf*.

**The core innovation:**
> *"Your shadow identity is randomly assigned by others — only YOU don't know who you are"*

You must deduce your own true faction through clues, then play cards strategically to help your faction win.

### Tech Stack

| Technology | Purpose |
|------------|---------|
| HTML5 + CSS3 | Structure, responsive layout, dark fantasy theme |
| Vanilla JavaScript | Pure native implementation (~2500 lines) |
| Web Audio API | Synthesized sound engine (20+ effects) |
| CrazyGames SDK | Ad integration, distribution |
| Remix Icon + Google Fonts | Icons & typography |

### Core Mechanics

**Dual Identity System**

| Identity Type | Visibility | Effect |
|---------------|------------|--------|
| Public Identity | Visible to all | Determines your passive ability |
| Shadow Identity | Unknown to you | Determines your true faction (win/loss) |

**Four Card Suits**

| Suit | Faction | Core Function |
|------|---------|----------------|
| 🗡️ Military | Order | Attack, defense, zone control |
| 💎 Economy | Order | Resources, gold generation |
| 📜 Strategy | Chaos | Intelligence, deduction |
| 🌙 Shadow | Chaos | Identity manipulation, assassination |

**Game Flow**

**Victory Conditions**
- Order wins if more Order survivors than Chaos
- Chaos wins if more Chaos survivors than Order
- Higher zone total = +1 effective survivor
- Eliminate opposing faction = instant win

### Game Parameters

| Parameter | Value |
|-----------|-------|
| Players | 4-6 (human + AI mix) |
| Total Rounds | 6 |
| Starting Resources | 4 gold + 7 cards |
| Actions Per Turn | 2 (1 card = 1 action) |

### AI System

- Weight-based decision engine
- AI uses collected clues for deduction
- Supports human + AI mixed play
- 50% chance per round for 1 AI to guess

### Project Scale

| Metric | Value |
|--------|-------|
| Lines of Code | ~2500 |
| Card Types | 32 × 2 = 64 cards |
| Identity Types | 6 (3 Order + 3 Chaos) |
| Random Events | 12 |
| Sound Effects | 20+ procedural |

### Design Highlights

- **Dark Fantasy Visual** — Gradients, glow borders, glassmorphism, fully custom CSS
- **Web Audio Engine** — 20+ procedural effects, no external audio files
- **Complete State Machine** — Event → Passive → Action → Zone → Guess, watchdog anti-freeze
- **Mobile Optimized** — Touch-friendly, horizontal scroll for cards, responsive breakpoints

### Local Development

```bash
git clone https://github.com/yourusername/shadow-council-card-game.git
cd shadow-council-card-game
# Use Live Server (VS Code) or:
python -m http.server 8000
# Open http://localhost:8000









