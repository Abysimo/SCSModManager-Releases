# SCS Mod Manager — privacy and data handling

SCS Mod Manager 1.0.0 — 21 October 2026.

Public publisher: **Abysimo**, also known as **Abysmo** on
gaming forums. Support and permission requests:
[GitHub Discussions](https://github.com/Abysimo/SCSModManager-Releases/discussions).
Reproducible bugs: [GitHub Issues](https://github.com/Abysimo/SCSModManager-Releases/issues).
Official releases: [SCSModManager-Releases](https://github.com/Abysimo/SCSModManager-Releases).
This describes application behavior. It is not a consent form and does not waive
data-protection rights.

## Local information and storage

SCS Mod Manager is a desktop utility. It discovers locally installed ETS2/ATS,
Steam libraries/accounts and profile locations, and reads profile identities,
storage type, modification times and active mod entries. Requested tools read
the selected mod/game resources and profile/configuration files they need.

Application state is stored under Windows LocalApplicationData, normally
`%LOCALAPPDATA%\SCSModManager`. Windows redirection/packaging may affect the physical
location. This state can include language/theme and game/profile/path selections,
mod configurations, requested-tool caches/metadata/path indexes, Ferry Editor and
Profile Manager records, diagnostic logs and update records.

Safety checkpoints can contain exact profile/configuration bytes and identifying
paths/account/profile information. Local storage is not an encrypted vault. A
user-selected export can contain mod orders, reports, configuration information or
original game/mod bytes, depending on the tool. Protect exports and backups using
your Windows account/storage controls; review them before sharing.

Confirmed editing operations write their selected targets or generated files;
discovery/preview is not a permission to apply edits. Steam Cloud storage here
means files resolved on your PC. Steam may subsequently synchronize changed files
under its own settings and policies; the application does not log in to Steam or
implement its own Steam Cloud service. User-selected network folders and operating
system services may also process files independently.

The portable EXE keeps bundled resources in the application. .NET can extract
native runtime libraries to its temporary bundle cache. An explicit update stages
downloaded application files/backups beside the portable installation and helper/
journal data under the app's `updates` storage; these are not profile migrations.

## Diagnostics and sharing

- General failure logs are local, rotating JSON records (four files, each bounded
  to approximately 64 KiB). They record time, application/game version, module,
  action/phase, exception type/error code and an application-owned summary. They
  deliberately exclude raw profile contents, arbitrary exception messages, stacks
  and detailed paths. They are still technical records, not a guarantee of anonymity.
- **Export diagnostics** writes a user-chosen local JSON file. The export retains
  selected technical fields and omits summaries, stacks and detailed Ferry logs.
  Exporting does not send the file to anyone.
- Detailed Ferry discovery logs are different: current/previous local reports can
  contain profile names/paths/hashes, game/mod source paths, identities, counts,
  failure reasons and exception messages. They are intended for targeted local
  investigation, not automatic transmission. Do not treat raw Ferry logs or profile
  checkpoints as anonymous. The general diagnostic export excludes them.

There is no app account/registration, advertising, usage analytics, telemetry or
automatic upload of diagnostics, profiles, saves or mods in the audited code.
If you choose to send a support file through a browser or another service, you
control that separate disclosure and the recipient/service's policies apply.
The official Discussions and Issues are public GitHub channels, not confidential
support intake. Posts, screenshots and attachments can be visible to others and
processed by GitHub and the maintainer. Remove personal information before posting;
do not upload raw profiles, saves, checkpoints or detailed logs without reviewing
them. The app does not automatically submit support requests or operate a separate
support-upload service. Use the official Discussions channel for support and
privacy-related questions about material you have voluntarily posted.

## GitHub requests

The verified official public repository is
[Abysimo/SCSModManager-Releases](https://github.com/Abysimo/SCSModManager-Releases),
GitHub repository ID **1427736746**. Its owner/name/numeric identity is pinned in
the trusted public-release build configuration. Local development builds retain
empty/disabled update authority and independently block update checking and
installation.

In an official stable build using that compiled-in source, the application
can check GitHub Releases asynchronously on startup, at most once per 24 hours
automatically. A manual check bypasses that interval. Version comparison and the
last-attempt timestamp are local. A check does not install an update; downloading/
installing requires the Update action, and release notes open in your browser only
on a click.

Application-owned update requests use HTTPS to `api.github.com`, with allowed
GitHub release-delivery redirects to `github.com`, `release-assets.githubusercontent.com`
and `objects.githubusercontent.com`. GitHub/delivery infrastructure receives the
network IP address and ordinary request information, including the product User-Agent,
time and requested public release/asset. The updater does not attach profile/mod
contents, local paths, Steam account identities or diagnostic logs to these requests.
It does not use your GitHub account or request a personal access token.

GitHub's handling of connection information is governed by its
[privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).
External browsers, Steam and Windows have their own behavior and policies. This
summary makes no promise to control their logging, retention or synchronization.

## Retention and control

General logs rotate and Ferry logs retain current/previous reports. Preferences,
configurations, checkpoints, caches, exports and failed-update recovery evidence
have their existing local lifecycles; there is no universal automatic erasure
deadline. No remote account is created for the application. Preserve pending
backup/recovery records until recovery is complete. Closing the app and removing
the portable folder does not delete separately stored application data or exports.
Review local files before removing them, because safety history may be needed.

Changes to application data handling will be reflected in this notice.
