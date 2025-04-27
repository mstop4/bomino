# Changelog

## v0.21.4 - 2025-04-26 - (Future Release)

- Fixed crash when changing settings in Marathon menu (Thanks Kilroy_1541).

## v0.21.3 - 2024-05-28 - (Current release)

- Fixed an issue where garbage lines were playing the "Trance Dance" track instead of the proper sound effect when added to the well.

## v0.21.2 - 2024-05-27

- DAS cancelling is now On by default
- Fixed an issue where regular minos would stay suspended in midair in Dig mode (thanks BlandJar)

## v0.21.1 - 2023-12-03

- Fixed a crash that occurred when performing a Spin without line fills while Back-to-Back bonus is active (thanks BlandJar)

## v0.21.0 - 2023-11-27

- Added new mode: Contest
  - Added new mino types: Hard (needs two explosions to clear) and Fixed (not affected by gravity)
  - Added one new BGM option
  - Added one new background
- Added a "Press Any Button" prompt on the first time the main menu is shown. If a controller button is pressed during this prompt,
  that controller will become the active controller. If a keyboard key is pressed instead, the game will auto-assign an active controller
  - Improved auto-assignment of the active controller. Game will try to use the first available connected controller instead of always defaulting to slot 0
- Added Smooth Shift option. When turned On, horizontal piece movements are animated smoothly. This is indpendent of Smooth Falling
- Added Restore Defaults option to Control Configuration menu
- Added Change Controller option in Control Configuration menu. This allows you to change the active controller
- Added save data backups. Whenever the game autosaves, it keeps the old save files as a backup
- Fixed bugs that prevented the Show Piece Centers, Screen Shift, and Screen Shake options from working properly
- Pausing and Quick Restarting can now only be done while a piece is in play. This prevent bugs that cause the game to desync when paused in other states
- Fixed a bug where lock delay of the current piece would not reset after Restarting
- After filling in 4 or more lines with a single piece, the next piece will now become a full bomb piece
- Hold piece window is now hidden if Hold Piece is turned off in the options
- Special clear and spin messages (e.g. "Quad", "T-Spin") now shift together with the well and the rest of the HUD
- Fixed a bug that prevented the text "New Best!" from appearing in Marathon and Survival modes
- Adjusted various UI elements to make them easier to read
- Bonus piece counter now appears over ghost piece
- Fixed a bug where the garbage height limit line in Dig Mode would not disappear when lines remaining were approaching 0
- Rebalanced BGM volumes
- Made various refactors to the code for better organization

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
