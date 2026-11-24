# Wololoader Mods

The public mod index for the **Mod Hub** in [Wololoader](https://github.com/Vitrie32/wololoader)'s Scriptorium.
Scriptorium reads `index.json` from this repository and lets players browse, install, update and uninstall these mods.

## Mods

| Mod | Version | What it adds |
|---|---|---|
| Monklanians | 0.2 | A Briton-based civilization of tough, fast-walking monks (example civ). |
| Woodlanders | 0.1 | A Frankish forest people with fast lumberjacks, heavy axe riders and a custom unit (example civ). |

## Adding your mod

1. Zip your mod folder so the zip contains exactly one folder named like your mod (`MyMod/mod.json`, `MyMod/civs/...`).
2. Put the zip and an `icon.png` in `mods/<MyMod>/`.
3. Add an entry to `index.json` with `id`, `name`, `version`, `author`, `description`, `tags`, `icon`, `download`, `sha256` and `size` of the zip, `requires_wololoader`, `depends` and `updated`.
   The full format is in [MODHUB.md](https://github.com/Vitrie32/wololoader/blob/main/wololoader/docs/MODHUB.md).
4. Open a pull request.

Scriptorium checks the sha256 and size of every download and refuses zips with unsafe paths.
