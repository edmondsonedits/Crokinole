# Crokinole

A dependency-free browser Crokinole game built for desktop and mobile.

## Play

Open `index.html` in a browser, or publish the repository with GitHub Pages.

### Controls

1. Tap/click the highlighted outer shooting arc to place your disc.
2. Press the disc and drag backward like a slingshot.
3. Release to shoot. A longer pull creates more power.

## Modes

- **1 Player:** Red vs CPU, with Easy, Normal, and Hard difficulty.
- **2 Players:** Local pass-and-play, Red vs Blue.

## Rules implemented

- 8 discs per player per singles round.
- Shots begin within the player's quadrant with the disc touching the outer shooting line.
- If an opposing disc is in play, the shot must contact an opposing disc directly or by combination.
- If no opposing disc is in play, the shot must play to the middle: an involved disc must finish in/touching the 15 circle or score a 20.
- Invalid shots remove the shooting disc and same-colour discs involved in the shot.
- Centre hole = 20; board zones = 15 / 10 / 5.
- A disc touching a scoring line receives the lower score.
- Four-round match scoring: 2 match points for a round win, 1 each for a tie.

The gameplay model is based on the core singles rules published by the World Crokinole Championship.

## Technical notes

The entire game is contained in `index.html` and uses Canvas, Pointer Events, and Web Audio. No external libraries, images, fonts, APIs, or build process are required.
