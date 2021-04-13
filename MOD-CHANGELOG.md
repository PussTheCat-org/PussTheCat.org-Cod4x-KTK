# 2021-04-09 - Update 1

- Added bot king skill
- Fix for the score

# 2021-04-10 - Update 2

Plugins:
- Fixed the xmodel plugin to be able to play the HnS event again

Mod code:
- Changes the title for the "Hall of Fame" to explain that it's an "All time" leader-board 
- Fixed the display of the team icons on round end (fixes https://github.com/PussTheCat-org/PussTheCat.org-Cod4x-KTK/issues/7 )
- Replaced the execution of "map_restart" with the cod4 default function
- Added a screen print when HnS can not start because the xmodel file is not written/read

# 2021-04-12 - Update 3

Addition:

- Added "none" as constant event to the event vote
- Added a fps check to avoid glitching through lolzor spawn protection
- Added a dvar check for the version on loadscreen

Enhancement:

- Changed the throw time of the throwing knife
- Changed healthbar of king and terminator to hide it when a menu is on top
- Removed the ammo counter for melee weapons
- Replaced the zombie dog model with a better paint weighted one

Fixes:

- Fixed Bot rapid fire (added delay between to shots; Durating grabbed from weapon file)
- Fixed Bot spawn on round start (removed the delay)
- Fixed sensitivity of the fast-fire-detection
- Fixed the team switch on new round of HnS
- Fixed the damage detection of props in HnS

---

The Mod.ff and some IWDs have changed because of those changes:

- Replaced the zombie dog model with a better paint weighted one
- Removed the ammo counter for melee weapons
- Changed the throw time of the throwing knife
