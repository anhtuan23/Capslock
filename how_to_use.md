# How to use

1. Run `cd mac_v3`
2. Edit `capslock.yml`
3. Run `make install` (install `yq` with `brew install yq` if necessary)
4. Copy to karabiner conf: `cp capslock.json ~/.config/karabiner/assets/complex_modifications/`
5. Go to Karabiner Element, remove to existing rule, then re add it
6. Readd to chezmoi: `chezmoi add ~/.config/karabiner`