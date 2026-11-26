# Gem Dash

Gem Dash is a browser-based maze and arcade prototype built with Godot. Navigate through two stages, collect glowing energy nodes and power-ups, avoid sentinels, and complete each maze as quickly as possible.

## Play the Game

The project is an exported browser build and should be run through a local web server:

```bash
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in a modern browser.

## Controls

- **Move:** WASD or arrow keys
- **Pause/resume:** Esc
- **Touch devices:** Use the on-screen direction pad
- **Restart or return to the title:** Use the on-screen controls

## Features

- Two maze stages
- Collectible energy nodes and power-ups
- Sentinel enemies to avoid
- Keyboard and touch controls
- Pause, restart, and title-screen controls
- Local display-name results and leaderboard

## Project Status

This repository contains the current playable browser prototype. It is based on the starter maze game; the intended Gem Dash gem-race objective and shared online leaderboard are not yet integrated. Results and leaderboard entries are currently local to the browser.

## Technical Details

The exported game uses Godot WebAssembly and consists of:

- `index.html` — browser entry point
- `index.js` — engine bootstrap
- `index.wasm` — Godot WebAssembly runtime
- `index.pck` — game assets and scene data
- Audio worklet scripts — browser audio support

## Notes

Because this is a WASM browser export, opening `index.html` directly with a `file://` URL may not work consistently. A local HTTP server is recommended.
