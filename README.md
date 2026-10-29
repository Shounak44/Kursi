# KURSI: The Night Before

> *"Don't let them make you comfortable, Meera."*

A single-file, browser-based political drama / interactive story. It is 2:14 AM, the Chief Minister is dead, and you are his deputy, **Meera**. You have one night and one morning to decide who you are before the House votes on who gets the chair.

No installs, no build step, no dependencies. Just one `kursi-game.html` file.

### 🎮 [Play it live here](https://bitter-fire-505.linkyhost.com)

## Play

**Online:** open **https://bitter-fire-505.linkyhost.com** in any modern browser, on desktop or mobile.

**Locally:** download `kursi-game.html` and open it in any modern browser.

**Host it yourself (e.g. GitHub Pages):**
1. Rename `kursi-game.html` to `index.html`.
2. Go to **Settings → Pages**, choose your branch and `/ (root)`, and save.
3. Your game will be live at `https://<your-username>.github.io/<repo-name>/`.

> An internet connection is only needed for the Google Fonts (Bricolage Grotesque and Fraunces). The game falls back to system fonts if they cannot load.

## About the game

You play through **7 chapters**, talking to a cast of allies and rivals while your choices quietly shift hidden values like integrity, public support, and loyalty.

| # | Chapter | Setting |
|---|---------|---------|
| 1 | The Call | General Hospital, 2:14 AM |
| 2 | The Folder | Secretariat, morning |
| 3 | Live | TV studio, 9 PM |
| 4 | Rampur | By the broken bridge |
| 5 | Dev's Price | Dev's farmhouse, midnight |
| 6 | The Leak | CM's residence, 6 AM |
| 7 | Vote of Confidence | State Assembly, vote day |

### Cast
**Dev** (the kingmaker with a price) · **Naina** (the journalist) · **Kabir** (your loyal aide) · **Lata** and **Vikram** (rival power brokers) · **Sunita** (a Rampur survivor) · **Anjali** (Raghav's widow)

### Features
- **8 different endings**, from clean victories to honest defeats, with a tracker on the title screen showing which you have found
- **Branching choices** that change relationships, alliances, and the final vote count
- **Mini-games and puzzles**: picking the entries that matter, ordering evidence, code and lock puzzles, a budget puzzle, and the final vote whip
- **Timed decisions** at high-pressure moments
- **Animated character portraits** drawn in SVG, with moods (angry, sad, shocked, smile, smirk), blinking, and a talking mouth that syncs with the typewriter text
- **Procedural audio** built with the Web Audio API: music, sound effects, and typing sounds, with separate volume controls
- **Auto-save** so you can close the tab and continue later (stored in your browser's `localStorage`)
- **Responsive** layout for desktop and mobile

## Controls

| Action | Input |
|--------|-------|
| Advance dialogue / skip typing | Click, tap, or keyboard |
| Pause menu / settings | `Esc` |
| Make a choice | Click or tap an option |

## Tech

- Plain HTML, CSS, and vanilla JavaScript in a single file
- Characters, backgrounds, and ending art are all inline SVG
- Audio is generated in real time with the Web Audio API (no audio files)
- Progress and unlocked endings are saved in `localStorage`

## Project structure

```
.
├── kursi-game.html   # the entire game
└── README.md
```

## Resetting progress

Save data lives in your browser under the keys `kursi_save_v1`, `kursi_ends_v1`, and `kursi_vol_v1`. Clear them from your browser's site data (or run `localStorage.clear()` in the console) to start fresh.

## Credits

Written, designed, and built by **Deep**.

## License

Add the license of your choice here (for example, [MIT](https://choosealicense.com/licenses/mit/)).
