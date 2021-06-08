# 2021-04-09 - Update 1

- Added bot king skill
- Fix for the score

# 2021-04-10 - Update 2

Plugins:
- Fixed the xmodel plugin to be able to play the HnS event again

Mod code:

- Changes the title for the "Hall of Fame" to explain that it's an "All time" leader-board 
- Fixed the display of the team icons on round end (Fixes https://github.com/PussTheCat-org/PussTheCat.org-Cod4x-KTK/issues/7 )
- Replaced the execution of "map_restart" with the cod4 default function
- Added a screen print when HnS can not start because the xmodel file is not written/read

# 2021-04-12 - Update 3

Additions:

- Added "none" as constant event to the event vote
- Added a fps check to avoid glitching through lolzor spawn protection
- Added a dvar check for the version on loadscreen

Enhancements:

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

# 2021-04-12

Fixes:

- Remove the all the textures (including concrete/sand textures) that were replaced with a grass texture (Fixes https://github.com/PussTheCat-org/PussTheCat.org-Cod4x-KTK/issues/16 )

# 2021-04-14

Fixes:

- Remove 23 textures that affected the maps because they replaced stuff they weren't supposed to (Fixes https://github.com/PussTheCat-org/PussTheCat.org-Cod4x-KTK/issues/27 and https://github.com/PussTheCat-org/PussTheCat.org-Cod4x-KTK/issues/28 )

# 2021-04-15 - Update 4

Additions:

- Adminmenu has a new popup page for server changes
- Admins can now noclip (used for debuging - don't abuse it!)
- Added a dvar to enable/disable the fast-fire/weaponswitch detection
- Added separated skill dvars for assassins and guards
- HnS has now an instruction hud in upper left corner

Enhancements:

- Adminmenu now has all players on one page
- FovScale setting added more values
- Removed the last Update Date from the Loadscreen
- Killstreak icons moved when the lagometer is enabled
- Antiglitch triggers will no longer destroy RC-Toys
- Suicide will now first explodes RC-Toys (so you need to suicide twice to die)
- Changed the fast-fire/weaponswitch detection back to 300 instead of 500
- Changed the fake lag detection so it has a short delay before triggering
- Auto map rotation when no players are online will now use bot maps when there are any in the map rotation
- Adminmenu will now send less commands from server to client
- Speed up the spawn helicopter and parachute

Fixes:
- Fixed the fast fire of bots
- Fixed the bot sprint (untested)

---

The Mod.ff has changed because of those changes:

- Adminmenu has a new popup page for server changes
- Adminmenu now has all players on one page
- FovScale setting added more values
- Removed the last Update Date from the Loadscreen
- Killstreak icons moved when the lagometer is enabled

# 2021-04-16 - Update 5

Enhancements:

- Make the Juggernaut health bonus different for each team
- Update some internal documentations
- Added the enemy name display to the anti-dvar-dump list (the list of dvar that's enforced by the mod and can't be changed on clients)

Fixes:

- Forcing enemy name display to 0 (disabled) when event is HnS
- Fixed the noclip function not always giving godmod
- Fixed the mod executing "cg_fov 0" for no reason when connecting (the value wasn't a supported value so this didn't do anything other than display an error in the console)

# 2021-04-22 - Update 6

Additions:
- Added the M40A3 to the assassins
- Removed the collision for weapon boxes so bots can walk through
- Added a golden texture for the new weaponbox (no collision)
- mp_bubba now supports bots (untested)
- Nade cooking removed to avoid suicide

Enhancements:

- Removed the FPS check
- Throwing knife speed increased
- Changed the display name for event "none" to "None (Standard KTK)"
- Forced the team switch variable when a player switches team (should fix the no weapon for guards in dog event)
- Tried to make the bots sprint (but i think that still does not work)
- Admin Menu has now custom buttons, no defaut CoD4 buttons (used to display all players on one page)
- Admin Menu now shows which player will be punished
- Admin Menu now contains traitor event
- Minimum player set to 3 for the traitor event 

Fixes:
- Zombie event: Fix the green knife that followed the guardians 
- Fixed mp_bubba
- Fixed the empty map rotation that bot maps are prefered (had a typo in the array)

---

Mod.ff and z_v18_2.iwd have changed because of those changes:

Mod.ff:
- Admin Menu has now custom buttons, no defaut CoD4 buttons (used to display all players on one page)
- Admin Menu now shows which player will be punished
- Admin Menu now contains traitor event

IWD:
- Added a golden texture for the new weaponbox (no collision)
- Added the M40A3 to the R700 weapon file
- Throwing knife speed increased
- Nade cooking removed to avoid suicide

# 2021-04-22 - Update 6 - Hotfix 1

Enhancements:

- Change transparent weapon box from gold to normal color
- Remove a king model that was only used by Viking

Fixes:

- Fix the server name having characters removed when the round changed
- Zombie event: Fix the model instead of the script to fix the knife following the guardians
- Fix the VIPs functions not working with an 8 character GUID
- Fix the VIPs self revive message
- Fix the VIPs RPG getting a new rocket at every weapon upgrade

# 2021-04-23 - Update 6 - Hotfix 2

Additions:

- Added a new dvar to control if the bots can revive or not

Enhancements:

- Cleaned the 'rotate empty map' script
- Changed the 'rotate empty map' script so it will fall back to normal ktk before the map switch

Fixes:

- Fixed the self revive for VIPs

# 2021-04-25 - Update 7

Changelog:

Additions:

- Added a new killstreak setting to separate the rc car from the rc helicopter
- Added a new setting to separate vip xp multiplier from normal xp multiplier
- Added a new setting to define for how long the main assassin gets full ammo for the explosive crossbow (team size)
- Added a votesystem to allow players to vote for an event or map switch, when the minplayer amount is not reached but there are no bots to play with
- Added a radius trigger around the rc helicopter to make it easier to hit it (untested - Viking thinks triggers spawned by script do not detect damage impacts)
- Added different buttons for RC Heli and RC Car in hardpoint menu

Fixes:

- Fixed the bot self revive
- Fixed the bots reviving others even if the number of players is lower than the minimum in config
- Alien event: Fixed the invisible viewhands, when an alien becomes a guard
- Fixed the empty rotatemap when no maps in rotation
- Fix the points counter at the bottom left

The Mod.ff has changed because of this change:

- Added different buttons for RC Heli and RC Car in hardpoint menu

# 2021-04-28 - Update 7 - Hotfix 1

Additions:

- Add a setting to make the King kills not switch the assassins bots when there are X guardians bots already

Enhancements:

- Votesystem now shows results (top 3)

Fixes:
- cg_fov and cg_fovscale will not reset anymore when the change is not done through the settings menu of ktk

The Mod.ff has changed because of this change:

- cg_fov and cg_fovscale will not reset anymore when the change is not done through the settings menu of ktk

# 2021-04-30 - Update 7 - Hotfix 2

Additions:

- Added a new shellshock (screen shaking) effect
- Added a shellshock (screen shaking) to players on the ground to make it a bit harder to aim (and feel like pain)
- Added a debug message to the helicopter script to backtrace the big console error for maps that come without a helicopter support (but the mod creates a helipath)

Enhancements:

- Changed the view of the bots when climbing ladders to force them to climb up/down no matter how far away the next waypoint is
- Reduced the var usage in the Knifeassisst script

The Mod.ff has changed because of this change:

- Added a new shellshock

# 2021-05-08 - Update 8

Additions:

- Main menu displays song info
- Main menu now has a button to read credits and intructions about events
- Added a new admin cmd to freeze players (not in admin menu) (was used it to debug javelin final killcam - made it easier to kill a bot when he is stuck at a car position)

Enhancements:

- L.K.S. event will now show the last alive king as winner
- L.K.S. new comers have to wait for next round
- More helipath debugging lines added
- Final Killcam will now follow javelin missiles

Fixes:

- KtK will now detect when players leave during events and end the round when only 1 player is left (instead of endless wait for new players)
- Removed the bot debug message "direct"
- Fixed the reset of the killstreak, when last one was reached
- Fixed round start of "reverse ktk" event

Mod.ff has changed because of those changes:

- Main menu displays song info
- Main menu now has a button to read credits and intructions about events

z_v18_3.iwd was created because of of those changes:

-> contains the config for the song info in main menu
-> some weapon updates (removed some false sound references)
-> prepared sound folder for the event sounds that are in development by ninja

# 2021-06-08 - Update 9

Additions:

- Added a kick message when bots get replaced
- Added a kick message for players banned in config
- Added a dvar to enable/disable exploding cars in map
- L.K.S event will now end when all 'real' players were killed or disconnected
- Maps will now rotate when empty (or bots online only) for x minutes -> x is set in config "scr_mod_empty_time"

Enhancements:

- Cleanup of player variables on some files
- Javelin added to global weapon array
- Player guid is now shared instead of recaptured when needed
- rewrote the thermal script to use less variables
- Updated readme & config file

Fixes:

- Fixed the thermal message display
- Fixed the riotshield button text when it's unlocked
- fixed a rare killcam crash
- Fixed the riotshield damage detection
- Fixed crash when event "lastkingstanding" was stopped through admin menu
- Fixed the map display for the menu based mapvote

Mod.ff has changed because of those changes:

- Fixed the thermal message display
- Fixed the riotshield button text when it's unlocked
