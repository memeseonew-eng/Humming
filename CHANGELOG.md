# Changelog

User-facing changes to Humming's public releases.

## [0.1.0-beta.2](https://github.com/memeseonew-eng/Humming/releases/tag/v0.1.0-beta.2) - Release protection and privacy

- Added explicit application-use and resource-reuse terms, preserving third-party licenses and applicable legal exceptions.
- Added a plain-language account of local data, deliberate browser searches, backups and public issue reports.
- Obfuscated private implementation identifiers in Humming's core, Windows and filename-index libraries. UI bindings, settings contracts and native entry points remain compatible.
- Omitted Humming debugging symbols and source-location metadata from protected release builds.
- Added recursive distribution allowlists, pinned third-party notice hashes and checks for accidental personal paths, secret signatures and screenshot metadata.
- Kept offline operation, portable data, background On / Windows startup Off defaults, and manual updates.

These are modest copying deterrents and release checks, not encryption of local data or a promise of protection against all reverse engineering. Public beta.1 downloads are retired in favor of beta.2. Original artifacts are retained privately with unchanged bytes and checksums; previously downloaded copies are unaffected.

## [0.1.0-beta.1](releases/v0.1.0-beta.1.md) — First beta

### Added

- Independent Run in the background (default On) and Start with Windows (default Off) preferences, quiet sign-in launch, and removal of only this installed copy's startup registration on uninstall.

- Automatic local filename discovery across accessible fixed and removable drives, with a persistent index and background change monitoring while Humming is running.
- File-search status, pause/resume, excluded folders, file refresh, and index rebuild controls.
- Windows Setup alongside the portable ZIP, with per-user installed data and a separate portable data folder.

### Included

- A unified launcher for installed Start Menu apps, files, folders, saved shortcuts, websites, calculations, and built-in actions.
- Explicit Google search through the Web search button or `?` mode.
- Calculator results copied with Enter, and local paths copied with Ctrl+Shift+C.
- Favorites, frequency and recency ranking, aliases, and Korean name/initial-consonant matching.
- Configurable global shortcut, keyboard navigation, light/dark themes, reduced motion, and local history controls.
- Settings recovery backups and preservation of personal data during program updates.

### Beta notes

Windows 11 x64; runtime included. The app and Setup are unsigned. The initial scan is progressive and coverage depends on available local drives and permissions. Windows startup is opt-in. There is no file-content search or automatic updater.

See the [release notes](releases/v0.1.0-beta.1.md) for historical feature notes, data paths, keyboard shortcuts, and validation limits. Use the current beta.2 release for downloads. This public repository contains distribution material rather than application development history.