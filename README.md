# VS Code User Settings Backup

Git-backed backup of personal VS Code configuration for easy restoration on fresh machines.

## 📁 Tracked Files

- [`settings.json`](settings.json) - Editor preferences, themes, fonts, formatting rules
- [`keybindings.json`](keybindings.json) - Custom keyboard shortcuts and overrides
- [`snippets/`](snippets/) - Code snippets directory (currently empty)
- [`extensions.json`](extensions.json) - Recommended extensions list
- [`.gitignore`](.gitignore) - Excludes workspace state, logs, caches, and extension binaries

## 🚀 One-Command Restore

```bash
# Clone to VS Code user settings directory
git clone <repo-url> "$HOME/AppData/Roaming/Code/User"
```

Or manually copy files to your VS Code user settings folder:
- **Windows**: `%APPDATA%\Code\User`
- **macOS**: `~/Library/Application Support/Code/User`
- **Linux**: `~/.config/Code/User`

## 📋 Commit Message Convention

Keep commits atomic and self-documenting:

```
feat: add new keyboard shortcut for format document
fix: correct tab size setting for JSON files
style: update font family to Monaspace Argon NF
docs: add snippet for React component
refactor: reorganize settings by category
```

## 🔧 Manual Extension Installation

After restoring settings, install extensions via Command Palette:
1. `Ctrl+Shift+P` → "Extensions: Show Recommended Extensions"
2. Install all recommended extensions from the list

## 📝 Notes

- Extension binaries are excluded from Git (see `.gitignore`)
- Workspace-specific settings are not tracked
- Settings are optimized for web development with Git Bash terminal