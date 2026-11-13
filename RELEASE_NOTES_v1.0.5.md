# SCS Mod Manager v1.0.5

Home now has a **Game Data Folder** setting for ETS2 and ATS. Select the
game-specific directory that holds your relocated profiles, mods, saves and
configuration files. The separate game installation setting still points to
the directory containing the game executable.

For example, if your game uses `-homedir "D:\TruckData"`, choose
`D:\TruckData\Euro Truck Simulator 2` or
`D:\TruckData\American Truck Simulator`. If you select the parent, the app
suggests the child for the selected game when it can identify it.

- Each game remembers its own data folder. **Restore default** returns that
  game to its folder under Windows Documents.
- Local profiles are rediscovered from the chosen folder. Steam Cloud profiles
  keep their Steam account and game identity.
- Local mods default to the `mod` subfolder. A separate local mod folder choice
  takes precedence.
- Folder selection updates application preferences. Game data stays in place.

The settings editor, mod management, diagnostics and profile protections from
v1.0.4 are included. Download the complete Windows x64 portable ZIP and extract
it to a writable directory, or use **Update and restart** in the app.
