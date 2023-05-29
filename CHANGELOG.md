# Changelog

## v0.20.0 - 2023-05-29

- Fixed an issue on macOS and Ubuntu where the game would crash or display the wrong key in the Control Configuration menu when the Quote and Backquote keys were assigned to an action
- Fixed an issue on Ubuntu where player data wasn't being saved
- Fixed issue where game could not detect the built-in gamepad on Steam Deck
- Darkened and flipped background for Survival mode to make UI easier to read
- Redid explosion drawing code to get rid of unwanted graphical artifacts
- Made various refactors to the code for better performance

## v0.19.0 - 2023-04-05

- Added two new modes: Dig and Survival
- Next Queue window now scales depending on the length of the queue
- Adjusted piece preview alignments in Hold and Next Queue windows
- Added "Hold" and "Next" headings to game UI
- Adjusted appearance of Ghost Piece
- Adjusted appearance of frozen lines
- Added two new music tracks
- Swapped the backgrounds and default BGMs for Marathon and Sprint
- "New Best!" text no longer appears if the current score ties with the Best Score in Marathon
- Fixed a crash that occurred in-game when Next Queue is set to 0
- Fixed a crash that occurred when more than 20 lines are filled in one move
- Fixed an issue where frozen lines were not clearing during Game Over sequence
- Fixed an issue where the Best Time in the Sprint options menu was displayed incorrectly
- Fixed an issue where hard dropping piece from row 21 or higher would cause it to lock in the wrong position
- Fixed an issue where a piece swapped from Hold would phase through minos near the spawn area via gravity
- Fixed minor issues with lock out conditions
- In-game performance improvements 

## v0.18.1 - 2023-03-12

- Fixed a bug where if a piece was hard dropped during lock delay, the next piece would lock at spawn and end the game with a lock out. (*thanks Rubiktor012*)
- Fixed issue with macOS version not running due to incorrectly-defined min version (*thanks briand*)

## v0.18.0 - 2023-03-11

- Fixed Marathon scoring
  - Spin Minis now award a flat 100 bonus points if there are no filled lines with bombs
  - Spin bonus points are now properly multiplied by Back-to-Back bonus if active
- Fixed high scores not being saved in Marathon and Piece Trial modes (*thanks Talon125*)
- Fixed issues with DAS and ARR (*thanks Xx-Henry-xX*)
  - Added option to enable/disable DAS Cancelling
- Fixed issues and bugs related to top out conditions
- Fixed a bug where the minos of rotated pieces were in the wrong locations after the runtime update
- Fixed an issue where the level up SFX would play more than once if multiple level ups occurred simultaneously
- Fixed an issue where the frozen line SFX would play even if frozen line(s) were formed and cleared with the same move
- Fixed an issue where piece centers were drawn one frame behind where they were supposed to be
  - This also fixes the issue where the piece center would jump up one cell for one frame when the current active piece crossed cell boundaries while Smooth Falling is on
- Fixed an issue where Big Bombs overlapping the current piece would disappear when the player blocks out
- Changed title in Piece Trial options menu from "Piece Attack" to "Piece Trial" (*thanks Talon125*)

## v0.17.2 - 2023-03-06

- First preview release
- Includes three game modes:
  - Marathon (1500 Minos, 2000 Minos, Endless)
  - Piece Trial (100 Pieces, 200 Pieces)
  - Sprint (200 Minos, 400 Minos, 1000 Minos, 10000 Minos)
