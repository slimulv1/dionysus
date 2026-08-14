# Rofi

Nord-inspired, neon-radioactive **Rofi** launcher theme.

![Rofi demo](../../assets/demo-rofi.png)

## Features

- Custom neon-radioactive theme
- Background image handled at launch (`rofi_image.png`)

## Usage

```sh
cp -r . ~/.config/rofi/
rofi -show drun
```

Bound to **ALT+SPACE** in the [Hyprland config](../hypr/hyprland.conf).

## Files

- `config.rasi` — launcher configuration
- `theme.rasi` — neon-radioactive theme
- `image.png` — launcher background (copied to `/dev/shm/rofi_image.png` at login)