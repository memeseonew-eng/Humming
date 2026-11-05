# Changelog

User-facing changes to Humming's public releases.

## [0.1.0-beta.6](https://github.com/memeseonew-eng/Humming/releases/tag/v0.1.0-beta.6) - Consistent hotkey and floating animation

- Fixed the global hotkey opening Humming without the floating-origin animation when the small floating icon was visible.
- Opening with Ctrl+Alt+Space now uses the same stable 260 ms circular expansion as clicking the floating icon.
- Retained the reverse animation on dismiss, search focus, custom image, docking, and accessible reduced-motion behavior.
- If the floating icon is disabled or not visible, the hotkey keeps its normal compact opening instead of inventing a floating origin.
- Kept beta.5 and earlier downloads unchanged for rollback.

## [0.1.0-beta.5](https://github.com/memeseonew-eng/Humming/releases/tag/v0.1.0-beta.5) - Sharper floating icon

- Fixed blurry default floating artwork caused by WPF loading the ICO's 16-pixel frame.
- Used a dedicated high-resolution image and better rendering in the button and Preferences.
- Fixed low-contrast text in the floating button's right-click menu with consistent light/dark styling and item hover states.
- Reworked the floating-to-launcher animation to paint within a fixed-size canvas instead of repeatedly resizing a transparent window, avoiding its visible jitter.
- Added a smooth reverse animation: dismissing the main launcher contracts the panel back to the floating circle.
- Respects reduced-motion/high-contrast settings and safely handles repeated opens, closes and interruptions.
- Preserved custom pictures, local privacy, keyboard focus, hotkeys, light/dark themes, and existing application/tray branding.
- Kept beta.4 available as a separate immutable download.

## [0.1.0-beta.4](https://github.com/memeseonew-eng/Humming/releases/tag/v0.1.0-beta.4) - Floating launcher

- Added an optional circular always-on-top launcher button that restores the search field with a click.
- Added dragging, edge docking and per-monitor position persistence.
- Added a right-click menu with Open, Preferences, Hide floating icon and Quit.
- Added a Preferences toggle, PNG/JPEG/Windows-supported WebP picker, live preview and built-in-image reset.
- The picture is converted locally to a 160-by-160 PNG without original metadata or source file path.
- Preserved existing global shortcut, dark/light modes, reduced motion, background/startup defaults and file search.

The new image remains local to personal settings and private backups; no user pictures are included in release downloads.

## [0.1.0-beta.3](https://github.com/memeseonew-eng/Humming/releases/tag/v0.1.0-beta.3) - Preferences theme fix

- Fixed a white background that could appear in the launcher's results area behind Preferences.
- Kept the disabled results surface in the active theme, including light and dark previews while Preferences is open.

Existing file search, explicit web search, background/startup defaults, privacy information and release protection continue in this maintenance beta.

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

See the [release notes](releases/v0.1.0-beta.1.md) for historical feature notes, data paths, keyboard shortcuts, and validation limits. Use the current beta release for downloads. This public repository contains distribution material rather than application development history.
