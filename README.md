# TekxLobster v2

**2D Arcade Fighter** — Teknium vs Lobster. Built with Hermes Agent.

**Play Online:** [https://123mikeyd.github.io/TekxLobster/](https://123mikeyd.github.io/TekxLobster/)

## Controls

| Action | Key | Action | Key |
|:---|:---|:---|:---|
| Move | A / D | Light Attack | U |
| Jump | W | Medium Attack | I |
| Crouch | S | Heavy Attack | O |
| Block | Q | Special (50 energy) | P |
| Uppercut | J | Pause | ESC |

**Gamepad:** Left stick move, A/B/X/Y attacks, LB block, RB special, Y uppercut

## Moves

### Teknium (Fast / Combo)
- Light → Medium → Heavy chain combos
- Rising Uppercut (J) — anti-air launcher
- Crouch Attack (S + attack) — low sweep
- Jump Attack (attack while airborne)
- Energy Blast (P) — green projectile

### Lobster (Heavy / Power)
- Claw Swipe → Overhead Slam chains
- Spinning Uppercut (J) — devastating launcher
- Crouch Sweep (S + attack) — leg sweep
- Flying Kick (attack while airborne)
- Beam Cannon (P) — fire blast projectile

## Features
- Best of 3 rounds
- Combo system with damage scaling and hitstun decay
- Combo cancel chains (light → medium → heavy → special)
- 3 difficulty levels (Easy / Normal / Hard)
- Adaptive AI with whiff punishment and spacing
- Particle effects, screen shake, slow-mo on KO
- Synthesized sound effects (Web Audio API)
- Gamepad support
- 7 sprite sheets with 60+ unique animation frames

## Run Locally
```bash
cd TekxLobster
python3 -m http.server 8080
# Open http://localhost:8080
```

## Credits
- Teknium: Inspired by Nous Research
- Lobster: OpenGAIT community meme
- Sprite art: AI-generated, refined in GIMP
- Built with [Hermes Agent](https://github.com/hermes-ai/hermes-agent)
