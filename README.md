# music-production

Handouts and browser-based tools for the music producers Inés Thiebaut works with in private lessons, independent of any single course. Where MUS 381 ([`csuebmusic/mus381`](https://github.com/csuebmusic/mus381)) is built around one course's arc and hands off to a graduate TA, this repository follows the producer: beat-making, mixing, arrangement, DAW production, and the craft questions that come up across projects rather than inside a syllabus.

Material here can borrow from the 381 handouts as a starting point, adapted for an audience that can go a step deeper than the course baseline and reframed away from course scaffolding such as the lab session routines, the NAS sync workflow, and the TA teaching notes.

## Visual system

Producer-facing material uses a retro-geek look that is deliberately distinct from 381: a light terminal/printout aesthetic on a white page, near-black green-tinted ink, a burnt-amber accent, and DM Mono carrying the chrome (a status-bar header, bracketed `[ LABEL ]` callouts, `//` and `▸` markers, an EOF footer). It reads like a vintage software manual rather than 381's warm cream and rust. Everything is self-contained and browser-only. The CSS custom properties (`--bg`, `--bg-alt`, `--ink`, `--ink-soft`, `--accent`, `--rule`, and the meter / gain-reduction / cable families) are always referenced by name, never written as raw hex in component CSS, so diagrams ported from 381 re-skin themselves to this palette with no edits. `assets/style.css` defines the system and is owned by this repo.

## Structure

Topic-named files under topic folders, with the course-style order numbers and `reading-` / `handout-` / `tool-` prefixes dropped (for example `foundations/digital-audio.html`). Per-topic audio lives in `assets/audio/<topic>/`. The layout grows as materials land rather than being imposed up front.
