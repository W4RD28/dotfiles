
# Dotfiles

My personal dotfiles managed with **chezmoi**, configured for an Arch Linux + Niri + Noctalia setup.

![Clean Desktop](https://i.postimg.cc/CxsVdFqR/Screenshot-from-2026-08-30-21-43-31.png)
![Steam Tiling Workspace](https://i.postimg.cc/B6v7S3xM/Screenshot-from-2026-08-30-21-43-25.png)
![Browser and Terminal](https://i.postimg.cc/YCWH76pN/Screenshot-from-2026-08-30-21-43-20.png)

---

## 🖥️ Environment

| Component | Choice |
| :--- | :--- |
| **Distro** | Arch Linux |
| **WM / Compositor** | Niri |
| **Terminal** | foot |
| **Shell** | Noctalia |
| **Multiplexer** | Zellij |
| **Prompt** | Starship |
| **Fonts** | Monaspace, CommitMono |

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

## 📄 License

MIT — feel free to reuse anything.
