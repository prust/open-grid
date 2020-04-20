# Red Planet

An immersive, rapid game builder, including a simple HTML5 game engine.

Features:

- [x] Easy level creation
- [x] Basic platformer dynamics
- [x] Gravity-changing blocks (`setGravity(x, y)`)
- [x] Springs (`setSpeed(0, -20)`)
- [x] Ability to change block colors (keys 1-9)
- [x] Ability to set blocks as non-solid (pass-through)
- [x] Portals (`setPosition(x, y)`)
- [x] Spikes (`restart()`)
- [x] Checkpoints (`setStart(x, y)`)
- [x] Click selected block to deselect
- [x] Ability to move between levels (`loadLevel(level_name)`)
- [x] Image Editor
- [x] Infinite scrolling

API:

* `setGravity(x, y)`
* `setSpeed(x, y)`
* `setPosition(x, y)`
* `setStart(x, y)`
* `loadGame(game_name)`
* `restart()`
* `loadLevel(level_num)`
* `createTile(grid_x, grid_y, sprite_x, sprite_y, *spritesheet_ix)`
* `cloneTile(tile, overrides)`
* `getTile(grid_x, grid_y)`
* `deleteTile(tile)`
* `getGridX/Y(obj)` and `setGridX/Y(obj, new_val)`
* `fireEvent(object, event_name)`
* `await timeout(seconds)`
* `await animate(obj, steps, seconds_per_step)`
* `setStatus(str)`
