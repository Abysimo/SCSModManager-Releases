# SCS Mod Manager v1.0.4

Unofficial Mod Manager for ETS2 and ATS. Not affiliated with, endorsed or
sponsored by SCS Software. Published by Abysimo (Abysmo on gaming forums).

## Game Settings Editor

- Browse supported ETS2/ATS settings, including economy, fines and progression.
- Compare original vanilla, observed current mods, installed and custom values.
- Generate and install a separate settings .scs mod; update validated app-owned
  packages and optionally enable them after exact profile/load-order review.
- Compose current official game definition structure with safely compatible
  active-mod values, then apply your overrides last. Included files resolve using
  the actual active priority; generated private includes avoid unrelated overrides.
- Keep compatible non-UI values, report skipped unreadable sources and omitted
  obsolete declarations, and reject unsafe or ambiguous affected-file merges.
- Use clearer inputs, individual descriptions, initially collapsed file groups,
  separate Reset and Use vanilla actions, and readable Dark/Light tooltips that
  follow theme changes without restarting.

## Mod inventory improvements

- Last modification dates and sorting by name, source, state and date.
- Stable manifest-based names with bounded shared metadata caching.
- Show in Explorer selects the exact archive or mod directory.
- Inventory sorting does not change active profile priority.

## Safety and coverage

Existing checkpoints, source freshness, guarded profile activation and recovery
remain in place. New-package installation and profile activation are separate;
potentially loaded existing packages are not overwritten while the game runs.

The stock settings catalog covers the inspected **ETS2/ATS 1.61 family**. Skipping
an unreadable higher-priority provider does not prove the observed value matches
the game's runtime state or guarantee compatibility with the full mod collection.
Recheck after changing game versions or sources; earlier local-test intentions
may require explicit rebase, retaining their values.

The publisher confirmed sorting, editor/group behavior, settings package creation
and installation, tested ETS2 gameplay effects, exact Explorer selection and
tooltip readability. This does not establish every setting, third-party mod,
ATS gameplay scenario, Steam Cloud configuration or recovery failure case.

## Installation and updates

Extract the complete portable ZIP into a writable application folder and run
**SCSModManager.exe**. Keep its notices and licenses. Windows x64; .NET is bundled.
Existing official versions can update directly to the latest stable release.
Startup checks run in the background; download and installation require your action.

[Support and permissions](https://github.com/Abysimo/SCSModManager-Releases/discussions)
· [Bug reports](https://github.com/Abysimo/SCSModManager-Releases/issues)

Freeware, proprietary and closed-source; mandatory legal exceptions and
independent third-party licenses remain applicable. See the accompanying terms.
