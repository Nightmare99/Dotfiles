# Dotfiles

Personal dotfiles for macOS. This repository includes configuration for Zsh, VS Code, iTerm2, Windsurf, fonts, and a Vivaldi theme.

## Prerequisites

- **Homebrew (brew)** is required for package management on macOS.
- **Oh My Zsh** is required by the Zsh configuration.

## Quick setup (recommended)

Run the following from the root of this repository to back up existing configs and create symlinks:

```sh
# Ensure you're in this repo's root
REPO_DIR="$(pwd)"
BACKUP_DIR="$HOME/.config-backup/dotfiles-$(date +%Y%m%d-%H%M%S)"
mkdir -p "$BACKUP_DIR"

# Zsh
[ -f "$HOME/.zshrc" ] && mv "$HOME/.zshrc" "$BACKUP_DIR/.zshrc"
ln -sfn "$REPO_DIR/shell/.zshrc" "$HOME/.zshrc"

# VS Code (stable)
VSC_USER_DIR="$HOME/Library/Application Support/Code/User"
mkdir -p "$VSC_USER_DIR"
[ -f "$VSC_USER_DIR/settings.json" ] && mv "$VSC_USER_DIR/settings.json" "$BACKUP_DIR/vscode.settings.json"
ln -sfn "$REPO_DIR/vscode/settings.json" "$VSC_USER_DIR/settings.json"

# Windsurf (Codeium)
mkdir -p "$HOME/.codeium/windsurf"
ln -sfn "$REPO_DIR/windsurf/rules" "$HOME/.codeium/windsurf/rules"
ln -sfn "$REPO_DIR/windsurf/workflows" "$HOME/.codeium/windsurf/workflows"
```

Then restart your terminal and VS Code.

## iTerm2

You can import the exported preferences/state file:

- Open iTerm2 → Preferences.
- Use iTerm2's import/restore functionality to load `iterm2/iTerm2 State.itermexport`.
- Restart iTerm2 if needed.

If you prefer loading preferences from a folder, point iTerm2 to this repo and save/restore as desired.

## Fonts (Victor Mono)

Install the font so your terminal/editor can use it:

```sh
unzip -o "fonts/Victor_Mono.zip" -d "fonts/Victor_Mono"
# Install via Font Book (opens the files); accept prompts to install
open "fonts/Victor_Mono"/*.ttf 2>/dev/null || open "fonts/Victor_Mono"/*.otf 2>/dev/null || true
```

Alternatively, install manually by double‑clicking the font files or copying them to `~/Library/Fonts/`.

## Vivaldi Theme

Import the theme via the Vivaldi UI:

- Vivaldi → Settings → Themes → Import/Open Theme.
- Select `vivaldi/full-black.zip`.

## Notes

- This repository currently does not include a Brewfile. If desired, add one later and run `brew bundle` to automate app/tool installation.
- After creating symlinks, restart apps (Terminal/iTerm2, VS Code, Vivaldi) to pick up changes.
