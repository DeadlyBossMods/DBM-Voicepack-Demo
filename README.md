[![Build Status](https://github.com/DeadlyBossMods/DBM-MoP/workflows/CI/badge.svg)](https://github.com/DeadlyBossMods/DBM-MoP/actions?workflow=CI)
[![DeadlyBossMods on Discord](https://img.shields.io/badge/discord-DeadlyBossMods-738bd7.svg?style=flat)](https://discord.gg/DeadlyBossMods) 

[![Patreon](https://media.forgecdn.net/attachments/76/25/patreon-medium-button.png)](https://www.patreon.com/deadlybossmods)

Deadly Boss Mods: Voice Pack Demo
=================================

Requirements
------------
Before we start, there're some tools you need to have.

1. A decent text editor. (I use Notepad++ on Windows, Atom on Mac.)
2. Voice recorder tools which can output ogg files. Could be some software or a physical recorder, as long as you can turn your voices to ogg.

That's it. Easy, yeah?

How to create a voice pack
--------------------------

1. Copy the folder "DBM-VPDemo" from this pack into your workspace. By workspace I mean another folder location just in case you do something wrong and want to override the whole thing back to the initial status.

2. Make a decision of what name you want to use for your voice pack, and rename the folder to "DBM-VPYourPackName". It must start with "DBM-VP", case sensitive.

3. Go into the folder and rename the file "DBM-VPDemo.toc" to the same name you just named your folder, so "DBM-VPYourPackName.toc". DO NOT accidentally change the extension ".toc".

4. Now open the toc file you renamed in step 3 with your text editor.
    1. First 3 lines are addon version info. No need to touch them unless future wow big version releases.
    2. Line 3 is the title of your voice pack which will be showed in wow addons list. So simply change "Voicepack Demo" to "Voicepack YourPackName".
    3. Line 4 and 5 is Taiwanese and Chinese translations for the title. If you don't speak those languages just remove those 2 lines. Or if you're making for some other languages please add yours here.
    4. "RequiredDeps", "DefaultState" DO NOT TOUCH.
    5. Change "Author: Iceoven" to "Author: YourName".
    6. "Version", usually start from 1.0 (or 0.1 if still in alpha/beta status) and increase while your voicepack evolves. (Note: if you release on Curse, please bump this number everytime you make a release so that Curse client is aware.)
    7. "X-DBM-Voice", DO NOT TOUCH.
    8. "X-DBM-Voice-Name" is the name that appears in /dbm options for selection.
    9. "X-DBM-Voice-ShortName" should always match "YourPackName" after "DBM-VP". So in this example, it's the word "Demo" in "DBM-VPDemo".
    10. "X-DBM-Voice-Version" Might change with DBM version if required. Please follow the value in this demo every time we update.
    11. "X-DBM-Voice-HasCount" 1 means you have the "count" folder which has 1-11 .ogg files, otherwise 0.
  done.

5. Congrats, the only last thing left now is to record your ogg files. See [here](https://github.com/DeadlyBossMods/DBM-Voicepack-Demo/blob/master/DBM-VPDemo/!VoiceText.txt) for a list of the file names on the left and the words we used on the right.
    1. You may search through and find the ones you want to customize or simply record all of them and replace the existing ones.
    2. Advance usage: If you know Lua and addon development, you can just go into each DBM module and find those places where the voice file is called and understand better when it's triggered.
