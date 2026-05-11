## 📸 Screenshots / 游戏截图

### 1. 标题界面 / Title Screen
![Title Screen](https://github.com/user-attachments/assets/dbf40d0a-8922-4261-a5d6-e4514ffda459)

### 2. 人数选择 / Player Setup
![Player Setup](https://github.com/user-attachments/assets/5c49e89c-0555-4cb9-b81c-b2fc08ba77b7)

### 3. 指定玩家 / Pass Device
![Pass Device](https://github.com/user-attachments/assets/6f75a0fa-b404-41c0-9b0c-31b5cc32dafe)

### 4. 身份揭示 / Identity Reveal
![Game Main](https://github.com/user-attachments/assets/e4b69ba4-e650-4904-b52e-795476e71681)

### 5. 游戏主页面 / Game MainAI 
![AI Thinking](https://github.com/user-attachments/assets/b960046c-ca39-416a-8d42-71193d9ac391)

### 6. 猜测身份 / Guess Phase
![Guess Phase](https://github.com/user-attachments/assets/824aed62-8980-4b5b-8b39-8ff4cbd937d3)

### 7. 思考 / AI Thinking
![Round Event](https://github.com/user-attachments/assets/466fffe8-792b-456a-bf14-c76a1418c47d)

### 8. 游戏结束 / End Game
![End Game](https://github.com/user-attachments/assets/1ba4d617-91fa-43da-bd6c-fee8fb4c925c)
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









