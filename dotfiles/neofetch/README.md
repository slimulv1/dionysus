# Neofetch

Custom **animated Neofetch** — minimal info layout with a 60-frame ASCII animation.

![Neofetch demo](../../assets/demo-neofetch.gif)

## Features

- Minimal info layout
- **Animated ASCII** via `animated-neofetch.sh`
- Fast load (cached output)

## Usage

Add to your shell rc (`~/.bashrc`, `~/.zshrc`, …):

```sh
# Animated Neofetch splash
if [[ -n $PS1 ]]; then
    ~/.config/neofetch/animated-neofetch.sh 0.05
    clear
fi
```

## Files

```
neofetch/
├── config.conf
├── myascii.txt
├── animated-neofetch.sh
└── frames_colour/
    └── frame0001.txt … frame0060.txt
```

## Notes

- Frames live in `frames_colour/` — swap them for a different animation.
- `animated-neofetch.sh` caches output in `~/.cache/neofetch.txt` for speed.
  After editing your config, clear the cache:

  ```sh
  rm -f ~/.cache/neofetch.txt
  ```