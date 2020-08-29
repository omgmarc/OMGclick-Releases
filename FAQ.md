# Frequently Asked Questions

**NOTE:** Certain issues such as failing to properly detect item rank, EXP boost state, or clicking a button can be attributed to an issue with Display Scaling. To troubleshoot, try setting your display scaling to 100% and see if the problem persists. If it goes away, then please include this information when submitting your bug report.

## Table of Contents

+ [My anti-virus said your program contains a virus/trojan. Is this safe?](#my-anti-virus-said-your-program-contains-a-virustrojan-is-this-safe)
+ [How do I use the "Block User Input" option?](#how-do-i-use-the-block-user-input-option)
+ [My mouse is stuck. How do I regain control of it?](#my-mouse-is-stuck-how-do-i-regain-control-of-it)
+ [Why does my game window keep getting resized?](#why-does-my-game-window-keep-getting-resized)
+ [I'm playing in fullscreen mode, why doesn't OMGclick work?](#im-playing-in-fullscreen-mode-why-doesnt-omgclick-work)
+ [My game crashed, so I had to restart it. Why isn't OMGclick working anymore?](#my-game-crashed-so-i-had-to-restart-it-why-isnt-omgclick-working-anymore)
+ [I set OMGclick to grind EXP overnight, but when I woke up, there was still a lot of energy left over (more than my energy cap), and my champs didn't gain much EXP. What caused this?](#i-set-omgclick-to-grind-exp-overnight-but-when-i-woke-up-there-was-still-a-lot-of-energy-left-over-more-than-my-energy-cap-and-my-champs-didnt-gain-much-exp-what-caused-this)
+ [After minimizing the game, the window looks all glitchy. Is this from OMGclick?](#after-minimizing-the-game-the-window-looks-all-glitchy-is-this-from-omgclick)
+ [OMGclick sold a Rank "X" artifact, but it was set to NOT sell it. How do I fix this?](#omgclick-sold-a-rank-x-artifact-but-it-was-set-to-not-sell-it-how-do-i-fix-this)
+ [OMGclick said it couldn't identify something. What do I do?](#omgclick-said-it-couldnt-identify-something-what-do-i-do)
+ [Where do I find the link to Discord?](#where-do-i-find-the-link-to-discord)
+ [How do I get the latest version?](#how-do-i-get-the-latest-version)
+ [How do I use OMGclick with only "X number" of clients while I manually handle "Y number" of clients?](#how-do-i-use-omgclick-with-only-x-number-of-clients-while-i-manually-handle-y-number-of-clients)

## My anti-virus said your program contains a virus/trojan. Is this safe?
Many (not all) anti-virus programs will be triggered with a false positive depending on what their definitions files qualify as malware. Until I implement the ability for users to check for updates from within program, the only things OMGclick does aside from moving your mouse cursor and performing clicks as needed, are it creates folders and files as it needs (e.g. its images and screenshots folders, its config file, and any screenshots when enabled). False positives might also be triggered by the compression used in creating the EXE from the original AHK script. Submitting my program to every Anti-Virus company to have it cleared by them is simply not a feasible option. In any case, these can be safely ignored. Of course, if you're really worried about it you're also free to disregard everything I just said and not use OMGclick altogether. 

## How do I use the "Block User Input" option?
You will need to launch OMGclick with the "Run as admin..." option. If it's already running, you can also just click on the little shield icon to reload OMGclick as admin.

## My mouse is stuck. How do I regain control of it?
If the "Block User Input" option is enabled, all user input, including mouse inputs, are blocked when OMGclick needs to do something. Should you encounter an issue where the program hangs up (e.g. it get stucks in a loop during auto-sell) thus blocking you from doing anything about it, press CTRL+ALT+DEL then click on Cancel (or open the task manager). This will break the lockout, and you should be able to stop/reload OMGclick. Do note that when this occurs, it's important to submit a bug report describing what you might have been doing when it happened.

## Why does my game window keep getting resized?
OMGclick resizes (and repositions) game client windows to a particular size. As such, it is necessary to switch out of fullscreen mode (Fullscreen windowed mode is OK) when using OMGclick (at least until I figure out how to detect it and perform the resize as needed). After the window is resized, you're free to reposition wherever you prefer so long as no portion of the window is off-screen. While scanning, if it detects any change to the window size, OMGclick will again resize and reset the window position.

## I'm playing in fullscreen mode, why doesn't OMGclick work?
See above.

## My game crashed, so I had to restart it. Why isn't OMGclick working anymore?
OMGclick uses your game's Process ID (PID) as a unique identifier rather than relying on its window title in order to properly handle multiple clients. However, when relaunching a client that might have crashed, for example, you will need to manually trigger a PID rescan by clicking the [Reload] button. Also, if you launch additional clients, changing the number of clients setting will cause OMGclick to rescan all clients for new PIDs before initiating the next scan.

## I set OMGclick to grind EXP overnight, but when I woke up, there was still a lot of energy left over (more than my energy cap), and my champs didn't gain much EXP. What caused this?
If you have OMGclick check for the 2x EXP boost and it expires while grinding EXP, an alert pops up asking if you wish to continue without the EXP boost. OMGclick will wait up to 30 seconds for a response. If no response is given (e.g. because you're AFK), then it will default to a "No" response and halt the session. This was done to prevent users from "wasting" energy. If you want to make sure the program continues grinding EXP even when your EXP boost expires while you're AFK, make sure to disable the "Check for +100% EXP boost" option before going AFK.

## After minimizing the game, the window looks all glitchy. Is this from OMGclick?
No, this is a graphical bug related to the Unity player. It's a pitfall of the redrawing mechanism of the game client whenever it attempts to restore the game window. While this can affect users of high-end GPU's, it seems to be more prevalent on users of integrated graphics. If you're experiencing this often, you may want to stop using the "Minimize when not scanning" option.

## OMGclick sold a Rank "X" artifact, but it was set to NOT sell it. How do I fix this?
In most cases, this isn't something you can fix directly. If you know exactly what the artifact was (set and rank), post a bug-report on Discord or create a new issue on Github. Ideally, enable the screenshots option while continuing to farm that particular dungeon. If you see it happen again, look in OMGclicks screenshots folder for that post-battle screen (they're datetimestamped for your convenience), and include it in your bug report.

## OMGclick said it couldn't identify something. What do I do?
If you saw this error message, then it also means a screenshot was automatically taken (even if screenshots are not enabled) of the unidentified item in the post-battle screen. Look for it in the screenshots folder wherever you have OMGclick located. Submit a bug report on Discord or create an issue on Github, and include the screenshot.

## Where do I find the link to Discord?
It's https://discord.gg/RBzHB5n, but if you can also find a link to from within OMGclick.

## How do I get the latest version?
The best way to stay notified of new versions is by [joining the Discord server](https://discord.gg/RBzHB5n), but you can always [find the latest version on the distribution page](https://github.com/omgmarc/OMGclick-Releases)...at least until I figure out a reliable way to do so automatically from within OMGclick that doesn't trigger more anti-virus programs from reporting false positives.

## How do I use OMGclick with only "X number" of clients while I manually handle "Y number" of clients?
When using OMGclick with multiple clients, clients are initially processed from the bottom up. If you wish to run OMGclick with a different client count than are actually running (e.g. setting number of clients to 1 but having 2 running), make sure that the one(s) you want OMGclick to "ignore" are the ones most-recently active. So in the previously-mentioned example, the one to be ignored would either be currently active (selected) or have been the most-recently active before switching to some other window that's NOT the client you wish to be scanned.
