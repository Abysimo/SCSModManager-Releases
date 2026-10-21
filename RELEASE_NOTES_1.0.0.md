# SCS Mod Manager v1.0.0 — first public stable release notes

## Included functionality

- Separate ETS2/ATS discovery and profile contexts, local and Workshop locations,
  Local/native Steam Cloud storage identification and profile-file modification times.
- Manual mod membership and priority editing, reviewed writes, exact checkpoints,
  safety history, named configurations and portable load-order import/export.
  Missing references retain their positions and have distinct selection indicators.
- Installed List/Tiles, bounded package metadata/thumbnails, full description
  information and description search.
- Selected-mod conflict evidence, comparison with matching installed game resources,
  a detailed difference viewer and selected original-file export.
- Current-game compatibility checks for selected mods, including sequential batches
  with per-mod outcomes and scoped cached reads.
- Ferry/train catalog for the selected profile's effective accessible sources;
  supported route edits with reviewed generated-patch/application steps.
- Same-game profile settings transfer for complete files or selected file groups,
  protected target state, review, backups and recovery. Separate game-wide graphics presets.
- Sixteen languages; Light, Dark and System appearance.
- Trusted public-source stable-update configuration, verified download/staging and
  recovery. User action is required to install/restart; local builds cannot update.

## Games and requirements

Euro Truck Simulator 2 and American Truck Simulator are supported as separate games.
Verification has used installations in the **1.61** series. Game/mod formats and
available resources affect individual operations; this is not a promise of support
for every older/future version or mod collection.

Windows x64 supported by the bundled .NET 10/WPF runtime; own installed game/data;
writable portable and user-data locations; adequate disk space for runtime extraction,
backups and staged operations. Internet is used for GitHub updates/support, not
required for ordinary local management. No Visual Studio, SDK or separate .NET
runtime install is required. Extract the complete ZIP and run **SCSModManager.exe**.
Keep the bundled legal documents/notices/licenses.

## Safety and known limitations

- Close the corresponding game before profile/settings writes. Steam may remain
  running; detected concurrent changes, uncertain identity or inaccessible data can
  cause safe refusal. Steam controls subsequent Cloud synchronization.
- No automatic correct-order solver, universal conflict repair or in-game guarantee.
  Unsupported/protected/corrupt/missing sources can limit results. Missing mods are
  not downloaded. Diagnostics reflect the selected scope and evidence.
- Profile settings transfer does not copy saves, progression or mod order. Controller
  bindings depend on devices. Profile copying does not reproduce graphics/weather
  mods, and graphics behavior remains inconclusive in the reported user scenario.
- Verification coverage varies by game, device and operation. Diagnostic checks
  and file verification do not guarantee in-game behavior or later Cloud sync.
  Retain independent backups and unresolved recovery evidence.
- Portable does not mean all data is stored beside the EXE. Preferences/caches/safety
  data use Windows LocalApplicationData; bundled native libraries may extract to a
  temporary runtime cache. Updates require a suitable writable separate app folder.

## License, identity and support

Freeware, closed-source, published as **Abysimo** (also **Abysmo**). The terms
permit free use, links, unchanged original-archive P2P and editorial use; restrict
unauthorized modification/repackaging/hosting/application resale, subject to mandatory
law and independently licensed components. Full terms and notices accompany the application.

Official releases: https://github.com/Abysimo/SCSModManager-Releases/releases

Support/permissions: https://github.com/Abysimo/SCSModManager-Releases/discussions

Bugs: https://github.com/Abysimo/SCSModManager-Releases/issues

Unofficial utility; not affiliated with, endorsed or sponsored by SCS Software.
No Valve/Steam or mod-author partnership is implied.

The [screenshot gallery](SCREENSHOTS.md) depicts the pre-release interface identified
in each image; it is not a screenshot set of the stable executable.
