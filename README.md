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
| 7 | **ctrlcat0xx Cursors** | ctrlcat0xx / GitHub | 31 themed packs (anime, games, etc.) | `install.inf` per pack |

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
├── ctrlcat0xx-cursors/           # 31 themed cursor packs
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
