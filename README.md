# Cutoff

A 3D light-trail duel for the browser, playable in VR (WebXR) or on a flat screen.

Two drones fly freely through one large room (80 x 36 x 80 m), each leaving a solid trail of light behind it. Fly into a trail or a wall and you lose. After 15 seconds the room shrinks a step every 6 seconds, with a rumble, so space always runs out.

- **1 player** against the computer (Easy, Normal, Hard), in VR or on screen
- **2 players** in split screen, on one keyboard or two gamepads

The soundtrack plays throughout, starting muffled and distant and opening up as the
room closes in. It can be turned off on the menu.

## Swapping the soundtrack

Tracks live in `music/`. To change one:

1. Put the audio file in `music/`.
2. Edit the `TRACKS` list near the top of the script in `index.html`:

```js
const TRACKS = [
  { name: 'Prog Trance A', src: 'music/cutoff_prog_trance_takeA_00001.mp3' },
];
```

The first entry plays. List more than one and a Track picker appears on the menu,
and the choice is remembered. Empty the list and the game falls back to a
soundtrack generated in code — ambient pads that build into a beat as the room
closes.

## Scoring

Staying alive pays a little. Most of the score comes from close passes: fly within
about two metres of a trail or a wall and the points land as you pull away, scaled
by how tight the gap was. Chain passes within four seconds to build a multiplier up
to x8, and cutting the computer off is worth a bonus. Best score, longest run and
win streak are kept in the browser.

## Play

The whole game is `index.html`. It loads three.js from a CDN and needs no build step.
VR needs the page served over HTTPS, for example with GitHub Pages
(Settings → Pages → deploy from the `main` branch), then opened in the headset browser.

## Controls

Steering is free flight: turn left and right, climb and dive. The view stays level.

| | Steer | Boost |
|---|---|---|
| VR controllers | Either thumbstick, flight-stick style: pull back to climb, push forward to dive | Hold a trigger |
| Player 1 keys | A / D turn, W climb, S dive | Left Shift |
| Player 2 keys | Arrow keys | Right Shift |
| Gamepad | Left stick, pull back to climb; d-pad up climbs | A or right trigger |
| Touch | Drag like a joystick | Hold the Boost button |
