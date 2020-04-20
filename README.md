# Red Planet

An immersive, rapid game builder with a built-in HTML5 game engine.

Features:

- [x] Easy, immersive level creation
- [x] Basic platformer or top-down dynamics
- [x] Viewport automatically follows player
- [x] Gravity & gravity-changing tiles (via `setGravity(0, 1)`)
- [x] Spring tiles (via `setSpeed(0, -20)`)
- [x] Solid and pass-through tiles
- [x] Portals (via `setPosition(x, y)`)
- [x] Spikes (via `restart()`)
- [x] Checkpoints (via `setStart(x, y)`)
- [x] Level exit & portal tiles (via `loadLevel(level_name)`)
- [x] Image Editor
- [x] Infinite level size

Player API:

* `setGravity(x, y)`
* `setSpeed(x, y)`
* `setPosition(x, y)`
* `setStart(x, y)`

Tile API:
* `createTile(grid_x, grid_y, sprite_id)`
* `cloneTile(tile, overrides)`
* `getTile(grid_x, grid_y)`
* `deleteTile(tile)`
* `getGridX/Y(tile)` and `setGridX/Y(tile, new_value)`
* `fireEvent(tile, event_name)`
* `await animate(tile, steps, seconds_per_step)`

General API:
* `loadLevel(level_num)`
* `await timeout(seconds)`
* `setStatus(message)`
* `setCursor(cursor_id)`
* `alert(message)`

Tile Properties:
* `.opacity` (number between 0 and 1)
* `.x` and `.y` (number of pixels from top-left corner)
* `.w` and `.h` (width and height, in pixels)
* `.sprite_x` and `.sprite_y` (coordinates of the sprite to draw)
* `.img_ix` (which spritesheet to look for sprite, indexes start at 0)
* `.types` (array of type strings, used for ECS)
* `.is_solid` (true/false; whether it passes through other solid objects)
