# Lobster Claw 🦞

A webcam party game where you catch lobsters escaping from a tank -- grab them with your hands or chomp them with your mouth. Uses MediaPipe face and hand tracking to turn your webcam into a lobster-catching claw machine.

Inspired by [Shark Snatch](https://github.com/ashleywolf/shark-snatch) with OpenClaw vibes.

## How to Play

**With your hands (claw machine style):**
- Hold your hand up so the camera can see it
- Pinch your thumb and index finger together to GRAB a lobster
- A claw machine arm follows your hand position

**With your mouth:**
- Look at the camera and line up with a lobster
- Open your mouth wide to CHOMP it

Both methods work simultaneously -- use hands and mouth at the same time for maximum chaos.

## Rules

- Lobsters swim across the screen from all directions
- Catch them before they escape off the edges
- Each escape costs a life (you get 8)
- Difficulty increases every ~55 seconds
- Combo multiplier for quick consecutive catches (up to 5x)

## Lobster Types

| Type | Size | Points | Frequency |
|------|------|--------|-----------|
| Baby (orange) | Small | 1 | Common |
| Regular (red) | Medium | 2 | Moderate |
| King (dark red, crown) | Large | 5 | Rare |

## Tech

- Single HTML file, no build step
- MediaPipe FaceLandmarker (mouth tracking, up to 4 faces)
- MediaPipe HandLandmarker (pinch detection, up to 4 hands)
- Canvas 2D rendering
- Procedural audio via Web Audio API
- Supports multiple players (multiple faces/hands tracked simultaneously)

## Play It

Open `index.html` in a browser with webcam access, or visit the GitHub Pages URL.

Requires a device with a camera and a browser that supports MediaPipe (Chrome, Edge, Safari).
