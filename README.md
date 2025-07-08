# Kanagawa Oh My Posh Theme

A Oh My Posh theme inspired by the Kanagawa color palette, featuring warm, muted colors that are easy on the eyes.

## Preview

![Kanagawa Theme Preview](https://github.com/user-attachments/assets/2acfc3d5-e1fe-4bb1-815c-76168ab2fd9f)

## Features

- **Multi-line prompt** with clean layout
- **Session info** - displays username@hostname with SSH indicator
- **Path display** - shows current directory with folder icon
- **Git integration** - branch status, changes, stash count with dynamic colors
- **Execution time** - shows command execution duration
- **Exit status** - visual indicator for command success/failure
- **Right-aligned info** - shell name, battery status, and current time
- **Colored prompt arrows** - tri-color arrow prompt indicator

## Color Scheme

Based on the Kanagawa color palette:
- **Background**: `#2A2A37`, `#7E9CD8`, `#98BB6C`
- **Foreground**: `#DCD7BA`, `#1F1F28`
- **Accent Colors**: `#957FB8`, `#E6C384`, `#FFA066`, `#76946A`
- **Error**: `#E82424`

## Installation

### Prerequisites

1. **Install Oh My Posh**:
   ```powershell
   winget install JanDeDobbeleer.OhMyPosh
   ```

2. **Install a Nerd Font** (required for icons):

3. **Set your terminal font** to the Nerd Font in your terminal settings

### Usage

#### Option 1: Direct Usage
```powershell
oh-my-posh init pwsh --config ~/path/to/kanagawa.omp.json | Invoke-Expression
```

#### Option 2: Add to Profile (Recommended)
Add to your PowerShell profile (`$PROFILE`):
```powershell
oh-my-posh init pwsh --config ~/path/to/kanagawa.omp.json | Invoke-Expression
```

For other shells:
```bash
# Bash
eval "$(oh-my-posh init bash --config ~/path/to/kanagawa.omp.json)"

# Zsh
eval "$(oh-my-posh init zsh --config ~/path/to/kanagawa.omp.json)"
```

#### Option 3: Use from GitHub
```powershell
oh-my-posh init pwsh --config 'https://raw.githubusercontent.com/username/repo/main/themes/kanagawa.omp.json'
```

## Segments

| Segment | Description | Icon |
|---------|-------------|------|
| Session | Username@hostname with SSH indicator | `🖧` |
| Path | Current directory | `📁` |
| Git | Branch, changes, stash count | `🔀` `📝` `📋` `📚` |
| Execution Time | Command duration | `⏱️` |
| Status | Exit code indicator | `✅` `❌` |
| Shell | Current shell name | `🐚` |
| Battery | Battery percentage and status | `🔋` |
| Time | Current time | `🕐` |

## Git Status Colors

- **Green** (`#98BB6C`): Clean repository
- **Orange** (`#FF9E3B`): Working or staged changes
- **Yellow** (`#E6C384`): Ahead and behind upstream
- **Purple** (`#957FB8`): Ahead or behind upstream

## Customization

To customize the theme, edit the `kanagawa.omp.json` file:

- **Colors**: Modify the `foreground` and `background` properties
- **Icons**: Change the Unicode characters in `template` strings
- **Segments**: Add, remove, or reorder segments in the `segments` array
- **Layout**: Adjust `alignment` and `style` properties

---
