# AGENTS.md — Cursor Themes Repository

## What this is

Personal collection of Windows cursor theme sets (`.cur` / `.ani` files). Each theme goes in its own folder with a Windows `.inf` installer.

## Current contents

- **mario-gant/** — Mario-themed cursor set by behelit/DeviantArt. Includes `install.inf`. See `readme.txt`.
- **Posy's Cursor/** — Posy's cursor set by Michiel de Boer. Includes `_install Posy Default.inf`. See `_info and instructions.txt`.
- **mario-gant.zip**, **All Posy's Cursors 1.4.zip** — source archives (don't edit; extract from the folder).

## Installing cursors

Right-click the `.inf` file → **Install**, then select the scheme in **Mouse Properties > Pointers**.

`.inf` files register the scheme under `HKCU\Control Panel\Cursors\Schemes` and copy cursors to `C:\Windows\Cursors\<FolderName>`.

## Agent's role

- Organize and map cursor themes.
- Create and fix `.inf` / `.ini` installers for each set.
- Help add new cursor themes consistently.
- Rename, restructure, or deduplicate as needed.

## Conventions

- No code, no build steps, no tests, no CI.
- Cursor files are binary — use existing `.cur`/`.ani` as templates if adding new ones.
- `.inf` syntax is the classic Windows Setup INF format (`[Version]`, `[DefaultInstall]`, `[Strings]`, etc.).
- Keep each theme self-contained in its own folder with its own `.inf`.
- Preserve original author credit files (readme, attributions) when adding themes.
