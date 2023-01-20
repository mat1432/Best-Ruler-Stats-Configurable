# Changelog
*Made by mat1432 [Steam](https://steamcommunity.com/id/mat1432/) [GitHub](https://github.com/mat1432/)*

## 1.0.2 (Not Yet Released)
* Bug Fix: Your Ruler can now get updated when they are the only claimant
* Recursive event options now show tooltip for reopening itself
* Rulers now update immediately upon exiting the main menu.
* Minor imporvements to use of colours in tooltips.
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