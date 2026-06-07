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
| `Yaru-Ubuntu/` | Yaru (Ubuntu) | csabika98 / GitHub | `install.inf` |
| `ctrlcat0xx-cursors/` | 31 themed packs | ctrlcat0xx / GitHub | `install.inf` per pack |
| `Capitaine-Cursors/` | Capitaine Cursors | keeferrourke / GitHub (r4) | `install.inf` |
| `Capitaine-Cursors-Variants/` | Capitaine Cursors (Colors) | sainnhe / GitHub (r5) | `Install.inf` per variant |
| `Apple-Cursor/` | Apple Cursor | ful1e5 / GitHub v2.0.1 | `install.inf` |
| `Apple-Cursor-White/` | Apple Cursor (White) | ful1e5 / GitHub v2.0.1 | `install.inf` |
| `macOS-Cursors-Sierra/` | macOS Cursors (Sierra+) | antiden / GitHub v0.5 | `Install.inf` per variant |
| `macOS-Cursors-ElCapitan/` | macOS Cursors (El Capitan) | antiden / GitHub v0.5 | `Install.inf` per variant |
| `DMZ-Black/` | DMZ-Black | Ubuntu package | `install.inf` (converted) |
| `DMZ-White/` | DMZ-White | Ubuntu package | `install.inf` (converted) |
| `Breeze/` | Breeze | KDE / Ubuntu package | `install.inf` (converted) |
| `Breeze-Snow/` | Breeze Snow (white) | KDE / Ubuntu package | `install.inf` (converted) |
| `ComixCursors-{Black,Blue,Green,Orange,Red}/` | ComixCursors (5 colors) | Ubuntu package | `install.inf` per color |
| `ComixCursors-Slim-{Black,Blue,Green,Orange,Red,White}/` | ComixCursors Slim (6 colors) | Ubuntu package | `install.inf` per variant |
| `ComixCursors-White/` | ComixCursors White | Ubuntu package | `install.inf` |
| `XCursors-Handhelds/` | Handhelds | xcursor-themes package | `install.inf` (converted) |
| `XCursors-Redglass/` | Redglass | xcursor-themes package | `install.inf` (converted) |
| `XCursors-Whiteglass/` | Whiteglass | xcursor-themes package | `install.inf` (converted) |

Source archives (`.zip` / `.deb`) go in `repos/`. Don't edit zip/deb files; extract into theme folders. Extracted source dirs in `repos/` are gitignored.

## New theme checklist

1. Download source (zip, clone repo, or .deb) into `repos/`
2. Extract cursor files into a new folder at root — name it descriptively
3. For Linux XCursor themes: remove 0-byte symlink stubs from `cursors/` dir, then run `x2wincurtheme -n "Name" -o "OutputFolder" "source/cursors"`
4. Preserve any readme/attribution/license files
5. Update this file and `README.md`
6. `git add -A && git commit -m "Add <ThemeName>" && git push`

## Installing cursors

Right-click the `.inf` file → **Install**, then select the scheme in **Mouse Properties > Pointers**.

`.inf` files register the scheme under `HKCU\Control Panel\Cursors\Schemes` and copy cursors to `C:\Windows\Cursors\<FolderName>`.

All current themes were installed on this machine on 2026-06-07 (42 schemes registered).

## Agent's role

- Organize and map cursor themes.
- Create and fix `.inf` / `.ini` installers for each set.
- Help add new cursor themes consistently.
- Rename, restructure, or deduplicate as needed.
- Convert Linux XCursor themes to Windows `.cur`/`.ani` format using `x2wincurtheme`.

## Conventions

- No code, no build steps, no tests, no CI.
- Cursor files are binary — use existing `.cur`/`.ani` as templates if adding new ones.
- `.inf` syntax is the classic Windows Setup INF format (`[Version]`, `[DefaultInstall]`, `[Strings]`, etc.).
- Keep each theme self-contained in its own folder with its own `.inf`.
- Preserve original author credit files (readme, attributions) when adding themes.
- Linux XCursor themes from `.deb` packages: extract with 7z; remove 0-byte symlink stubs from `cursors/` before running `x2wincurtheme`.
- Generated `.inf` from `x2wincurtheme` uses `HKLM` and lacks `[Wreg]` section — must fix to `HKCU` + add `[Wreg]` with per-cursor registry entries (see Yaru `.inf` as template).
