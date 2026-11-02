# Azeroth Survivors Save Editor v1.5.6

**[Open the editor](https://yssadora.github.io/azeroth-survivors-editor/)** · [Source code](https://github.com/yssadora/azeroth-survivors-editor)

A free, unofficial browser-based save editor for **Azeroth Survivors**. Import a `.sav` file, edit your save, and download a modified `.sav` file. Processing happens locally in your browser.

## What changed in v1.5.6

- **Achievement Unlocker:** Add an achievement unlocker. You can either unlock all achievements at once or individually. Also locks the Scarab and other champion achievements with a warning to clear the zone first with the zone manager for the specific class.


## What changed in v1.5.5

- **Talent Tree Fixes:** Fix talent trees to match what is in game on current v0.138.0

## What changed in v1.5.4

- **Heroic Items/Star Items:** Added the ability to select heroic stars or tiers for each individual item without affecting the zone. Can add in increments of 1 up to 5 for each item.


## What changed in v1.5.3

- **Third specialization slot supported:** Save files with an active talent-spec index of `2` (seen in an October 21 browser export) are now synchronized when ranks are edited. The inactive builds are preserved.
- **Safer zone editing:** If a class lacks `open|`, `beat|`, and `unlock|` progression records, its zone controls are disabled instead of fabricating progression that the game may ignore or reset. Play the class in-game and export a fresh save first.
- **Clearer browser-game guidance:** Updated the compatibility notice using a player's comparative test: the **same modified save worked in Chrome and the downloaded game but reverted after a run in Firefox**. This suggests browser-specific game persistence behavior; the underlying Firefox cause remains unconfirmed.
- **Existing protections retained:** Verification of the encrypted export, talent XP/ranks, specialization synchronization, equipment, and preservation of unrelated Codex/character/achievement records.

## Browser game vs. downloaded game

The reported Firefox problem happens **in the browser version of the game**, not necessarily in the web-based save editor itself. If your game resets imported progression in Firefox, try playing and importing in Chrome or in the downloaded version.

**Important:** We cannot change how Firefox or the game's browser version stores/autosaves progress. v1.5.3 addresses editor bugs and provides better safeguards, **not a proven fix to the Firefox game's persistence issue**. One player's Chrome and PC success does not guarantee every browser or game build behaves the same.

## Features

- Interactive talent editing and XP for **9 classes**
- Equipment Armory with **498 pieces**, rarity tracking, search, and missing/collected filters
- Progression editing for **12 zones**, including prerequisite clearing
- Experimental permanent perk-reset restoration
- Unified export with a sticky Export Save button
- Class navigation, change indicators, and dark/light appearance

## How to use safely

1. Export a **fresh save from the game** you plan to use.
2. Keep that original somewhere safe. This editor can also download an untouched backup.
3. Import the fresh file at the [online editor](https://yssadora.github.io/azeroth-survivors-editor/), make your changes, and click **Export Save**.
4. Import the modified file into the game. **An in-game import replaces the full account save, including Codex discoveries; it does not merge newer progress.**
5. In the browser game, check immediately after import, then again after a completed run. If the game reverts, stop and restore your backup.

The editor validates what it writes; it cannot guarantee the game will persist those changes.

## Previous releases

- [v1.5.2 archive](https://yssadora.github.io/azeroth-survivors-editor/releases/v1.5.2.html)
- [v1.5.1 archive](https://yssadora.github.io/azeroth-survivors-editor/releases/v1.5.1.html)
- [v1.5 archive](https://yssadora.github.io/azeroth-survivors-editor/releases/v1.5.html)
- [v1.4 archive](https://yssadora.github.io/azeroth-survivors-editor/releases/v1.4.html)

## Credits

**Original Talent Editor:** Unknown community creator — credit to the original author.

**Armory, Zone Manager, integrations, and UI extensions:** Shilen.

This is an unofficial community tool and is not affiliated with the game's developers.
