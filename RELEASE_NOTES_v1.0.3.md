# SCS Mod Manager v1.0.3

This stable update improves the Ferry Editor's create, install and enable workflow.
The existing Mod Manager layout and v1.0.2 startup update notification are retained.

## Ferry Editor

- Create and install a ferry mod directly from saved route proposals. Select the
  exact directions to include, including reverse directions only when selected.
  Other saved proposals remain available and are not silently included.
- Review the selected routes and values before creating the package. When some
  active mod sources cannot be read, supported new routes with readable endpoints
  can proceed after explicit acknowledgment of uncertain compatibility.
- Generate and structurally validate the .scs package, then install it into the
  configured local mod folder without manually copying or renaming files.
- Preview, create and install a new package to an unused destination while ETS2
  or ATS is running. It stays inactive, with clear guidance and an **Enable mod**
  action. Different existing package bytes are never replaced while the game runs.
- After closing the game, enable the installed mod without rebuilding or
  reinstalling it. Review the exact load-order change before the existing guarded
  profile writer makes any change. Steam itself may remain open.
- Preserve package ownership, source/profile freshness checks, atomic installation,
  backups and recovery. Identical owned packages are reused without rewriting.
- Show specific localized failure explanations beside the workflow instead of
  hiding the reason behind a generic error banner.

## Compatibility and safety

Structural validation does not guarantee compatibility with unreadable map mods.
Unsafe edits or deletions of existing routes remain blocked where their original
definitions cannot be verified. Original third-party mod archives are not edited.
Profile activation always requires the corresponding game to be closed and an
explicit review; new installation does not change active profile membership.

The publisher manually exercised the updated local workflow and reports that it
appears to work. This is limited acceptance, not exhaustive testing of all routes,
map collections, games or Steam Cloud configurations. The earlier successful
Bogorodskoje → Moskalvo Sak gameplay test is a separate historical result.

## Updating

Existing official installations can update directly to the latest stable version;
no intermediate release is required. Update checks run in the background at normal
startup. Download and installation require your action. You can also use
Settings → About → Check for updates or extract the portable archive separately.

SCS Mod Manager is unofficial and is not affiliated with, endorsed or sponsored
by SCS Software. [Support](https://github.com/Abysimo/SCSModManager-Releases/discussions)
and [reproducible bug reports](https://github.com/Abysimo/SCSModManager-Releases/issues)
remain available in the official release repository.
