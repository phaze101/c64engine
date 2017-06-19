# c64engine
a game engine for the c64

## Building

```bash
acme engine.acme
```

## Run

```bash
x64 engine.prg
```

Use joystick in port 2 to run the demo.

## Features

* Bitmap scrolling using [AGSP](http://codebase64.org/doku.php?id=base:agsp_any_given_screen_position)

    This technique only requires 36 raster lines CPU time and 33 raster lines of screen space. All other screen space - including screen memory (used for colors ```%01``` and ```%10```) and color ram (color ```%11```) is moved around as well.
    The code for copying around tiles is not yet implemented.
    
* Sprite-Multiplexer

    Multiplixing 24 x 2 sprites. This means 24 virtual multi-color sprites where each sprite is overlayed with a single-color sprite for more colors and better resolution.
