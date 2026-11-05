# Space Cinema

A small 3D user interface built with **A-Frame**: a control console that switches the videos shown on a cinema screen.

## Features

* Cinema screen with a welcome layer that disappears on the first interaction.
* Control console with four buttons: Moon, Solar System, Galaxy and Galaxy 2.
* Each button plays its own video on the screen and stops the previous one.
* Indicator light on each button showing which video is active.
* Hover and click sound effects.
* Interactive hover and press effects on the buttons.
* Mouse, VR controller and hand tracking (pinch) interaction.

## Project Structure

```
.
├── index.html
├── README.md
└── assets
    ├── night.jpg
    ├── sounds
    │   ├── click.wav
    │   └── hover.wav
    ├── textures
    │   ├── dark_rock_02_diff_4k.jpg
    │   └── metal_plate_diff_4k.jpg
    └── videos
        ├── galaxy.mp4
        ├── galaxy2.mp4
        ├── moon.mp4
        └── solar.mp4
```

## How to Run

1. Download or clone the project.
2. Make sure the `assets` folder contains the required files:
   * `night.jpg`
   * `videos/` (`moon.mp4`, `galaxy.mp4`, `galaxy2.mp4`, `solar.mp4`)
   * `sounds/` (`hover.wav`, `click.wav`)
   * `textures/` (`dark_rock_02_diff_4k.jpg`, `metal_plate_diff_4k.jpg`)
3. Open the project using a local web server (for example, the Live Server extension for VS Code). Opening `index.html` directly from the file system may block the videos and textures.
4. Open the page in your browser.

## Controls

* **Mouse:** move the cursor over a button and click.
* **VR controllers:** point the laser at a button and press the trigger.
* **Hand tracking:** point at a button and pinch.

## Testing

The project was tested in Google Chrome using the **Immersive Web Emulator** browser extension by Meta, with the **Meta Quest 2** headset selected as the emulated device. Both the controller input mode and the hand input mode were tested.

## Built With

* [A-Frame](https://aframe.io/) 1.8.0
* [aframe-event-set-component](https://github.com/supermedium/aframe-event-set-component)
