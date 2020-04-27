# Red Planet

An immersive, rapid game builder with a built-in HTML5 game engine.

It is designed around an Entity Component System, where the game is defined by properties and components set in the editor.

## Features:

- Easy, immersive level creation
- Basic platformer or top-down dynamics
- Viewport automatically follows player
- Gravity & gravity-changing
- Springs
- Solid and pass-through tiles
- Portals
- Auto-growing level size

## Components:

### Positionable (required)
* Left (x): number (px)
* Top (y): number (px)
* Width: number (px)
* Height: number (px)

### Drawable (required)
* Sprite X: number (horiz. tile index)
* Sprite Y: number (vert. tile index)
* Spritesheet #: number (zero-based index)
* Layer ID: number

### Speed
* Right: number (px/frame)
* Down: number (px/frame)

### Collideable
* Left Padding: number (px)
* Right Padding: number (px)
* Top Padding: number(px)
* Bottom Padding: number (px)

### Animateable
* Number of Frames: number
* Animate Interval: number (ms/frame)

###  Rotateable
* Rotates to Sprite IDs: comma delimited array of sprite IDs

### Growable
* Grow Interval: number (ms, default: 1000)
* Grow Direction: string (default: left)
* Grow Sprite ID: string

### Shoots
* Bullet Sprite ID: string
* Shoot Interval: number (ms, default: 1000)

### Ephemeral (disappears on collide or out-of-bounds)

### Damager
* Damage Points: number (default: 50)

### Damageable
* Health Points: number (default: 100)
* Death Sprite ID: string

### Wins Game on Death

### Loses Game on Death

### Placeable

### Purchaseable
* Cost: number (default: 1)

The following variables are hard-coded & still need to be moved to components:

* Money: number (starting amount, default: 30)
* Earns Amount: number (default: 1)
* Earns Interval: number (ms, default: 5000)
