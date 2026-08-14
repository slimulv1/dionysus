# Dionysus — Dotfiles

Configuration for the **Dionysus** Hyprland rice — Arch Linux, tuned on a ROG Zephyrus G15.

Nord-inspired **neon-radioactive** theme across every component.

## Components

| Directory | Component | Description |
| --- | --- | --- |
| [alacritty](alacritty/) | Terminal | Neon-radioactive theme |
| [cava](cava/) | Audio visualizer | Raw ASCII output for widgets |
| [eww](eww/) | HUD & widgets | ASCII visualizer, sensors, network |
| [firefox](firefox/) | Browser theme | Firefox Color theme |
| [hypr](hypr/) | Window manager | Core WM config + scripts |
| [neofetch](neofetch/) | Animated fetch | 60-frame ASCII animation |
| [rofi](rofi/) | App launcher | Custom launcher theme |
| [waybar](waybar/) | Status bar | Dynamic modules & styling |
| [zsh](zsh/) | Shell | Shell configuration |

## Gallery

| | | |
| --- | --- | --- |
| ![Neofetch](../assets/demo-neofetch.gif) | ![EWW](../assets/demo-eww.png) | ![Rofi](../assets/demo-rofi.png) |
| ![Cava](../assets/demo-cava.gif) | ![Alacritty + Waybar](../assets/demo-alacritty.png) | ![Waybar](../assets/demo-waybar.png) |

## Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/slimulv1/dionysus.git
   ```

2. Copy each component into `~/.config/`:

   ```sh
   cp -r dionysus/dotfiles/* ~/.config/
   ```

3. Follow the per-component guide in each directory's `README.md`.

## Requirements

- **Hyprland** + **hyprpaper** (compositor & wallpaper)
- **eww** (Elkowar's Wacky Widgets), **cava**, **rofi**, **alacritty**, **waybar**
- **grim / slurp / wl-clipboard** (screenshots & clipboard)
- **wpctl / playerctl / brightnessctl** (volume, media, backlight)
- **lm-sensors** (temps, fans, voltages), **jq** (EWW JSON parsing)
- **Nerd Font** (Waybar & EWW icons)