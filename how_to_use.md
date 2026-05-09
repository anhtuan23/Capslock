# How to use

1. Run `cd mac_v3`
2. Edit `capslock.yml`
3. Run `make compile` or `make install` (install `yq` with `brew install yq` if necessary)
4. Copy to karabiner conf: `cp capslock.json ~/.config/karabiner/assets/complex_modifications/`
5. In Karabiner-Elements, enable your mouse under `Devices` if you want mouse button remaps to apply
6. Go to Karabiner Element, remove the existing rule, then re-add it
7. Re-add to chezmoi: `chezmoi add ~/.config/karabiner`

## Notes

- Added mouse button remaps in `mac_v3/capslock.yml`:
  - `button4` -> `option + 1`
  - `button5` -> `command + w`
- Karabiner-Elements supports mouse button remapping, but it does not expose horizontal scroll events as `from` inputs in complex modifications. That means `scroll left` -> `control + tab` and `scroll right` -> `control + shift + tab` cannot be implemented in this repo via Karabiner alone.
