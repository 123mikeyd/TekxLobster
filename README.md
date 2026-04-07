# TekxLobster

A 2D arcade fighting game built with HTML5 Canvas and JavaScript.

**Play it:** https://123mikeyd.github.io/TekxLobster/

> Note: Must be served from a web server (GitHub Pages, VS Code Live Server, etc.)
> Cannot be opened as a local file because it loads sprite images from the `sprites/` folder.

---

## Characters

| Character | Type | Special |
|-----------|------|---------|
| **TEKNIUM** | Fast / Combo | Energy Blast projectile |
| **LOBSTER** | Heavy / Power | Beam Cannon |

---

## Controls

| Action | Key |
|--------|-----|
| Move | A / D |
| Jump | W |
| Crouch | S |
| Block | Q |
| Light Attack | U |
| Medium Attack | I |
| Heavy Attack | O |
| Special (costs 50 energy) | P |
| **Pause** | **ESC** |

---

## Repo Structure

```
TekxLobster/
├── index.html          The game (all logic, no dependencies)
├── sprites/
│   ├── teknium.png     Teknium sprite sheet  (green background, chroma keyed)
│   └── lobster.png     Lobster sprite sheet  (dark gray background, chroma keyed)
│   └── stage.png       Stage background image
└── README.md
```

---

## Editing Sprites

1. Open `sprites/teknium.png` or `sprites/lobster.png` in GIMP or your editor
2. Keep the background color the same (green for Teknium, dark gray for Lobster)
3. Do not change the overall sheet dimensions or frame positions
4. Save and refresh the browser -- changes load instantly

### Sprite Sheet Layout

**Teknium** (1254x1254, green bg `#15F20E`):
| Row | Y | Height | Contents |
|-----|---|--------|----------|
| 1 | 26 | 230 | Idle (3 frames) + Ready + Punch windup + Punch hit |
| 2 | 287 | 219 | Walk Right (5 frames) + Special/Energy blast |
| 3 | 536 | 215 | Walk Left (5 frames) + Jump |
| 4 | 773 | 211 | Walk Back (6 frames, unused) |
| 5 | 1003 | 237 | Aura + Crouch + KO + Hurt (3 frames) |

**Lobster** (1254x1254, dark gray bg `#2F3030`):
| Row | Y | Height | Contents |
|-----|---|--------|----------|
| 1 | 53 | 162 | Idle (4) + Walk Fwd (6) |
| 2 | 253 | 192 | Walk Back (4) + Jump (3) + Crouch (2) |
| 3 | 543 | 147 | Light Atk (3) + Medium Atk (3) + Heavy Atk |
| 4 | 780 | 151 | Special (4 frames) |
| 5 | 1038 | 158 | Block (2) + Hurt (2) + KO (3) |

---

## Running Locally

```bash
# Python (simplest)
cd TekxLobster
python3 -m http.server 8080
# then open http://localhost:8080
```

Or use VS Code with the Live Server extension.

---

## Built With

- Pure HTML5 Canvas + JavaScript
- No frameworks, no build tools, no dependencies
- Sprite sheets generated with AI (ChatGPT), cleaned up in GIMP
- Web Audio API for sound (no audio files needed)

---

## Credits

- Game concept & art direction: @123mikeyd
- Characters: Teknium (Nous Research), Lobster (OpenGAIT community meme)
- Built with Hermes Agent (Nous Research)
