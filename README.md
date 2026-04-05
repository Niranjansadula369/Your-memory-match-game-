# Your-memory-match-game-
🃏 Memory Match — a sleek card-flipping puzzle game. Flip cards to find matching pairs, track your moves &amp; time, and clear the board. Two difficulty modes: 4×4 and 6×4. Built with pure HTML, CSS &amp; JavaScript. No libraries needed!
# Memory Match Game

A clean, polished card-flipping memory puzzle built with pure HTML, CSS, and vanilla JavaScript — no libraries, no frameworks, no dependencies.

---

## Demo

Open `memory_match.html` directly in any browser. No server or installation required.

---

## How to Play

1. Click any card to flip it and reveal the symbol underneath
2. Click a second card — if both symbols match, they stay face-up and turn green
3. If they don't match, both cards flip back after a short pause
4. Find all pairs to win the game

---

## Features

- Two difficulty modes — **4×4** (8 pairs) and **6×4** (12 pairs)
- Live tracking of **moves**, **matched pairs**, and **time**
- Timer starts on your first flip
- Win screen shows your final score (moves + time)
- New shuffled layout on every restart
- Smooth CSS 3D flip animation
- Fully responsive layout

---

## Tech Stack

| Layer | What's used |
|---|---|
| Structure | HTML5 |
| Styling & animation | CSS3 (3D transforms, backface-visibility) |
| Game logic | Vanilla JavaScript (ES6) |
| Shuffle algorithm | Fisher-Yates |

---

## Project Structure

```
memory_match.html   ← entire game in one self-contained file
README.md
```

---

## How It Works

Each card is a CSS 3D element with two faces — a plain back and an emoji front. The front starts pre-rotated 180° so it stays hidden. Clicking a card adds a `.flipped` class which rotates the whole card, revealing the emoji.

The game tracks the two currently flipped cards. On a match both cards receive a `.matched` class and stay green. On a mismatch the board locks for 900ms (so you can memorise the positions), then flips both cards back and unlocks.

Emojis are picked randomly from a pool of 12, duplicated into pairs, and shuffled with Fisher-Yates on every new game — guaranteeing a different layout each time.

---

## Getting Started

```bash
# Clone the repo
git clone https://github.com/your-username/memory-match.git

# Open the game
open memory_match.html
```

---

## License

MIT — free to use, modify, and distribute.
