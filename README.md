# ClickFlow

A game and application creation tool that runs entirely in the browser: storyboard, frame, event and picture editors, movements, expressions, an HTML5 runtime, and a LÖVE exporter. Made for everyone trying to make their game without coding.

> [!NOTE]
> This project is **AI-assisted** for now. It means that code is made by humans and robots. *Beep-boop, blah-blah*.

> [!WARNING]
> **EXTREMELY work in progress.** This is an early alpha: features are still being built, formats may change, and bugs are expected. Things will break; save often (projects are also autosaved in the browser). It is not ready for production use yet.

## Run it

Open `index.html` in any modern browser - that is the whole editor, one file, no install, no server. There is an online version if you want.

## URL parameters

The editor boots from URL parameters, like every other webpage.

| URL | Behavior |
| --- | --- |
| *(no parameters)* | Creates a new application automatically |
| `?new` | Same as no parameters: fresh application |
| `?open` | Restores the automatically saved session, then opens the file picker |
| `?help` | Opens the quick start guide |
| `?example=<key>` | Loads a built-in example: `breakout` (Chocobreak (breakout game)), `platform` (Forest Run (platform game with scrolling)), `shooter` (Asteroid Storm (space shooter)) |

## Features

- **Storyboard / Frame / Event / Event List / Picture editors** in the Clickteam Fusion spirit.
- **Global Event Editor** (`View > Global Event Editor`): one event sheet evaluated in every frame; lines naming objects the current frame does not contain are skipped in that frame.
- **Sounds**: samples up to 1 GB, big files streamed; pause / resume / stop per sample; application setting *Play sounds only in their frame* with a per-sound *Continue across frames* flag for music.
- **Movements**: Static, Bouncing Ball, Eight Directions, Platform, Mouse Controlled, **Drag And Drop**, Race Car, Path.
- **Gamepad support** in both runtimes: the standard mapping drives the usual keys (D-pad/stick = arrows, A = Space...), plus explicit joystick conditions (button pressed, X/Y axis compare).
- **Build**: one standalone HTML5 file, or a LÖVE `.love` package for cross-platform (instructions are inside every built package).
- Projects save as `.cflow`.
