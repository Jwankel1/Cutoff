# Cutoff

A 3D light-trail duel for the browser, playable in VR (WebXR) or on a flat screen.

Two drones fly freely through one large room (80 x 36 x 80 m), each leaving a solid trail of light behind it. Fly into a trail or a wall and you lose. After 15 seconds the room shrinks a step every 6 seconds, with a rumble, so space always runs out.

- **1 player** against the computer (Easy, Normal, Hard), in VR or on screen
- **2 players** in split screen, on one keyboard or two gamepads

## Play

The whole game is `index.html`. It loads three.js from a CDN and needs no build step.
VR needs the page served over HTTPS, for example with GitHub Pages
(Settings → Pages → deploy from the `main` branch), then opened in the headset browser.

## Controls

Steering is free flight: turn left and right, climb and dive. The view stays level.

| | Steer | Boost |
|---|---|---|
| VR controllers | Either thumbstick (forward climbs, back dives) | Hold a trigger |
| Player 1 keys | A / D turn, W climb, S dive | Left Shift |
| Player 2 keys | Arrow keys | Right Shift |
| Gamepad | Left stick or d-pad | A or right trigger |
| Touch | Drag like a joystick | Hold the Boost button |
