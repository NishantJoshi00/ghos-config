# Ghostty Configuration

A meticulously crafted terminal configuration for [Ghostty](https://ghostty.org/) featuring the Kanagawa Dragon color scheme, custom visual effects, and optimized keybindings for efficient workflow management.

## Visual Configuration

### Theme & Appearance

| Setting | Value | Description |
|---------|-------|-------------|
| **Theme** | Kanagawa Dragon | Dark, low-contrast color scheme |
| **Background Opacity** | 0.85 | Semi-transparent background |
| **Background Blur** | 20px | Blur effect for transparency |
| **macOS Icon** | Blueprint | Custom application icon |
| **Titlebar Style** | Tabs | Native macOS tab bar integration |
| **Window Padding** | 2px (x/y) | Minimal edge spacing |

### Color Palette

The configuration uses the Kanagawa Dragon theme with the following color values:

| Color | Hex | Usage |
|-------|-----|-------|
| **Background** | `#181616` | Main background color |
| **Foreground** | `#c8c093` | Primary text color |
| **Selection BG** | `#223249` | Selected text background |
| **Selection FG** | `#c5c9c5` | Selected text foreground |
| **Cursor** | `#c5c9c5` | Cursor color with inverted fg/bg |

#### ANSI Colors

| Index | Normal | Bright | Description |
|-------|--------|--------|-------------|
| 0 | `#0d0c0c` | `#a6a69c` | Black / Bright Black |
| 1 | `#c4746e` | `#e46876` | Red / Bright Red |
| 2 | `#8a9a7b` | `#87a987` | Green / Bright Green |
| 3 | `#c4b28a` | `#e6c384` | Yellow / Bright Yellow |
| 4 | `#8ba4b0` | `#7fb4ca` | Blue / Bright Blue |
| 5 | `#a292a3` | `#938aa9` | Magenta / Bright Magenta |
| 6 | `#8ea4a2` | `#7aa89f` | Cyan / Bright Cyan |
| 7 | `#c8c093` | `#c5c9c5` | White / Bright White |

## Keybindings

### Disabled Keys

| Keybind | Action | Reason |
|---------|--------|--------|
| `alt+p` | Ignore | Custom override |

### Window Management

| Keybind | Action | Description |
|---------|--------|-------------|
| `ctrl+super+f` | Toggle Fullscreen | Enter/exit fullscreen mode |

### Terminal Control

| Keybind | Action | Description |
|---------|--------|-------------|
| `super+k` | Clear Screen | Clear terminal display |

### Interface Actions

| Keybind | Action | Description |
|---------|--------|-------------|
| `super+shift+p` | Toggle Command Palette | Open command palette |

### Pane Management

#### Splitting

| Keybind | Action | Description |
|---------|--------|-------------|
| `super+shift+j` | New Split Down | Create horizontal split below |
| `super+shift+k` | New Split Up | Create horizontal split above |
| `super+shift+h` | New Split Left | Create vertical split left |
| `super+shift+l` | New Split Right | Create vertical split right |

#### Navigation

| Keybind | Action | Description |
|---------|--------|-------------|
| `super+h` | Go to Left Split | Navigate to left pane |
| `super+l` | Go to Right Split | Navigate to right pane |
| `super+j` | Toggle Split Zoom | Maximize/restore current pane |

## Custom Features

### Shaders

- **Cursor Warp Effect** (`shaders/cursor-warp.glsl`)
  Custom GLSL shader providing visual cursor effects

## File Structure

```
ghostty/
├── config              # Main configuration file
├── shaders/
│   └── cursor-warp.glsl  # Custom cursor shader
├── CLAUDE.md          # Development instructions
└── README.md          # This file
```

## Installation

1. Ensure Ghostty is installed on your system
2. Clone or copy this configuration to `~/.config/ghostty/`
3. Restart Ghostty or reload configuration

## Usage Notes

- The configuration is optimized for macOS with native titlebar integration
- Keybindings follow vim-style directional navigation (h/j/k/l)
- Semi-transparent background requires compositor support
- Custom shader may impact performance on older hardware

## References

- [Ghostty Documentation](https://ghostty.org/docs)
- [Configuration Reference](https://ghostty.org/docs/config/reference)
- [Keybind Reference](https://ghostty.org/docs/config/keybind/reference)
