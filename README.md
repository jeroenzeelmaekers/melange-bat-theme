# Melange Theme for Bat

## Installation 

## Copy themes to config

### If no theme file is present create a new one

Create the theme folder (if not present already) and navigate into the folder.

```bash
mkdir -p "$(bat --config-dir)/themes"

cd "$(bat --config-dir)/themes"
```

### clone themes inside `themes` folder

```bash
git clone git@github.com:jeroenzeelmaekers/melange-bat-theme
```

# Rebuild cache

Bat requires you to update the binary cache when adding new themes.

```bash
bat cache --build
```

# Enable themes

Theme theme should be in `bat --list-themes`. If so add these 2 lines to your config:

```
# Set the theme to "Melange"
--theme-dark="Melange Dark"
--theme-light="Melange Light"
```
