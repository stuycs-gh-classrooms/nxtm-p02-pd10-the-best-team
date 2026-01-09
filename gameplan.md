## 1. driver file needs: setup, draw, mousePressed
   - also create tile class & 2d array containing tile class (see below)
## 2. make a grid of tiles, which "reveal" themselves when clicked
   - for now, grid should be like 20x20 tiles
   - tiles go from grey (revealed = false) to not grey (revealed = true)
## 3. make bombs spawn randomly in grid, assign values to tiles.
   - for now, they can be revealed even if revealed = false. pref colored RED, to ensure we can see they've spawned.
   - run through the grid again - for each tile, check the 8 adjacent tiles. if there is a bomb in a tile, increase the tile's value by one.
     - when clicks tiles, it reveals the tile & checks the 4 adjacent tiles.
     - if tile is a bomb: lose.
     - if tile is not a bomb, and value > 0: reveal the tile.
     - if tile is not a bomb, and value = 0: reveal the tile, then check the 4 adjacent tiles.
       - if adjacent tile is a bomb: don't reveal.
       - if adjacent tile isn't a bomb & value > 0: reveal the tile.
       - if adjacent tile isn't a bomb & value = 0: reveal the tile, then check the 4 adjacent tiles (just like done with the previous tile).
\* tiles should display their value, or a color. bomb => red, revealed = false => grey, value > 0 => display value, value = 0 => not grey or red

## other important things to include:
- flags
  - a value representing the starting number of bombs/flags used
- a way to reset the game, also a way to lose if not done yet

## things we also need to do right now:
- create additional game mechanics
- find a way to have more than 1 class
- code
- visuals?
