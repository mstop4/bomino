# Changelog

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
- Fixed an issue where the frozen line SFX would play even if frozen line(s) were formed and cleared with the same piece
- Fixed an issue where piece centers were drawn one frame behind where they were supposed to be
  - This also fixes the issue where the piece center would jump up one cell for one frame when the current active piece crossed cell boundaries while Smooth Falling is on
- Fixed an issue where Big Bombs overlapping the current piece would disappear when the player blocks out
- Changed title in Piece Trial options menu from "Piece Attack" to "Piece Trial"

## v0.17.2 - 2023-03-06

- First preview release
- Includes three game modes:
  - Marathon (1500 Minos, 2000 Minos, Endless)
  - Piece Trial (100 Pieces, 200 Pieces)
  - Sprint (200 Minos, 400 Minos, 1000 Minos, 10000 Minos)
