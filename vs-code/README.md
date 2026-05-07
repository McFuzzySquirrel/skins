# McFuzzySquirrel Warm Hooks (VS Code Theme)

This folder contains a VS Code color theme based on the shared palette used in:

- `McFuzzySquirrel/hooked-on-hooks` dashboard theme
- `McFuzzySquirrel/mcfuzzysquirrel.github.io` blog theme

## Local usage

1. Copy this `vs-code` folder somewhere local.
2. In VS Code, open the folder and run **Extensions: Install from VSIX...** after packaging, or use this folder as the basis for publishing.
3. Select **McFuzzySquirrel Warm Hooks** from **Preferences: Color Theme**.

## Package as VSIX

1. Open a terminal in this `vs-code` directory.
2. Run:
   - `npx @vscode/vsce package`
3. This generates a `.vsix` file (for example, `mcfuzzysquirrel-warm-hooks-0.0.1.vsix`).
4. In VS Code, run **Extensions: Install from VSIX...** and select the generated file.

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
