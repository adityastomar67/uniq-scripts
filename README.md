# ⚡ uniq-scripts

A collection of custom, standalone scripts tailored for system automation, workspace scaffolding, and terminal utilities.

## 📜 Included Scripts

### 1. `dotup`
**System Configuration Updater**
A robust, cross-platform update tool for your local system dotfiles.
- Handles `git` pulls for Master Dotfiles, Neovim config, and Zsh config.
- Automatically handles dirty working trees using `--autostash`.
- Automatically reloads Window Managers (BSPWM, sxhkd) on Linux or posts notifications on macOS.
- Cleans up common artifacts securely.

### 2. `DSA`
**Competitive Programming Workspace Scaffolder**
Instantly spins up a `tmux` + `neovim` playground specifically customized for Competitive Programming in C++.
- Generates competitive programming C++ boilerplate loaded with custom macros, optimized fast I/O, `DSU`, `SegTree`, and a robust debugging system.
- Mounts a 3-pane `tmux` layout: Main Code (Left), Input (Top Right), and Output (Bottom Right).
- Automatically manages `input.txt`, `output.txt` and `error.txt` files for local testing.

### 3. `fetch`
**Minimal System Fetch**
A visually distinct system information fetch tool leveraging [gum](https://github.com/charmbracelet/gum).
- Displays a clean ASCII logo paired with the active `USER` and cross-platform `UPTIME`.
- Dynamically adapts to terminal dimensions properly.

### 4. `mackeys`
**macOS Interactive Shortcut Cheat Sheet**
A fuzzy-searchable, comprehensive cheat sheet for macOS shortcuts.
- Leverages `fzf` to navigate an extensive list of categorized macOS keybinds.
- Features Nerd Font icons, colored terminal outputs, and descriptions.
- Hitting `Enter` copies the underlying key combo directly to your clipboard.

## 🛠 Dependencies

Depending on which scripts you are using, make sure the following dependencies are installed on your system:
- `git` (for `dotup`)
- `tmux` & `neovim` (for `DSA`)
- `gum` (for `fetch`)
- `fzf` (for `mackeys`)
- Optional: Nerd Fonts for accurate icon rendering in `mackeys`.

## 🚀 Usage

Ensure the scripts correspond with executable permissions:
```bash
chmod +x dotup DSA fetch mackeys
```

Execute them directly:
```bash
./dotup [ -z | -n ]
./DSA [session_name]
./fetch
./mackeys
```
