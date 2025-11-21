
# Dotfiles

My personal dotfiles managed with **chezmoi**, configured for a clean and minimal **Arch Linux + Niri** workflow.

---

## 🖥️ Environment

| Component           | Choice                                                 |
| ------------------- | ------------------------------------------------------ |
| **Distro**          | Arch Linux                                             |
| **WM / Compositor** | Niri                                                   |
| **Bar**             | Waybar                                                 |
| **Launcher**        | Fuzzel                                                 |
| **Terminal**        | foot                                                   |
| **Shell**           | *(none — using default system shell)*                  |
| **Multiplexer**     | Zellij                                                 |
| **Prompt**          | Starship                                               |
| **GTK Theme**       | Tokyo Night (AUR: `tokyonight-gtk-theme-git`)          |
| **Cursor**          | Simp1e Tokyo Night (AUR: `xcursor-simp1e-tokyo-night`) |
| **Fonts**           | Monaspace, CommitMono                                  |

---

## 📁 Structure

This repo uses Chezmoi’s layout:

```
~/.local/share/chezmoi
├── dot_config/
│   ├── fastfetch/
│   ├── foot/
│   ├── fuzzel/
│   ├── gtk-3.0/
│   ├── gtk-4.0/
│   ├── mako/
│   ├── niri/
│   ├── nwg-look/
│   ├── systemd/
│   ├── yazi/
│   ├── zellij/
│   └── starship.toml
└── run_once_*.sh (optional setup scripts)
```

All files inside `dot_config/` map directly to `~/.config/`.

---

## 🚀 Installation

To pull these dotfiles onto a new machine:

```bash
sh -c "$(curl -fsLS get.chezmoi.io)" -- init https://github.com/W4RD28/dotfiles
chezmoi apply
```

Or using SSH:

```bash
chezmoi init git@github.com:W4RD28/dotfiles.git
chezmoi apply
```

---

## 🎨 Themes & Appearance

The GTK theme and cursor are installed separately via AUR:

```bash
paru -S tokyonight-gtk-theme-git
paru -S xcursor-simp1e-tokyo-night
```

Fonts used:

* **Monaspace**
* **CommitMono**

Waybar and Niri use Tokyo Night–inspired colors where possible.

---

## 📌 Notes

* Themes, wallpapers, and icons are **not stored** in this repo.
* Only configuration and small templates are committed.
* This ensures the repo stays lightweight and fast to clone.

---

## 📄 License

MIT — feel free to reuse anything.

*(Generated using ChatGPT)*
