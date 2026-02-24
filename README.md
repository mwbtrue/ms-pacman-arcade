Ms. Pac-Man Arcade Clone

A fully playable, single-file clone of the classic arcade game Ms. Pac-Man, built entirely with HTML5 Canvas, vanilla JavaScript, and Tailwind CSS.

This project aims to recreate the classic arcade feel, including grid-based movement, ghost AI, retro styling, and synthesized sound effects, all without needing any external assets (images or audio files).

🎮 Play the Game

Simply download the index.html file and double-click it to open it in any modern web browser. No local server or build tools are required!

✨ Features

Zero Dependencies: Everything (logic, styles, rendering) is contained within a single index.html file.

Classic Ghost AI: Features 4 ghosts (Blinky, Pinky, Inky, and Sue) with distinct chase, scatter, and frightened states.

Procedural Audio: Uses the browser's native Web Audio API to synthesize classic arcade sounds dynamically (waka-waka, power pellet sirens, start jingles, etc.)—no .mp3 files needed.

Audio Toggles: Cycle through All Audio, SFX Only, Music Only, or Muted modes.

Cross-Platform Controls: Playable on both desktop (keyboard) and mobile (touch/swipe).

Responsive Styling: Uses Tailwind CSS (via CDN) for a clean, centered, retro arcade cabinet aesthetic.

🕹️ Controls

Desktop (Keyboard):

Arrow Keys or W, A, S, D: Move Ms. Pac-Man

Spacebar: Start Game

P or Escape: Pause / Resume

M: Cycle Audio Modes (All, SFX, Music, Mute)

Mobile (Touch):

Tap Screen: Start Game / Resume from Pause

Swipe: Swipe Up, Down, Left, or Right to queue your next turn.

On-Screen Button: Tap the audio icon in the bottom right to cycle audio modes.

🛠️ Tech Stack

HTML5 Canvas: For rendering the map, entities, and UI overlay.

Vanilla JavaScript (ES6+): For the game loop, entity classes, collision detection, and AI logic.

Web Audio API: For generating real-time waveforms (oscillators) to simulate retro sound chips.

Tailwind CSS: For responsive layout and basic UI styling.

🧠 Architecture Overview

Game Loop: Utilizes requestAnimationFrame for a smooth 60 FPS update and draw cycle.

Grid Movement: Entities snap to a 24x24 pixel grid, allowing for the classic "input buffering" feel where players can queue turns slightly before hitting an intersection.

Map Definition: The level is defined by a simple 2D array, making it easy to design new levels by changing integers (0 = path, 1 = wall, 2 = pellet, 3 = power pellet, 4 = ghost gate).

🚀 Deployment

Because this is a static, single-file application, it can be hosted for free on almost any web hosting platform:

GitHub Pages: Upload to a repository and enable Pages in the settings.

Netlify / Vercel: Drag and drop the folder containing index.html into their web interface.

Tiiny.host: Upload the .html file directly for instant sharing.
