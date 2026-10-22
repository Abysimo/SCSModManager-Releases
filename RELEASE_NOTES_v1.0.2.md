# SCS Mod Manager 1.0.2

- Every normal startup performs one nonblocking background update check. Previous
  no-update or failed attempts do not suppress the next launch's check. There is
  no normal persistent cooldown, repeated navigation check or periodic polling.
- GitHub rate limits are handled without retry loops, respecting server retry/reset
  instructions. Network failures do not block normal startup or show intrusive dialogs.
- A prominent update notice appears above the workspace without opening Settings.
  Validated known-update notifications survive restarts and offline checks.
- Update and restart, Later and Release notes remain available. Downloads and
  installation require an explicit action and fresh official asset verification.
- Mod Manager uses the owner-approved compact lower panel, anchored to the bottom,
  while both mod lists expand into the remaining space.
- Selected-mod information uses a compact card with scrollable full descriptions;
  both configuration/history tables show about four to five rows with scrolling.

All v1.0.1 corrections are retained. Direct upgrades to the latest stable version
are supported; intermediate versions are not required. Windows x64 portable,
self-contained .NET 10/WPF. Existing settings and profile safety checks are preserved.
