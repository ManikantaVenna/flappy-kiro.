# 👻 FLAPPY KIRO: The Unemployed Ghost

A tiny ghost in a business suit flaps through the absurd horrors of the corporate
hiring process. Dodge giant rejection emails, judgmental interview panels, HR robots,
LeetCode walls, coffee machines, and signs demanding **"ENTRY LEVEL: 10 YEARS EXPERIENCE."**

A one-tap, Flappy-Bird-style arcade game — **100% self-contained in a single
`index.html`**. No backend, no npm, no dependencies, no external images. Everything
(art, animation, and sound) is generated programmatically with HTML5 Canvas and the
Web Audio API.

> Built to run in **Chrome on Android** with touch controls, in responsive portrait mode.

---

## 🎮 How to play

- **Tap anywhere** to flap and stay airborne.
- Fly through the gaps between corporate nightmares.
- **Collect coffee cups ☕** to trigger **SUPER CAFFEINATED MODE** for 5 seconds:
  sunglasses, a glowing aura, and protection from **one** collision.
- Survive as long as you can. Difficulty ramps up the longer you last.

### Milestones
- **10 points** — a jet-packing HR robot flies in muttering *"We'll circle back!"*
- **25 points** — confetti rains down and you finally land a (totally real, definitely
  not unpaid) **JOB OFFER** 🎉. Play continues endlessly after that.

### Features
- Expressive, adorable ghost that sweats, panics, rolls its eyes, and dramatically cries.
- Comic-book pop effects: **BONK!**, **WHOOSH!**, **REJECTED!**
- Rotating HR commentary ("HR is typing…", "Your résumé was eaten by AI 🤖", …).
- Randomized game-over rejection letters.
- Layered parallax office skyline, confetti, particles.
- Web Audio sound effects with a **mute** button, plus **pause** and best-score saving
  (`localStorage`).

### Controls
| Action | Touch | Keyboard (desktop) |
|--------|-------|--------------------|
| Flap / Start / Restart | Tap screen | `Space` / `↑` |
| Pause / Resume | ⏸ button | `P` |
| Mute / Unmute | 🔊 button | `M` |

---

## ▶️ Run it locally

It's a single file — just open it:

```
# Option A: open the file directly
open index.html        # macOS
xdg-open index.html    # Linux
# (or double-click index.html)

# Option B: serve it (recommended for Web Audio autoplay rules)
python3 -m http.server 8000
# then visit http://localhost:8000
```

---

## 📱 Play & share it from your phone with GitHub Pages

1. Make sure `index.html` is on the **`main`** branch of this repo (merge the PR that
   adds it).
2. On GitHub, go to **Settings → Pages**.
3. Under **"Build and deployment" → Source**, choose **"Deploy from a branch"**.
4. Set **Branch** to `main` and the folder to **`/ (root)`**, then click **Save**.
5. Wait ~30–60 seconds. GitHub shows your live URL, which looks like:

   ```
   https://ManikantaVenna.github.io/flappy-kiro./
   ```

6. Open that URL in **Chrome on your Android phone** and start flapping. Share the link
   with anyone — it runs entirely in the browser.

> 💡 Tip: In Chrome on Android, use the **⋮ menu → "Add to Home screen"** to launch it
> fullscreen like a native app.

---

## 🛠️ Tech notes

- Pure vanilla JS, HTML, and CSS in one file.
- Canvas scales to the device with `devicePixelRatio` for crisp visuals and a
  frame-rate-independent game loop (smooth on 60fps+ displays).
- Forgiving circular hit-boxes for fair collisions.
- Append `?debug` to the URL to expose a small `window.__kiro` test hook (used for
  automated logic testing; harmless during normal play).

Made for the "Most Creative and Funniest Game" award. Good luck out there — the job
market is rough, even for ghosts. 👻📄
