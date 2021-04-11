# Blitz tactics puzzles

The puzzle data files used on https://blitztactics.com

* 125,262 lichess v1 puzzles
  * speedruns and countdowns are generated from a subset of these
* 150 repetition levels, 2912 puzzles
  * around 20 puzzles each level
* 28,649 haste puzzles, same puzzles as 'three'
* 18,308 rated puzzles
* 4 infinity puzzle difficulties
  * easy - 8,960 puzzles
  * medium - 8,219 puzzles
  * hard - 6,652 puzzles
  * insane - 4,533 puzzles

This is the data structure of each JSON file in `lichess-puzzles-v1`:
```
{
  "puzzle_data": {
    "initial_fen": "5r2/5pk1/2p3pp/1p2q3/3rN3/PB2R3/1P4PP/4Q2K b - - 5 36",
    "initial_move_san": "Re8",
    "initial_move_uci": "f8e8",
    "puzzle_fen": "4r3/5pk1/2p3pp/1p2q3/3rN3/PB2R3/1P4PP/4Q2K w - - 6 37",
    "lines": {
      "e4d6": {
        "e5d6": {
          "e3e8": {
            "d4d3": "win"
          }
        }
      }
    }
  },
  "metadata": {
    "id": 125262,
    "rating": 2280,
    "enabled": true,
    "color": "white",
    "game_id": "e2m7WGOU",
    "attempts": 375,
    "vote": 4
  }
}
```

The new lichess puzzles have not been added yet. This is a work in progress.

Each JSON file in `game-modes` contains an array of puzzles with this structure:
```
{
  "id": 51073,
  "fen": "1Q6/8/8/8/8/2K5/k7/8 b - - 13 62",
  "lines": {
    "b8a7": "win",
    "b8a8": "win",
    "b8b3": "win"
  },
  "initialMove": {
    "san": "Ka3",
    "uci": "a2a3"
  }
}
```
