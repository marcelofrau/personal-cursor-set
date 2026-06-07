# AGENTS.md — Cursor Themes Repository

## What this is

Personal collection of Windows cursor theme sets (`.cur` / `.ani` files). Each theme goes in its own folder with a Windows `.inf` installer.

## Current contents

| Folder | Theme | Source | Installer |
|--------|-------|--------|-----------|
| `mario-gant/` | Mario Gant | behelit / DeviantArt | `install.inf` |
| `Posy's Cursor/` | Posy's Cursor | Michiel de Boer | `_install Posy Default.inf` |
| `Bibata-Modern-Amber/` | Bibata Modern Amber | ful1e5 / GitHub | `install.inf` |
| `Bibata-Modern-Classic/` | Bibata Modern Classic | ful1e5 / GitHub | `install.inf` |
| `Bibata-Modern-Ice/` | Bibata Modern Ice | ful1e5 / GitHub | `install.inf` |
| `Windows-Cursor-Concept-v2.2/` | W11 Cursor Concept v2.2 | Jepri Creations / AMag1c | Per variant folder |
| `Bibata-Modern-Ice/` | Bibata Modern Ice | ful1e5 / GitHub | `install.inf` |
| `Windows-Cursor-Concept-v2.2/` | W11 Cursor Concept v2.2 | Jepri Creations / AMag1c | Per variant folder |
| `Yaru-Ubuntu/` | Yaru (Ubuntu) | csabika98 / GitHub | `install.inf` |
| `ctrlcat0xx-cursors/` | 31 themed packs | ctrlcat0xx / GitHub | `install.inf` per pack |

Source archives (`.zip`) go in `repos/`. Don't edit zip files; extract into theme folders.

## New theme checklist

1. Download source (zip or clone repo) into `repos/`
2. Extract cursor files into a new folder at root — name it descriptively
3. Verify or create `install.inf` (see existing ones as templates)
4. Preserve any readme/attribution/license files
5. Update this file and `README.md`
6. `git add -A && git commit -m "Add <ThemeName>" && git push`

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
