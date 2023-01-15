# Best Ruler Stats (Configurable)
*Made by mat1432 [Steam](https://steamcommunity.com/id/mat1432/) [GitHub](https://github.com/mat1432/)*

<img src="/thumbnail.png" style="float:right;" />

**1.34.X ; This Mod Does Not Need to be Updated!**

Updates your **Ruler**, **Heir** and **Consort** skill points!

This Mod gives you a choice at the start of the game to configure your ruler stats boost. * *Can be changed at any time via a Decision!* *
It allows you to set a defined target for your ruler stats between **1 Point** and **16 Points**!
This means you can configure your ruler to have max stats with any mod that changes max ruler stats!

This Mod is completely dynamic and should be compatible with just about every major mod.

**This is a cheat mod!**

## How It Works
**This mod DOES NOT EDIT THE DEFINES (For Compatability)**

There are 2 types of operation: 'Normal' and 'Minimum'
- Normal (Default) = For each MP category: ADD Defined Points to each category up to the **Game Maximum**.
- Minimum = For each MP category: Raise each ruler stat up to the **Defined Minimum**; except unless it is already higher than your set minimum.

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

## Mod Templates
I have included a [Template Feature](https://github.com/mat1432/Best-Ruler-Stats-Configurable/blob/main/Mod%20Template%20Codes.md) that configures the selected stat target automatically.

**It is hard-coded**; So new additions or updating changes will require a new patch of this mod.
### Supported Mod Templates List
- Base Game (6 Max Skill)
- [Anbennar Expanded](https://steamcommunity.com/sharedfiles/filedetails/?id=2422633137) (9 Max Skill)

## Mod Compatability
### The Defines
* *This mod DOES NOT EDIT THE DEFINES* *

Reason being, is to ensure likely compatability with other mods.
#### If you want to edit the Defines
Check the [**Wiki**](https://eu4.paradoxwikis.com/Defines), you are looking for **RULER_MAX_SKILL** under [**NNationDesigner**](https://eu4.paradoxwikis.com/Defines#NNationDesigner)!
### On Actions
* *This mod does NOT use On Actions* *

Like above, to ensure likely compatability.

Though, I am considering adding a second vesion of this mod that uses strictly On Actions. (No guarantee)

The theory is it will boost performance (marginally) by only running its complex checks when Rulers ascend, heirs are born/elected and consorts are added. (AKA Event-based scripting)

## Not Yet Asked Questions / Q&A
### Q: Multiplayer?
A: Yes
### Q: With [No Limits Nation Designer](https://steamcommunity.com/sharedfiles/filedetails/?id=1528959434) I can make a 50,50,50 ruler, can this mod do that?
A: Nope, Sorry Mate! The command *change_<adm|dip|mil>* will only ever bring their stats up to game maximum! (Found in Defines)
### Q: Why not just hardcode it to 15 from the start?
A: Then the hidden background event would fire every month and error every time. To keep log files down and help wih that little bit of performance, I suggest you honestly select the correct option.

## Install and Uninstall Compatibility
### Forwards Compatability
- Almost Guaranteed!
- The mod doesn't edit or replace any files, only adds files. It should be forwards compatible with every future update!
### Backwards Compatability
- Limit is [Patch 1.23](https://eu4.paradoxwikis.com/Patch_1.23) (16 Nov 2017)
- I'm not entirely sure when each feature I use here was added but 1.23 is the absolute limit.
### Save Compatability
- Should be safe for any active save game!

## AI
- **The AI will never use this mod or its features!**
- If a game is saved with any menu open, the AI will close it without changes.

Inspired by [Best Ruler Stats](https://steamcommunity.com/sharedfiles/filedetails/?id=625725145) by [Paragon](https://steamcommunity.com/id/paragonnnnnnn)

Check out my other Monarch Point Mod: [Greater National Focus](https://github.com/mat1432/greater_national_focus) ([Steam](https://steamcommunity.com/sharedfiles/filedetails/?id=2905801426))

[GitHub Repository](https://github.com/mat1432/Best-Ruler-Stats-Configurable)
Licensed under the [GNU General Public License v3.0](https://github.com/mat1432/Best-Ruler-Stats-Configurable/blob/main/LICENSE)
