<div align="center">

# vibetag 🏷️

**personalized emoji combos for your friends' contacts (and your bio ♡)**

describe a friend → get little emoji combos that match their vibe, relationship, and aesthetic.

[**✨ try it live**](https://therealzoyak.github.io/vibetag/) · made with 💜 by [Zoya Khan](https://github.com/therealzoyak)

</div>

---

## the idea

people have friends who give off a certain *vibe* — the chaotic mom-friend, the matcha-and-astrology bestie, the online friend who's secretly a genius. **vibetag** turns that vibe into a cute emoji combo you can drop straight into their contact name (or your Pinterest / IG bio).

it started as a personal habit — i tag my friends' contacts with emojis — and grew into a tiny [neal.fun](https://neal.fun)-style toy.

## what it does

- 📝 **describe them** — interests, personality, your relationship
- ♓︎ **astrology mode** — toggle it on, pick their sign, get cosmic combos
- 🎛️ **dial in the vibe** with four sliders:
  - **how many emojis** (2–6)
  - **on the nose ↔ deep cut** — literal (`smart → 🤓`) or clever (`smart → 📊 ♟️ 💻`)
  - **variety across options** — how different the choices are from each other
  - **focus within a combo** — one clean identity (`🌸`) or all their different sides (`🌈`)
- 🎨 **three styles** — cute, aesthetic (bio-ready ⋆˚), or funny 💀
- 📋 **one-tap copy** + regenerate

## run it locally

it's a single static file — no build step, no dependencies.

```bash
# just open it
open index.html

# ...or serve it
npx serve .
```

## roadmap

- [ ] **Claude-powered generation** — swap the built-in dictionary for a Claude API call so *any* description works and the "deep cut" combos get genuinely clever
- [ ] shareable result cards (screenshot-friendly)
- [ ] more styles (y2k, soft-girl, goth) + bigger emoji vocab
- [ ] save your favorites

## how it works (v1)

the current generator matches keywords in your description against a hand-built dictionary, where each keyword maps to a *literal* and a *deep-cut* emoji pool. the sliders then control how it samples and arranges them. it's fully offline and instant — the trade-off is it only knows words it's been taught. the Claude upgrade (see roadmap) removes that ceiling.

## license

[MIT](LICENSE) © Zoya Khan
