# Snake Drift

A browser snake game with a twist: the arena starts to sway once you've eaten, and the more you eat, the further it tilts and the faster the snake moves.

The controls always follow the grid, not your screen, so "up" means up on the board even when the board is tilted.

## Play

No install or build step. Open `index.html` in any modern browser:

```bash
open index.html
```

## Controls

| Action | Keyboard | Touch |
| --- | --- | --- |
| Steer | Arrow keys or `W` `A` `S` `D` | Swipe |
| Start / play again | `Space`, `Enter`, or the Play button | Tap Play |
| Pause / resume | `Space` (or `Enter` to resume) | Tap Resume |

## How it works

- The board is a 20 × 20 grid. Eating a pink dot scores a point and grows the snake by one.
- Each point speeds the snake up, from 140 ms per step down to 60 ms.
- The sway grows with your score, up to about 38°.
- Hitting a wall or yourself ends the game. Fill the whole board to win.
- Your best score is saved in the browser (`localStorage`), so it stays after you reload the page.

Everything, including HTML, CSS and JavaScript, lives in the single `index.html` file.
