# CAVA

Custom **CAVA** configuration with raw ASCII output for easy widget integration.

![Cava demo](../../assets/demo-cava.gif)

## Features

- Raw ASCII bars written to `/tmp/cava.raw`
- Pipeable into **EWW** widgets, **Waybar** modules, or custom scripts

## Usage

```sh
cava -p ~/.config/cava/config
```

CAVA writes raw ASCII bars to `/tmp/cava.raw`.

## Integration

Pairs with [audio_visualizer.py](../eww/scripts/audio/audio_visualizer.py) for the ASCII visualizer:

```sh
python3 ~/.config/eww/scripts/audio/audio_visualizer.py
```

Or watch the raw output live:

```sh
watch -n 0.1 cat /tmp/visualizer.txt
```