# Best Ruler Stats (Configurable)
Made by mat1432 [Steam](https://steamcommunity.com/id/mat1432/) [GitHub](https://github.com/mat1432)

1.34.* ; This Mod Does Not Need to be Updated!

This Mod gives you a choice at the start of the game to configure your ruler stats boost. * *Can be changed at any time via a Decision!* *
It allows you to set a defined target for your ruler stats between **1 Point** and **15 Points**!

Updates your Ruler, Heir and Consort skill points! **Yes, both your Heir and Consort are updated!**

**This is without a doubt a cheat mod!**

Additionally, some major mods change the Defines for the Maximum Skill Points of your ruler; No need to worry!
I have included a [Template Feature](/Mod%20Template%20Codes.md) that configures this mod automatically! **It is hard-coded**; So:
All that is required is an update and your selected template will auto update your targeted stats when you click the decision.
If you find mods have changed their defines, or want me to add a new mod to the templates list; Please post in the Discussion (not comments).

NOTE: The mod can only raise your rulers stats to the highest the game allows (Normally 6)!
You can change that in the Defines if you want, but this mod DOES NOT EDIT THE DEFINES (For Compatability)

Here is another Version of this mod, that uses **On Actions** to SIGNIFICANTLY reduce end of month performance impact.
Do note, it is almost definately NOT compatible with major map mods! But should work on most of your nearly vanilla games.
If your mod uses these On Actions this mod is NOT compatible: on_new_monarch, on_new_heir, on_new_consort.

There are 2 types of operation: 'Normal' and 'Minimum'
- Normal (Default) = For each MP category: ADD Defined Points to each category up to the **Game Maximum**.
- Minimum = For each MP category: Use your **Defined Minimum** or **Game Maximum** (Whichever is lowest).
By default the mod will ADD points to each category up to the defined maximum.
Alternatively you can configure it to use your defined selection as a minimum (CANNOT be higher than the game Defines allows!)

## Example:
- Say your ruler is elected as a 1, 5, 4
- You have chosen a defined target of 4
- In this game, maximum possible stat is 6 (like normal)

After your ruler updates:
| Setting Type | Normal     | Minimum  |
| ---          | ---        | ---      |
| Outcome      | 5, 6, 6    | 4, 5, 4  |
| Difference   | +4, +1, +2 | +3, -, - |

### Another Example but with [Anbennar Expanded](https://steamcommunity.com/sharedfiles/filedetails/?id=2422633137):
- Say your ruler is elected as a 2, 8, 6
- You have chosen a defined target of 6
- In this game, maximum possible stat is 9 ([Anbennar Expanded](https://steamcommunity.com/sharedfiles/filedetails/?id=2422633137))

After your ruler updates:
| Setting Type | Normal     | Minimum  |
| ---          | ---        | ---      |
| Outcome      | 8, 9, 9    | 6, 8, 6  |
| Difference   | +6, +1, +3 | +4, -, - |

## This Mod is:
- **NOT Achievement Compatible! (Modifies the checksum)**
- But will work on an Ironman save.

## Supported Mod Templates List:
- Base Game (6 Max Skill)
- [Anbennar Expanded](https://steamcommunity.com/sharedfiles/filedetails/?id=2422633137) (9 Max Skill)

## Not Yet Asked Questions / Q&A
### Q: Multiplayer?
A: Yes
### Q: With [No Limits Nation Designer](https://steamcommunity.com/sharedfiles/filedetails/?id=1528959434) I can make a 50,50,50 ruler, can this mod do that?
A: Nope, Sorry Mate! The command change_<adm|dip|mil> will only ever bring their stats up to game maximum! (Found in Defines)
* If you want to edit the Defines for ruler stats, check the [Wiki](https://eu4.paradoxwikis.com/Defines), you are looking for RULER_MAX_SKILL under [NNationDesigner](https://eu4.paradoxwikis.com/Defines#NNationDesigner)!
### Q: Why is none of this done through the Defines?
A: If I modify the defines, then this mod will not work with any other major mod. Since it's supposed to be the configurable, incompatibility would defeat its purpose.
### Q: Why not just hardcode it to 15 from the start?
A: Then the hidden background event would fire every month and error every time. To keep log files down and help wih that little bit of performance, I suggest you honestly select the correct option.

## Install and Uninstall Compatibility:
### Forwards Compatability:
- Almost Guaranteed!
- The mod doesn't edit or replace any files, only adds files. It should be forwards compatible with every future update!
### Backwards Compatability:
- Limit is [Patch 1.23](https://eu4.paradoxwikis.com/Patch_1.23) (16 Nov 2017)
- I'm not entirely sure when each feature I use here was added but 1.23 is the absolute limit.
### Save Compatability:
- Should be safe for any active save game!

## AI
- **The AI will never use this mod or its features!**
- If a game is saved with any menu open, the AI will close it without changes.

Inspired by [Best Ruler Stats](https://steamcommunity.com/sharedfiles/filedetails/?id=625725145) by [Paragon](https://steamcommunity.com/id/paragonnnnnnn)

Check out my other Monarch Point Mod: [Greater National Focus](https://github.com/mat1432/greater_national_focus) ([Steam](https://steamcommunity.com/sharedfiles/filedetails/?id=2905801426))

[GitHub](/../../)
Licensed under the [GNU General Public License v3.0](/LICENSE)
