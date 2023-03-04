# Changelog
*Made by mat1432 [Steam](https://steamcommunity.com/id/mat1432/) [GitHub](https://github.com/mat1432/)*

## 1.1.0
* The mod now automatically detects the maximum possible ruler stats.
* Collapsed ludicrous mode dynamically.
* Added options 100 to 200
* Added auto-detect max skill mechanic.
  * This is automatically used and is forced to run at game start replacing the default static template of 6.

## 1.0.3a
* Stat target now autocorrects itself to the game defines each time the hidden event fires.

## 1.0.3
* Bug Fix: Chosing a stat target of 10 now works correctly.
* Added selections 17 to 20.
* Added ludicrous mode; 0 to 100
  * *The button is likely temporary, I know how to improve this and collapse it dynamically, I just need time to develop the mod.*
  * Only if enabled:
    * This **will not** affect the background monthly **check** event performance.
    * This **will** affect the background monthly **change** event performance.
* Minor Bug Fix: Menu tooltips now show up on 'Detatch Template' button on the config menu
* Minor Bug Fix: Tooltip colours and intuitive language

## 1.0.2b
* Major Bug Fix: Localisation fixed, and mod loading issue fixed

## 1.0.2
**Localisation Broken***; see 1.0.2b.*
* Major Bug Fix: Your Ruler can now get updated when they are the only claimant
* Added Dynasty Icon and Admin Power Icon to prefix decisions and events
* Recursive event options now show tooltip for reopening itself
* Rulers now update immediately upon exiting the main menu.
* Combined both specific stat target menus
* Opening the menu for the first time via a decision now also configures itself for the 'Base Game Template' automatically.
* Minor imporvements to use of colours in tooltips.
* Minor Bug Fix: Removed tooltip 'detach from template' when changing template, and moved it to 'set stat target' when a template is already in use.
* Fixed typos
### Notes
* Ruler Bug Fix details:
  * When the game parses an empty argument (no argument) in a trigger, if it is the first character of a value, the game will throw an error and ignore the command.
  * This presented an opportunity to simplify the code. Hence, there are now:
    * six different change ruler effect scripts: **brs_update_ruler**, **brs_update_ruler_min**, **brs_update_heir**, **brs_update_heir_min**, **brs_update_consort**, and **brs_update_consort_min**; and
    * three different check ruler trigger scripts: **brs_check_ruler**, **brs_check_heir**, and **brs_check_consort**.

## 1.0.1d
* Refactored changing templates code

## 1.0.1c
* Fixed Customisable Localisation
* Fixed Templates not showing up

## 1.0.1b
* Credited Myself to my code
* Improved Mod Pages

## 1.0.1
* Updated Steam Workshop Page
* Updated descriptor

## 1.0.0
* Foundation of the mod.
* Added [GitHub Repository](https://github.com/mat1432/Best-Ruler-Stats-Configurable)
* Now licensed under the [GNU General Public License v3.0](https://github.com/mat1432/Best-Ruler-Stats-Configurable/blob/main/LICENSE)