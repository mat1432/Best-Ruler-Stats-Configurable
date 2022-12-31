# Made by mat1432 (Steam) https://steamcommunity.com/id/mat1432/ or https://github.com/mat1432 (GitHub)

[b]1.34.* ; This Mod Does Not Need to be Updated![/b]

This Mod gives you a choice at the start of the game to configure your ruler stats boost. [i]Can be changed at any time via a Decision![/i]
It allows you to set a defined target for your ruler stats between [b]1 Point[/b] and [b]16 Points[/b]!

Updates your [b]Ruler[/b], [b]Heir[/b] AND [b]Consort[/b] skill points!

This Mod is completely dynamic and should be compatible with just about every major mod.

[b]This is a cheat mod![/b]

Additionally, some major mods change the Defines for the Maximum Skill Points of your ruler; No need to worry!
I have included a [url=https://github.com/mat1432/Best-Ruler-Stats-Configurable/blob/main/Mod%20Template%20Codes.md]Template Feature[/url] that configures this mod automatically! [b]It is hard-coded[/b]; So:
All that is required is an update and your selected template will auto update your targeted stats when you click the decision.

[i][u]If you find mods have changed their defines, or want me to add a new mod to the templates list; Please post in the Discussion (not comments).[/u][/i]


[i]This mod DOES NOT EDIT THE DEFINES (For Compatability)[/i]

There are 2 types of operation: 'Normal' and 'Minimum'
[list]
    [*]Normal (Default) = For each MP category: ADD Defined Points to each category up to the [b]Game Maximum[/b].
    [*]Minimum = For each MP category: Use your [b]Defined Minimum[/b] or [b]Game Maximum[/b] (Whichever is lowest).
[/list]
By default the mod will ADD points to each category up to the defined maximum.
Alternatively you can configure it to use your defined selection as a minimum (CANNOT be higher than the game Defines allows!)

[h2]Example:[/h2]
[olist]
    [*]Say your ruler is elected as a 1, 5, 4
    [*]You have chosen a defined target of 4
    [*][i]In this game, maximum possible stat is 6 (like normal)[/i]
[/olist]
After your ruler updates:
[table]
    [tr]
        [th]Setting Type[/th]
        [th]Normal[/th]
        [th]Minimum[/th]
    [/tr]
    [tr]
        [td]Outcome[/td]
        [td]5, 6, 6[/td]
        [td]4, 5, 4[/td]
    [/tr]
    [tr]
        [td]Difference[/td]
        [td]+4, +1, +2[/td]
        [td]+3, -, -[/td]
    [/tr]
[/table]

[h2]This Mod is:[/h2]
[list]
    [*][b]NOT Achievement Compatible! (Modifies the checksum)[/b]
    [*]But will work on an Ironman save.
[/list]

[h2]Supported Mod Templates List:[/h2]
[list]
    [*]Base Game (6 Max Skill)
    [*][url=https://steamcommunity.com/sharedfiles/filedetails/?id=2422633137]Anbennar Expanded[/url] (9 Max Skill)
[/list]

[h2]Not Yet Asked Questions / Q&A[/h2]
[h3]Q: Multiplayer?[/h3]
A: Yes
[h3]Q: With [url=https://steamcommunity.com/sharedfiles/filedetails/?id=1528959434]No Limits Nation Designer[/url] I can make a 50,50,50 ruler, can this mod do that?[/h3]
A: Nope, Sorry Mate! The command change_<adm|dip|mil> will only ever bring their stats up to game maximum! (Found in Defines)
[i]If you want to edit the Defines for ruler stats, check the [url=https://eu4.paradoxwikis.com/Defines]Wiki[/url], you are looking for RULER_MAX_SKILL under [url=https://eu4.paradoxwikis.com/Defines#NNationDesigner]NNationDesigner[/url]![/i]
[h3]Q: Why is none of this done through the Defines?[/h3]
A: If I modify the defines, then this mod will not work with any other major mod. Since it's supposed to be the configurable, incompatibility would defeat its purpose.
[h3]Q: Why not just hardcode it to 15 from the start?[/h3]
A: Then the hidden background event would fire every month and error every time. To keep log files down and help wih that little bit of performance, I suggest you honestly select the correct option.

[h2]Install and Uninstall Compatibility:[/h2]
[h3]Forwards Compatability:[/h3]
[list]
    [*]Almost Guaranteed!
    [*]The mod doesn't edit or replace any files, only adds files. It should be forwards compatible with every future update!
[/list]
[h3]Backwards Compatability:[/h3]
[list]
    [*]Limit is [url=https://eu4.paradoxwikis.com/Patch_1.23]Patch 1.23[/url] (16 Nov 2017)
    [*]I'm not entirely sure when each feature I use here was added but 1.23 is the absolute limit.
[/list]
[h3]Save Compatability:[/h3]
[list]
    [*]Should be safe for any active save game!
[/list]

[h2]AI[/h2]
[list]
    [*][b]The AI will never use this mod or its features![/b]
    [*]If a game is saved with any menu open, the AI will close it without changes.
[/list]

Inspired by [url=https://steamcommunity.com/sharedfiles/filedetails/?id=625725145]Best Ruler Stats[/url] by [url=https://steamcommunity.com/id/paragonnnnnnn]Paragon[/url]

Check out my other Monarch Point Mod [url=https://steamcommunity.com/sharedfiles/filedetails/?id=2905801426]Greater National Focus[/url]

[url=https://github.com/mat1432/Best-Ruler-Stats-Configurable]GitHub Repository[/url]
Licensed under the [url=https://github.com/mat1432/Best-Ruler-Stats-Configurable/blob/main/LICENSE]GNU General Public License v3.0[/url]
