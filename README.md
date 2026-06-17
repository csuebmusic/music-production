# music-production

Handouts and browser-based tools for the music producers Inés Thiebaut works with in private lessons, independent of any single course. Where MUS 381 ([`csuebmusic/mus381`](https://github.com/csuebmusic/mus381)) is built around one course's arc and hands off to a graduate TA, this repository follows the producer: beat-making, mixing, arrangement, DAW production, and the craft questions that come up across projects rather than inside a syllabus.

Material here can borrow from the 381 handouts as a starting point, adapted for an audience that can go a step deeper than the course baseline and reframed away from course scaffolding such as the lab session routines, the NAS sync workflow, and the TA teaching notes.

The landing page holds everything in one place: **[csuebmusic.github.io/music-production](https://csuebmusic.github.io/music-production/)** (built from `index.html` at the repo root).

## Contents

Live pages, grouped by section. The learning arc runs concepts to capture to production, with listening alongside.

**Foundations** — the ideas under the craft.
- [Digital Audio Fundamentals](https://csuebmusic.github.io/music-production/foundations/digital-audio.html)
- [Editing concepts & envelope](https://csuebmusic.github.io/music-production/foundations/editing-envelope.html)
- [More on envelopes & LFOs](https://csuebmusic.github.io/music-production/foundations/envelopes-lfos.html)
- [Mixing](https://csuebmusic.github.io/music-production/foundations/mixing.html)
- [Dynamics, compression & limiting](https://csuebmusic.github.io/music-production/foundations/dynamics.html)

**Recording** — capturing your own sound, one mic up to the full studio.
- [A Simple Recording Chain](https://csuebmusic.github.io/music-production/recording/recording-chain.html)
- [Widening the Flow](https://csuebmusic.github.io/music-production/recording/widening-the-flow.html)
- [The Mixer](https://csuebmusic.github.io/music-production/recording/the-mixer.html)
- [The Studio](https://csuebmusic.github.io/music-production/recording/studio.html)

**The DAW** — producing in Ableton Live.
- [Into the DAW](https://csuebmusic.github.io/music-production/daw/the-daw-environment.html)
- [Audio Editing in Ableton](https://csuebmusic.github.io/music-production/daw/audio-editing.html)
- [Sampling in Ableton](https://csuebmusic.github.io/music-production/daw/sampling-in-practice.html)
- [Mixing in Ableton](https://csuebmusic.github.io/music-production/daw/mixing-in-practice.html)

**Listening**
- [Listening](https://csuebmusic.github.io/music-production/listening/listening.html)

## Visual system

Producer-facing material uses a retro-geek look that is deliberately distinct from 381: a light terminal/printout aesthetic on a white page, near-black green-tinted ink, a burnt-amber accent, and DM Mono carrying the chrome (a status-bar header, bracketed `[ LABEL ]` callouts, `//` and `▸` markers, an EOF footer). It reads like a vintage software manual rather than 381's warm cream and rust. Everything is self-contained and browser-only. The CSS custom properties (`--bg`, `--bg-alt`, `--ink`, `--ink-soft`, `--accent`, `--rule`, and the meter / gain-reduction / cable families) are always referenced by name, never written as raw hex in component CSS, so diagrams ported from 381 re-skin themselves to this palette with no edits. `assets/style.css` defines the system and is owned by this repo.

## Structure

A root `index.html` is the landing page and the GitHub Pages entry point; it links to every page. Topic-named files live under topic folders, with the course-style order numbers and `reading-` / `handout-` / `tool-` prefixes dropped (for example `foundations/digital-audio.html`). Per-topic media lives under `assets/audio/<topic>/`, `assets/images/<topic>/`, and `assets/videos/<topic>/`. The layout grows as materials land rather than being imposed up front.

```
music-production/
├── index.html          Landing page (GitHub Pages entry point)
├── README.md
├── assets/
│   ├── style.css       The retro-geek system, owned by this repo
│   ├── audio/<topic>/
│   ├── images/<topic>/
│   └── videos/<topic>/
├── foundations/        Concepts: digital audio, editing, envelopes, mixing, dynamics
├── recording/          Capture: the chain, wider signal flow, the mixer, the studio
├── daw/                Ableton Live: environment, audio editing, sampling, mixing
└── listening/          Listening guide
```
