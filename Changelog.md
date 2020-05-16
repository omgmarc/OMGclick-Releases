# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

+ Market Monitor to buy Shards when AFK (Coming in v4.0)
+ Automatic/Dynamic battle time calculation
+ Artifact rarity and flat stats filters for Auto-Sell (Coming in v4.0)
+ Food champ swapping (Coming in v4.0)
+ Support for BlueStacks and other clients
+ "Nexter" to automatically progress through (and optionally 3-star) campaign/dungeon stages
+ Indicator for how many runs have taken place

## [3.3.7] - 2020-05-15

Bugfix. Users should use this over older versions.

### Fixed

+ Energy restore not working with energy refill bottles from inbox for some users
+ Rank 6 accessories ID'd as Rank 5 in Spider's Den
+ Factions not ID'd for Spider's Den accessories for some users:
  + Banner Lords
  + Dark Elves
  + Demonspawn
  + Dwarves
  + High Elves
  + Knight Revenant
  + Lizardmen
  + Sacred Order
  + Skinwalkers
  + Undead Hordes

## [3.3.6] - 2020-05-14

Bugfix. Users should use this over older versions.

### Fixed

+ Getting stuck during Auto-Sell process
+ +100% EXP boost not properly detected for some users
+ Entering values directly into scan interval fields instead of using UP/DOWN buttons now updates interval properly (for next interval)

## [3.3.5] - 2020-05-13

Hotfix. This update not necessary unless your system is affected. See below for changes.

### Fixed

+ Users (particularly Windows 7 users) encountering unidentified Rank 4 and Rank 5 artifacts

## [3.3.4] - 2020-05-13

### Added

+ More information provided in status messages
+ Option to ignore max levels in dungeons without disabling the option for compaign runs

### Fixed

+ Rank 5's no longer ID'd as Rank 4's
+ Certain Avenging artifacts not being identified
+ Certain Stalwart artifacts not being identified
+ Certain Toxic artifacts not being identified

### Changed

+ Rebuilt the entire Auto-Sell routine for better reliability
+ Checking for max levels now accommodates all team sizes from 1 to 5 champs
+ Enabling screenshots will now capture non-artifact post-battle screens (e.g. shards, brews, champions, and any unidentified artifacts)
+ Auto-sell "star" ranks will display "text" ranks instead for versions before Windows 10.0.18300

## [3.3.3] - 2020-05-10

Hotfix. This update not necessary unless your system is affected. See below for changes.

### Fixed

+ Restore Energy affecting users with certain OS configurations.

## [3.3.2] - 2020-05-10

### Added

+ Link to new Discord server: go there to be notified of new releases and to discuss features, bugs, etc.
+ Support for Auto-Sell in Spider's Den
+ Option to always enable "Auto" combat mode
+ Option to always set combat to "x2" speed
+ Adjust wait time before starting next round (Range: 0-10 seconds)
+ Restore energy will now also use free refills when available

### Fixed

+ Restore energy now restores energy properly
+ Resolved more false positive identification of Rank 5 on Rank 4 artifacts

### Changed

+ Download link text
  - *PS: Thank you to those who have donated and suggested adding this option.*

## [3.3.1] - 2020-05-05

## Changed

+ Rank 1 and 2 artifacts marked for sale by default
+ Minimize window no longer on by default

### Fixed

+ Corrected SendMode switching
+ Typo causing first-run rank scans to fail 100% of the time

## [3.3.0] - 2020-05-05

### Added

+ Override auto-sell options to sell **EVERYTHING** from Ch. 12 (Brimstone Path)
+ Alternate (slower) clicking mode for those having issues with clicks not registering with standard click mode
+ Capture screenshots of auto-sell operations (sold and kept items)

### Changed

+ New GUI layout to better-accommodate DPI scaling users

### Removed

+ Monitor placement options removed to make way for using preferred window size/position option

### Fixed

+ Numerous bugs and detection faults. There might still be a few, so please report any.

## [3.2.1] - 2020-04-29

### Fixed

+ Not detecting Plarium Play clients anymore

## [3.2.0] - 2020-04-29

### Added

+ OSD to display status messages
+ All remaining dungeons, potions keeps, and campaign chapters to detection library
+ Provisions to support other client types underway...

### Changed

+ Auto-sell will now detect what level was run and detect artifacts accordingly
+ Refactoring of variables, methods, and subroutines for more consistency

### Fixed

+ Fixed range calculation in search fcn. (cause of major slowdowns)
+ Rank 4 artifact detection corrected

## [3.1.2] - 2020-04-26

### Added

+ Auto-sell dungeon artifacts

### Changed

+ Detection of dungeons is performed before campaign chapters to reduce detection times

### Fixed

+ Dungeon detection: The Dragon's Lair & Fire Knight's Castle are now properly detected and their respective artifact sets parsed accordingly

## [3.1.1] - 2020-04-25

### Added

+ This changelog file
+ Campaign Chapter Detection: referencing chapter name on post-battle screen
+ Assigned artifact sets to respective campaign chapter
+ Dragon's Lair & Fire Knight Dungeon Detection: referencing dungeon name on post-battle screen
+ Usage information now included in README

### Changed

+ Switched to GNU AFFERO GENERAL PUBLIC LICENSE
+ Updated header information to reflect new license
+ Added header information to all code files
+ Energy restore check is now done after [Replay] & [Edit Team] attempts
+ Updated artifact detection process in preparation for artifact-restriction feature

### Fixed

+ Energy restore now occurs immediately rather than waiting an entire interval


## [3.1.0] - 2020-0424

### Added

+ Run count limiter

## [3.0.0] - 2020-04-05

Codebase uploaded to GitHub

### Added

+ GUI

### Fixed

+ Broken variable references and other bug fixes

https://keepachangelog.com/en/1.0.0/
