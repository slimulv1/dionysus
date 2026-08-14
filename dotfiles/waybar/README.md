# Waybar

Custom **Waybar** configuration with dynamic, clickable modules.

![Waybar demo](../../assets/demo-waybar.png)

## Features

- **Custom workspace** modules (`workspace-1.sh` … `workspace-4.sh`), clickable
- **Battery status** — JSON script with dynamic icons and low-battery warnings
- **Volume control** via PipeWire (`wpctl`) — mute + scroll-to-change
- **Microphone toggle** — instant mute/unmute
- **Brightness control** — slider, scroll actions, and toggle
- **VPN integration** — NordVPN status module
- **Bluetooth module** — toggle script with tooltips
- **Network widget** — icons, bandwidth stats, `nm-connection-editor` launcher
- **ASUS profile module** — shows/toggles performance modes
- **Power menu** — integrated via Rofi

## Structure

```
waybar/
├── config
├── style.css
└── scripts/
    ├── asus-profile.sh
    ├── battery.sh
    ├── bluetooth-toggle.sh
    ├── brightness-toggle.sh
    ├── brightness.sh
    ├── mic.sh
    ├── nordvpn-status.sh
    ├── nordvpn-toggle.sh
    ├── powermenu.sh
    ├── volume.sh
    └── workspaces/
        ├── workspace-1.sh
        ├── workspace-2.sh
        ├── workspace-3.sh
        └── workspace-4.sh
```

## Requirements

- `hyprland` (`hyprctl` for workspaces)
- `rofi` (power menu)
- `wpctl` (PipeWire volume), `playerctl`, `brightnessctl`
- `nm-connection-editor` (network)
- `nordvpn` CLI (optional — VPN modules)
- **Nerd Font** for icons (󰤆, 󰖪, …)

## Usage

```sh
cp -r . ~/.config/waybar/
chmod +x ~/.config/waybar/scripts/*.sh
chmod +x ~/.config/waybar/scripts/workspaces/*.sh
```

- `config` → main Waybar configuration
- `style.css` → custom styling
- `scripts/` → helper scripts for modules