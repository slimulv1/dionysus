# 🍸 Dionysus

> °˖* ૮( • ᴗ ｡)っ🍸 shheersh — Dionysus vers. 1.0

A curated **Hyprland** rice for Arch Linux, tuned on a **ROG Zephyrus G15**.

![Arch Linux](https://img.shields.io/badge/Arch_Linux-1793D1?style=flat-square&logo=archlinux&logoColor=white)
![Hyprland](https://img.shields.io/badge/WM-Hyprland-67c6e3?style=flat-square)
![EWW](https://img.shields.io/badge/HUD-EWW-8b5cf6?style=flat-square)
![Waybar](https://img.shields.io/badge/Bar-Waybar-2ea043?style=flat-square)
![Neofetch](https://img.shields.io/badge/Neofetch-Animated-00a6a6?style=flat-square)

## Highlights

- **Animated Neofetch** splash (60-frame ASCII)
- **EWW HUD** — ASCII audio visualizer, sensor & network monitoring
- **Dynamic Waybar** with custom modules (workspaces, VPN, ASUS profiles)
- **CAVA** raw-ASCII output, pipeable into any widget
- **ASUS keyboard scripts** — brightness, breathing, profile cycling
- Nord-inspired **neon-radioactive** theme

## Demo

![Hyprland demo](assets/demo.gif)

## Components

| Directory | Component |
| --- | --- |
| [alacritty](dotfiles/alacritty/) | Terminal config |
| [cava](dotfiles/cava/) | Audio visualizer |
| [eww](dotfiles/eww/) | HUD & widgets |
| [firefox](dotfiles/firefox/) | Browser theme |
| [hypr](dotfiles/hypr/) | Window manager |
| [neofetch](dotfiles/neofetch/) | Animated fetch |
| [rofi](dotfiles/rofi/) | App launcher |
| [waybar](dotfiles/waybar/) | Status bar |
| [zsh](dotfiles/zsh/) | Shell config |

## Quick start

```sh
git clone https://github.com/slimulv1/dionysus.git
cp -r dionysus/dotfiles/* ~/.config/
```

> ⚠️ Configs are tuned for this setup (ROG Zephyrus G15, NordVPN, `wlp4s0`).
> Adjust interface names and device paths in the scripts as needed.

See [dotfiles/](dotfiles/) for the full walkthrough and per-component guides.