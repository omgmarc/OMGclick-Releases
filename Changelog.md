# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

+ Monitoring market for shards
+ Automatic/Dynamic battle time calculation
+ Artifact rarity and (main) stats in Auto-Sell filter
+ Food champ swapping
+ Support for BlueStacks and other clients

## [3.2.0] - 2020-04-29

### Added

+ OSD to display status messages
+ Added all remaining dungeons, potions keeps, and campaign chapters to detection library

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
