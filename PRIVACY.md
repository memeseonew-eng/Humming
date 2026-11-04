# Humming privacy and local data

Applies to Humming 0.1.0-beta.2. Updated 2026-11-04.

## What stays on your computer

Humming searches local app shortcuts, saved targets and a filename index on your PC. The index stores file and folder names, paths and metadata needed for discovery and change tracking, including local drive information. It does not index file contents. Ordinary local search text is processed locally.

Preferences, saved shortcuts, favorites and successful-use history are stored in `settings.json`, with `settings.json.bak` for recovery. A filename cache is stored under `index/`. Transient web-search queries and calculator expressions are not saved as usage-history entries.

Portable copies keep data beside the executable in `data/`. Windows Setup uses `%LOCALAPPDATA%\Humming`. Updates and uninstall retain that installed data. A portable data folder and a private backup can contain sensitive paths and website targets. These files are not encrypted by Humming; protect access to your Windows account and backup storage.

## When a browser opens

Clicking Web search or entering `? query` prepares a Google search. Typing alone does not send it. Activating the result opens Google in your browser, where the query and normal browser/network information are handled under Google's and your browser's policies. Opening a website shortcut or URL similarly contacts that chosen site.

Local results can open other applications. Those applications have their own behavior and privacy policies.

## Accounts, telemetry and protection

This beta has no Humming account, analytics, advertising, cloud sync, automatic update service or remote license check. Code obfuscation runs during the release build and does not add tracking, device fingerprinting or a network dependency to the app.

The public distribution repository contains release information, demonstration screenshots and version metadata. It does not contain the private development history, a personal Humming profile or a computer's filename index.

## Controls and backups

Preferences lets you disable computer file search, pause indexing, exclude folders, rebuild the index and clear usage history. Pausing retains cached search results. Disabling or pausing is not secure deletion. Saved shortcuts are explicit and remain available independently of discovery exclusions.

For a private settings backup, quit Humming and copy the two settings files. The index is rebuildable and can be excluded. Keep backups private. Before sharing screenshots or issue reports, remove personal paths, filenames, queries, clipboard contents and credentials.

## Downloads and GitHub

GitHub hosts the public repository and downloads and handles access under its own policies. Downloading Humming or using GitHub issues is separate from local app operation. Public issues are visible to others; never attach a private project continuation archive, personal profile or index.

Project and feedback: https://github.com/memeseonew-eng/Humming
