# SCS Mod Manager v1.0.1

Maintenance release for Mod Manager and Ferry Editor.

- Mod Manager now explains when external profile changes block Apply. Recheck
  keeps the proposed order and opens a fresh review; Reload discards the proposal.
- Saved Configurations and Backup History have larger tables, separated action
  bars and better resizing, with scrolling for smaller windows.
- Ferry Editor adds **Recheck saved routes** to recover drafts after source
  refreshes without recreating routes or losing their values. Apply explains stale
  drafts, unsaved values, work in progress and unverifiable providers separately.
- Unrelated, fully parsed ferry catalog warnings do not block supported routes.
  Unknown providers that might contain conflicting definitions still block
  publishing; no missing routes are invented.
- Advanced expert export can create a standalone patch for a supported selected
  new ferry connection after explicit compatibility acknowledgment. It never
  installs or activates uncertain output. Protected source contents stay untouched.
- Ferry lookup avoids unrelated HashFS directory failures; stored HashFS v2
  tables are supported, with malformed metadata still rejected.

Existing profiles, settings, configurations and Ferry Editor JSON remain
compatible. Package installation and profile activation retain separate reviews,
automatic profile checkpoints, concurrency checks and the game-closed requirement.
Steam itself may remain running. Exact priorities and missing references are preserved.

The publisher confirmed that the expert-exported Bogorodskoje → Moskalvo Sak route
(64 / 621 minutes / 300 km) works in ETS2. This confirms that route only; it does
not guarantee compatibility with other routes or unreadable map sources. Expert
patches remain explicitly unverified and are never installed or activated automatically.
Other in-game behavior and Steam synchronization require the user's own checks.

Windows x64 portable distribution with bundled .NET 10/WPF. Stable builds use the
official Abysimo/SCSModManager-Releases update source. Development builds have
updates disabled. The public v1.0.0 release is unchanged.
