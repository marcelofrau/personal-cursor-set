# personal-cursor-set

My personal collection of Windows custom cursor themes (`.cur` / `.ani`).

## Themes

| # | Theme | Source | Variants | Installer |
|---|-------|--------|----------|-----------|
| 1 | **Mario Gant** | behelit / DeviantArt | Mario-themed | `install.inf` |
| 2 | **Posy's Cursor** | Michiel de Boer | Default cursors | `_install Posy Default.inf` |
| 3 | **Bibata Modern Amber** | ful1e5 / GitHub | Amber (orange) | `install.inf` |
| 4 | **Bibata Modern Classic** | ful1e5 / GitHub | Classic (black) | `install.inf` |
| 5 | **Bibata Modern Ice** | ful1e5 / GitHub | Ice (white) | `install.inf` |
| 6 | **Windows Cursor Concept v2.2** | Jepri Creations / AMag1c | Dark, Light, Big Dark, Big Light | See variant folders |
| 7 | **Yaru Ubuntu** | csabika98 / GitHub | Ubuntu Yaru cursor theme for Windows | `install.inf` |
| 8 | **ctrlcat0xx Cursors** | ctrlcat0xx / GitHub | 31 themed packs (anime, games, etc.) | `install.inf` per pack |
| 9 | **Capitaine Cursors** | keeferrourke / GitHub | Original (keeferrourke r4) | `install.inf` |
| 10 | **Capitaine Cursors (Colors)** | sainnhe / GitHub | 8 color variants (Default, White, Gruvbox, Nord, Palenight + White) | `Install.inf` per variant |
| 11 | **Apple Cursor** | ful1e5 / GitHub | macOS-style, 3 sizes (Regular, Large, Extra-Large) | `install.inf` |
| 12 | **Apple Cursor (White)** | ful1e5 / GitHub | White variant, 3 sizes | `install.inf` |
| 13 | **macOS Cursors (Sierra+)** | antiden / GitHub | Sierra+. No Shadow / With Shadow → 3 sizes each | `Install.inf` per variant |
| 14 | **macOS Cursors (El Capitan)** | antiden / GitHub | El Capitan. No Shadow / With Shadow → 3 sizes each | `Install.inf` per variant |
| 15 | **DMZ-Black** | Ubuntu package | Classic Ubuntu black cursor | `install.inf` |
| 16 | **DMZ-White** | Ubuntu package | Classic Ubuntu white cursor | `install.inf` |
| 17 | **Breeze** | KDE / Ubuntu package | KDE Plasma dark cursor | `install.inf` |
| 18 | **Breeze Snow** | KDE / Ubuntu package | KDE Plasma light cursor | `install.inf` |
| 19 | **ComixCursors** | Ubuntu package | Black, Blue, Green, Orange, Red, White + Slim variants (11 total) | `install.inf` per variant |
| 20 | **XCursors Handhelds** | xcursor-themes / Ubuntu | Handheld device cursor theme | `install.inf` |
| 21 | **XCursors Redglass** | xcursor-themes / Ubuntu | Classic red glass theme | `install.inf` |
| 22 | **XCursors Whiteglass** | xcursor-themes / Ubuntu | Classic white glass theme | `install.inf` |

## Installation

1. Open the desired theme folder
2. Right-click the `.inf` file → **Install**
3. Go to **Mouse Properties > Pointers** and select the scheme from the dropdown

The `.inf` registers the scheme under `HKCU\Control Panel\Cursors\Schemes` and copies files to `C:\Windows\Cursors\<FolderName>`.

## Organization

```
personal-cursor-set/
├── mario-gant/                   # Mario-themed cursors
├── Posy's Cursor/                # Posy's cursor set
├── Bibata-Modern-Amber/          # Bibata Amber (orange)
├── Bibata-Modern-Classic/        # Bibata Classic (black)
├── Bibata-Modern-Ice/            # Bibata Ice (white)
├── Windows-Cursor-Concept-v2.2/  # Cursor Concept v2.2 (4 variants)
├── Yaru-Ubuntu/                  # Ubuntu Yaru cursor theme
├── ctrlcat0xx-cursors/           # 31 themed cursor packs
├── Capitaine-Cursors/            # Capitaine Cursors (kefferourke r4)
├── Capitaine-Cursors-Variants/   # Capitaine Color Variants (sainnhe r5)
├── Apple-Cursor/                 # macOS-style (ful1e5)
├── Apple-Cursor-White/           # macOS-style white (ful1e5)
├── macOS-Cursors-Sierra/         # macOS Sierra+ (antiden)
├── macOS-Cursors-ElCapitan/      # macOS El Capitan (antiden)
├── DMZ-Black/                    # DMZ Black (Ubuntu)
├── DMZ-White/                    # DMZ White (Ubuntu)
├── Breeze/                       # KDE Breeze (dark)
├── Breeze-Snow/                  # KDE Breeze Snow (light)
├── ComixCursors-{Black,Blue,Green,Orange,Red,White,Slim-*}/  # ComixCursors (11)
├── XCursors-Handhelds/           # Handheld cursor theme
├── XCursors-Redglass/            # Redglass cursor theme
├── XCursors-Whiteglass/          # Whiteglass cursor theme
├── repos/                        # Original downloads cache
├── AGENTS.md                     # OpenCode agent instructions
└── README.md                     # This file
```

## Licenses

Each theme retains its original author's license. See attribution and readme files inside each folder.

| Theme | License |
|-------|---------|
| Mario Gant | CC Non-Commercial |
| Posy's Cursor | Freeware |
| Bibata | GPL-3.0 |
| Windows Cursor Concept v2.2 | Freeware |
| ctrlcat0xx Cursors | Varies per pack |
| Capitaine Cursors | LGPL-2.1 |
| Apple Cursor | MIT |
| macOS Cursors (antiden) | Freeware |
| DMZ | LGPL |
| Breeze | GPL-2.0 |
| ComixCursors | LGPL-2.1+ |
| XCursors (xorg) | MIT |
