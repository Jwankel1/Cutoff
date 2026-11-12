# Cutoff

A 3D light-trail duel for the browser, playable in VR (WebXR) or on a flat screen.

Two drones fly through one large room, each leaving a solid ribbon of light behind it. Fly into a ribbon or a wall and you lose. The walls close in every few seconds, so the room always runs out.

- **1 player** against the computer (Easy, Normal, Hard), in VR or on screen
- **2 players** in split screen, on one keyboard or two gamepads

## Play

The whole game is `index.html`. It loads three.js from a CDN and needs no build step.
VR needs the page served over HTTPS, for example with GitHub Pages
(Settings → Pages → deploy from the `main` branch), then opened in the headset browser.

## Controls

| | Steer | Level off | Boost |
|---|---|---|---|
| VR controllers | Flick either thumbstick | A or X | Hold a trigger |
| Player 1 keys | A / D turn, W climb, S dive | E | Left Shift |
| Player 2 keys | Arrow keys | / | Right Shift |
| Gamepad | Stick or d-pad | B | A or right trigger |
| Touch | Swipe | | Hold the Boost button |
