# McFuzzySquirrel Warm Hooks (Copilot CLI Companion Theme)

Copilot CLI runs in your terminal, so matching it to **Warm Hooks** means applying a matching terminal color scheme.

This folder includes ready-to-use presets for:

- Alacritty
- WezTerm
- Windows Terminal

## Core palette

- Background: `#1A120F`
- Surface: `#2A1D18`
- Surface soft: `#3A2720`
- Text: `#F7EEE8`
- Muted text: `#D4B9A6`
- Accent: `#FF9A45`
- Accent strong: `#CF6223`
- Link/highlight: `#FFC98D`
- Border: `#5B3C2D`

## Quick apply

### Alacritty (Linux/macOS)

1. Copy the theme file:

   ```bash
   mkdir -p ~/.config/alacritty/themes
   cp <repo-root>/copilot-cli/alacritty/mcfuzzysquirrel-warm-hooks.toml ~/.config/alacritty/themes/
   ```

2. Import it from your `~/.config/alacritty/alacritty.toml`:

   ```toml
   import = ["~/.config/alacritty/themes/mcfuzzysquirrel-warm-hooks.toml"]
   ```

### WezTerm (Linux/macOS/Windows)

1. Copy the scheme file:

   ```bash
   mkdir -p ~/.config/wezterm/colors
   cp <repo-root>/copilot-cli/wezterm/mcfuzzysquirrel-warm-hooks.lua ~/.config/wezterm/colors/
   ```

2. Reference it from your `~/.wezterm.lua`:

   ```lua
   local warm_hooks = dofile(os.getenv("HOME") .. "/.config/wezterm/colors/mcfuzzysquirrel-warm-hooks.lua")
   local wezterm = require("wezterm")
   return {
     color_schemes = { ["McFuzzySquirrel Warm Hooks"] = warm_hooks },
     color_scheme = "McFuzzySquirrel Warm Hooks",
   }
   ```

### Windows Terminal

1. Open Windows Terminal settings JSON.
2. Copy the JSON object from:

   - `<repo-root>/copilot-cli/windows-terminal/mcfuzzysquirrel-warm-hooks.json`

3. Paste it into the `schemes` array.
4. Set your profile `colorScheme` to:

   - `McFuzzySquirrel Warm Hooks`

## Copilot CLI note

Copilot CLI uses your terminal styling, so once the terminal scheme is active, Copilot CLI output will match the Warm Hooks palette.
