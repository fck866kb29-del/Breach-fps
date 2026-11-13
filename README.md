# BREACH — Dock 07

**BREACH** is an original, lightweight first-person shooter built for the browser with WebGL. Jump into a compact industrial arena, fight AI opponents, and get straight into the action—no installation required.

## Play

The game is contained in `index.html` and does not require external JavaScript libraries or downloaded 3D models.

- **Desktop:** Use WASD to move, the mouse to look, left-click to fire, right-click to aim, Shift to sprint, Space to jump, R to reload, and 1/2 to switch weapons.
- **Mobile:** Rotate your device into landscape orientation. Use the on-screen joystick, touch aiming, and action buttons. On iPhone, turn off Portrait Orientation Lock if needed; mobile Safari does not reliably support automatic orientation locking.

You can open `index.html` locally in a modern WebGL-capable browser. To make it accessible via a website, configure a static hosting service such as GitHub Pages.

## Current features

- Procedurally generated low-poly 3D graphics, textured asphalt, depth-tested solid scenery, and an industrial shipping yard
- First-person camera with full horizontal and vertical aiming
- Two weapons with distinct, easy-to-control camera recoil, visual weapon kick, smooth ADS, muzzle flash, hit markers, and multiple hit zones
- Procedurally generated shot/impact audio with an in-game sound toggle
- AI opponents, respawns, an elimination counter, and a radar
- Touch controls and adjustable rendering quality

## Project status

This repository currently contains a **single-player prototype with bots**. Online multiplayer, matchmaking, accounts, and anti-cheat are planned ideas—not implemented features.

## Development

The game currently lives in `index.html` for simple deployment. Future updates can split rendering, game logic, controls, and networking into separate modules.

## Publishing

The repository is public. GitHub Pages can serve the root `index.html` from the `main` branch after Pages is enabled in repository settings.

BREACH is an independent original project. It does not use assets or branding from other FPS games.

## Fullscreen and touch controls

- **iPhone:** Use Safari → Share → **Add to Home Screen**, then launch BREACH from the new icon. This opens it as a standalone web app without Safari's address bar. Keep Portrait Orientation Lock off and turn the phone sideways.
- **Other supported browsers:** Tap **FULLSCREEN** in the game. Where the Fullscreen API is unavailable, the button displays alternative instructions.
- **Aiming:** Hold **AIM** while you want to zoom. Let go to return to normal view, so aiming cannot accidentally remain toggled on.
- **Accidental browser zoom:** The game surface suppresses double-tap/pinch gestures during matches, while normal browser zoom remains available outside gameplay.

iPhone Safari does not reliably permit arbitrary webpage elements to enter native fullscreen on demand. The Home Screen launch is the preferred iPhone workaround.
