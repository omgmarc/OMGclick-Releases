# Frequently Asked Questions

**NOTE:** Certain issues such as failing to properly detect item rank, EXP boost state, or clicking a button can be attributed to an issue with Display Scaling. To troubleshoot, try setting your display scaling to 100% and see if the problem persists. If it goes away, then please include this information when submitting your bug report.

## Table of Contents

+ [Will I get I get banned for using OMGclick?](#will-i-get-banned-for-using-omgclick)
+ [My anti-virus said your program contains a virus/trojan. Is this safe?](#my-anti-virus-said-your-program-contains-a-virustrojan-is-this-safe)
+ [Where is the source code?](#where-is-the-source-code)
+ [My mouse is stuck. How do I regain control of it?](#my-mouse-is-stuck-how-do-i-regain-control-of-it)
+ [Why does my game window keep getting resized?](#why-does-my-game-window-keep-getting-resized)
+ [I'm playing in fullscreen mode, why doesn't OMGclick work?](#im-playing-in-fullscreen-mode-why-doesnt-omgclick-work)
+ [It resized my game, but it's not doing anything after that.](#It-resized-my-game,-but-it's-not-doing-anything-after-that.)
+ [My game crashed, so I had to restart it. Why isn't OMGclick working anymore?](#my-game-crashed-so-i-had-to-restart-it-why-isnt-omgclick-working-anymore)
+ [I set OMGclick to grind EXP overnight, but when I woke up, there was still a lot of energy left over (more than my energy cap), and my champs didn't gain much EXP. What caused this?](#i-set-omgclick-to-grind-exp-overnight-but-when-i-woke-up-there-was-still-a-lot-of-energy-left-over-more-than-my-energy-cap-and-my-champs-didnt-gain-much-exp-what-caused-this)
+ [After minimizing the game, the window looks all glitchy. Is this from OMGclick?](#after-minimizing-the-game-the-window-looks-all-glitchy-is-this-from-omgclick)
+ [OMGclick sold (or kept) an artifact that it wasn't supposed to. How do I fix this?](#omgclick-sold-(or-kept)-an-artifact-that-it-wasn't-supposed-to.-how-do-i-fix-this?)
+ [OMGclick said it couldn't identify something. What do I do?](#omgclick-said-it-couldnt-identify-something-what-do-i-do)
+ [Where do I find the link to Discord?](#where-do-i-find-the-link-to-discord)
+ [How do I get the latest version?](#how-do-i-get-the-latest-version)
+ [How do I use OMGclick with only "X number" of clients while I manually handle "Y number" of clients?](#how-do-i-use-omgclick-with-only-"x-number"-of-clients-while-i-manually-handle-"y-number"-of-clients)

## Will I get banned for using OMGclick?
The simple answer is, "That's not likely." The proper answer, however, follows...

The only language in Plarium's [Terms of Use](https://plarium.com/en/terms-of-use/) that pertains to this matter states that you are not allowed to do the following:
```
decipher, decompile, disassemble, reverse engineer, or otherwise attempt to derive any code or underlying ideas or algorithms of any part of the Service, including any Service available on or through Third-Party Platforms;
```
This program does none of those things, nor have I as its author performed any of those actions during the development of this program. It's also common knowledge (or so we've been led to believe, anyway) that Plarium is "OK with autoclickers." Though I have yet to see any citation on this, their Terms of Use does not contradict that statement. Along with my earlier statement, that indicates to me that end-users of OMGclick are **NOT** in violation of Plarium's Terms of Use. That said, Plarium's Terms of Use *is* subject to change at any time, which would then be communicated to users via in-game announcement, email, or other form of communication. Those changes will then go into effect after five (5) days have passed. Should any change deem the use of this program explicity in violation of Plarium's Terms of Use, users will be advised against using it. Responsibility for any continued use of this program beyond that will be placed solely on the end-user.

I should also point out that I am well aware of programs similar to OMGclick; however, some of them are different in that they do in fact explicitly violate Plarium's Terms of Use. Though there are no active anti-cheat measures in place (e.g. something like BattlEye, VAC, or TruePlay) within the game client, that does not necessarily mean your account is safe. Should Plarium ever decide to, they are well within their rights to ban users of said programs. Again, at the time of this writing, OMGclick and its users do NOT violate Plarium's Terms of Use as it is currently defined.

## My anti-virus said your program contains a virus/trojan. Is this safe?
Many (not all) anti-virus programs will be triggered with a false positive depending on what their definitions files qualify as malware. Until I implement the ability for users to check for updates from within OMGclick, the only thing the program does aside from moving your mouse cursor and performing clicks as needed, is it creates folders and files as it needs (e.g. its images and screenshots folders, its config file, and any screenshots when enabled). False positives might also be triggered by the compression used in creating the EXE from the original AHK script. Submitting my program to every Anti-Virus company to have it cleared by them is simply not a feasible option. In any case, these can be safely ignored.

I have submitted my software to Windows to have it cleared from the Windows 10 SmartScreen filter, but until that happens, you will need to manually allow it through.

Of course, if you're really worried about it you're also free to disregard everything I just said and not use OMGclick altogether. 

## Where is the source code?
For the time being, I have chosen to keep the source code private. I explain why here on [this Reddit post](https://www.reddit.com/r/RaidShadowLegends/comments/is4v4n/the_god_of_autoclickers_no_need_to_play_the_game/g5iwl9l/?utm_source=share&utm_medium=web2x&context=3). 

## My mouse is stuck. How do I regain control of it?
You can usually press `CTRL+ALT+DEL` and then open the Task Manager to regain control of your mouse. This was likely caused by an endless loop being triggered in the script somehow. In most cases, they tend to be random user inputs that conflict with something the script is trying to do (e.g. moving the mouse or clicking on a button). They're technically not bugs, but because they're hard to catch, they can often slip through testing. If you're able to reproduce the problem reliably, be sure to submit a bug report with all the details so that it can be patched.

## Why does my game window keep getting resized?
OMGclick resizes game client window to a particular size in order to "normalize" the size of UI elements. As such, it is also necessary to switch out of fullscreen mode (Fullscreen windowed mode is OK) when using OMGclick (at least until I figure out how to detect it and perform the resize as needed). After the window is resized, you're free to reposition wherever you prefer so long as no portion of the window is off-screen. While scanning, if it detects any change to the window size, OMGclick will again resize and reset the window position.

**NOTE:** Avoid attempting to reposition the game window while OMGclick is running with a short scan interval.

## I'm playing in fullscreen mode, why doesn't OMGclick work?
See above.

## It resized my game, but it's not doing anything after that.
This is likely due to you using a display scaling other than 100%. 

## My game crashed, so I had to restart it. Why isn't OMGclick working anymore?
OMGclick uses your game's Process ID (PID) as a unique identifier rather than relying on its window title in order to properly handle multiple clients. However, when relaunching a client that might have crashed, for example, you will need to manually trigger a rescan by clicking the [Reload] button. Also, if you launch additional clients, changing the number of clients setting will cause OMGclick to rescan all clients for new PIDs before initiating the next scan.

## I set OMGclick to grind EXP overnight, but when I woke up, there was still a lot of energy left over (more than my energy cap), and my champs didn't gain much EXP. What caused this?
If you have OMGclick check for the 2x EXP boost and it expires while grinding EXP, an alert pops up asking if you wish to continue without the EXP boost. OMGclick will wait up to 30 seconds for a response. If no response is given (e.g. because you're AFK), then it will default to a "No" response and halt the session. This was done to prevent users from "wasting" energy. If you want to make sure the program continues grinding EXP even when your EXP boost expires while you're AFK, make sure to disable the "Check for +100% EXP boost" option before going AFK.

## After minimizing the game, the window looks all glitchy. Is this from OMGclick?
No, this is a graphical bug related to the Unity player. It's a pitfall of the redrawing mechanism of the game client whenever it attempts to restore the game window. While this can affect users of high-end GPU's, it seems to be more prevalent on users of integrated graphics. If you're experiencing this often, you may want to stop using the "Minimize when not scanning" option.

## OMGclick sold (or kept) an artifact that it wasn't supposed to. How do I fix this?
In most cases, this isn't something you can fix directly. If you know exactly what the artifact was (set, rank, rarity, etc.), post a bug-report on Discord or the issue tracker. Ideally, enable the screenshots option while continuing to farm that particular dungeon. If you see it happen again, look in OMGclick's screenshots folder for that post-battle screen (they're timestamped for your convenience), and include it in your bug report.

## OMGclick said it couldn't identify something. What do I do?
If you saw this error message, then it also means a screenshot was automatically saved (even if screenshots are not enabled) of the unidentified item in the post-battle screen. Look for it in the screenshots folder wherever you have OMGclick located. Submit a bug report on Discord or create an issue on Github, and include the screenshot.

## Where do I find the link to Discord?
It's https://discord.gg/RBzHB5n, but if you can also find a link to it at https://getomgclick.com.

## How do I get the latest version?
The best way to stay notified of new versions is by [joining the Discord server](https://discord.gg/RBzHB5n), but you can always find the latest version on at https://getomgclick.com. I plan to eventually include a way to check for updates from within the program.

## How do I use OMGclick with only "X number" of clients while I manually handle "Y number" of clients?
**NOTE for users accustomed to older versions of OMGclick:** As of version 4.0.0, selection of game clients has changed from bottom up to a top down selection process to make it more intuitive for new users.

If you wish to run OMGclick with a different client count than are actually running (e.g. setting number of clients to 1 but having 2 running), just have the one(s) you want handled by OMGclick to be the ones most-recently active, then start OMGclick. After it captures all the intended game clients, you should be OK to go back to controlling the others manually.

If the above is too complicated, the alternative is to have only the clients you want controlled by OMGclick to be running, then start OMGclick. Once it's captured all the game clients, you're free to launch additional game clients. These new clients will not be handled by OMGclick.