# Hyprland

Custom **Hyprland** configuration tuned for EWW integration, the CAVA visualizer, and Waybar.

![Hyprland demo](../../assets/demo-hypr.gif)

## Features

- **Dynamic Waybar** — switches depending on active/inactive windows
- **Firefox preload** for smooth quick access
- **ASUS keyboard fixes** — brightness, breathing, and profile cycling

## Structure

```
hypr/
├── hyprland.conf
├── hyprpaper.conf
├── extras/
│   ├── ascii_boot.txt
│   └── quotes.txt
├── scripts/
│   ├── refresh-eww.sh
│   ├── waybar_watcher.sh
│   └── asus-kbd/
│       ├── cycle-profile.sh
│       ├── kbd-breathing.sh
│       └── kbd-brightness.sh
├── shaders/
│   └── screenshot_overlay.frag
└── wallpapers/
    ├── bg_wallpaper.png
    └── black.png
```

## Requirements

- **Hyprland** (Wayland compositor & WM)
- **hyprpaper** (wallpaper daemon)
- **eww** (Elkowar's Wacky Widgets)
- **cava** (audio visualizer)
- **rofi** (application launcher)
- **alacritty** (terminal emulator)
- **thunar** (file manager)
- **firefox** (browser)
- **grim**, **slurp** (screenshots)
- **wl-clipboard** (`wl-copy`)
- **wpctl** (PipeWire volume), **playerctl** (media), **brightnessctl** (backlight)
- **curl** (network requests), **lm-sensors** (temps, fans, voltages)

## Usage

- **Waybar / EWW / hyprpaper** are kept running reliably by
  [`waybar_watcher.sh`](scripts/waybar_watcher.sh) via `exec-once`.
- **CAVA visualizer** launches on login and outputs ASCII to `/tmp/cava.raw`,
  rendered by [`audio_visualizer.py`](../eww/scripts/audio/audio_visualizer.py).
- **ASUS keyboard** controls live in
  [`scripts/asus-kbd/`](scripts/asus-kbd/) — brightness, breathing, and profile cycling.