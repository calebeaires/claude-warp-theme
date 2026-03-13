# Claude Theme for Warp

A warm, elegant theme for [Warp](https://www.warp.dev/) inspired by [Claude AI](https://claude.ai)'s interface. Includes **light** and **dark** variants featuring Claude's signature amber/orange accent.

Based on [AuroralFrost/claude-light-theme](https://github.com/AuroralFrost/claude-light-theme) (VS Code).

---

## Preview

### Light

| Color     | Hex       | Preview |
|-----------|-----------|---------|
| Background | `#FFFFFF` | ![#FFFFFF](https://via.placeholder.com/16/FFFFFF/FFFFFF) |
| Foreground | `#374151` | ![#374151](https://via.placeholder.com/16/374151/374151) |
| Accent     | `#D97706` | ![#D97706](https://via.placeholder.com/16/D97706/D97706) |

### Dark

| Color     | Hex       | Preview |
|-----------|-----------|---------|
| Background | `#1A1A1A` | ![#1A1A1A](https://via.placeholder.com/16/1A1A1A/1A1A1A) |
| Foreground | `#F5F5F5` | ![#F5F5F5](https://via.placeholder.com/16/F5F5F5/F5F5F5) |
| Accent     | `#D97706` | ![#D97706](https://via.placeholder.com/16/D97706/D97706) |

---

## Install

### macOS

```bash
# Create the themes directory (if it doesn't exist)
mkdir -p ~/.warp/themes

# Copy the theme files
curl -o ~/.warp/themes/claude_light.yaml \
  https://raw.githubusercontent.com/calebeaires/claude-warp-theme/main/claude_light.yaml

curl -o ~/.warp/themes/claude_dark.yaml \
  https://raw.githubusercontent.com/calebeaires/claude-warp-theme/main/claude_dark.yaml
```

### Linux

```bash
THEMES_DIR="${XDG_DATA_HOME:-$HOME/.local/share}/warp-terminal/themes"
mkdir -p "$THEMES_DIR"

curl -o "$THEMES_DIR/claude_light.yaml" \
  https://raw.githubusercontent.com/calebeaires/claude-warp-theme/main/claude_light.yaml

curl -o "$THEMES_DIR/claude_dark.yaml" \
  https://raw.githubusercontent.com/calebeaires/claude-warp-theme/main/claude_dark.yaml
```

### Windows (PowerShell)

```powershell
$ThemesDir = "$env:APPDATA\warp\Warp\data\themes"
New-Item -ItemType Directory -Force -Path $ThemesDir

Invoke-WebRequest -Uri "https://raw.githubusercontent.com/calebeaires/claude-warp-theme/main/claude_light.yaml" `
  -OutFile "$ThemesDir\claude_light.yaml"

Invoke-WebRequest -Uri "https://raw.githubusercontent.com/calebeaires/claude-warp-theme/main/claude_dark.yaml" `
  -OutFile "$ThemesDir\claude_dark.yaml"
```

### Manual

1. Download [`claude_light.yaml`](claude_light.yaml) and/or [`claude_dark.yaml`](claude_dark.yaml)
2. Place them in your Warp themes directory:
   - **macOS:** `~/.warp/themes/`
   - **Linux:** `~/.local/share/warp-terminal/themes/`
   - **Windows:** `%APPDATA%\warp\Warp\data\themes\`
3. It may take a few minutes for Warp to discover new themes

### Activate

Open Warp, go to **Settings > Appearance > Themes**, and search for **Claude Light** or **Claude Dark**.

---

## Color Palette

### Terminal Colors (Light)

| Color   | Normal    | Bright    |
|---------|-----------|-----------|
| Black   | `#000000` | `#6B7280` |
| Red     | `#DC2626` | `#EF4444` |
| Green   | `#059669` | `#10B981` |
| Yellow  | `#D97706` | `#F59E0B` |
| Blue    | `#2563EB` | `#3B82F6` |
| Magenta | `#C026D3` | `#D946EF` |
| Cyan    | `#0891B2` | `#06B6D4` |
| White   | `#E5E7EB` | `#FFFFFF` |

### Terminal Colors (Dark)

| Color   | Normal    | Bright    |
|---------|-----------|-----------|
| Black   | `#333333` | `#888888` |
| Red     | `#DC2626` | `#EF4444` |
| Green   | `#059669` | `#5CDB95` |
| Yellow  | `#D97706` | `#FFB84D` |
| Blue    | `#2563EB` | `#5AA3FF` |
| Magenta | `#C026D3` | `#FF6B9D` |
| Cyan    | `#0891B2` | `#4ECDC4` |
| White   | `#B8B8B8` | `#FFFFFF` |

---

## Credits

- Theme colors derived from [AuroralFrost/claude-light-theme](https://github.com/AuroralFrost/claude-light-theme)
- Warp custom themes documentation: [docs.warp.dev](https://docs.warp.dev/terminal/appearance/custom-themes)

## License

[MIT](LICENSE)
