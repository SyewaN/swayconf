# Void + Sway Rice

*Minimal Wayland setup*

![Screenshot_2025-07-01_16-29-27](https://github.com/user-attachments/assets/ee6887ae-ba10-447e-b5fd-d1ae9ec30214) ![image](https://github.com/user-attachments/assets/2cb4f762-9ab1-48d4-b1fa-1292da550a02) 


## ⚡ System Info

- **OS**: Void Linux
- **WM**: Sway
- **Terminal**: Alacritty
- **Bar**: Waybar 
- **Launcher**: Fuzzel
- **Notifications**: Dunst

## 🎨 Features

- **Auto Tiling**: Automatic window layouts
- **Roman Numerals**: Workspace icons (Ⅰ-Ⅹ)
- **Gruvbox Colors**: Consistent theming
- **Minimal UI**: Clean, distraction-free

## 📦 Quick Install

```bash
# Core packages
sudo xbps-install -S sway waybar foot fuzzel dunst shotman

# Audio & extras
sudo xbps-install -S pipewire pavucontrol polkit-gnome udiskie

# Auto-tiling (AUR equivalent için kendi build'in gerekebilir)
# git clone + make install autotiling
```

## 🚀 Setup

```bash
git clone https://github.com/SyewaN/swayconf.git

## ⚙️ Configuration

## ⌨️ Keybinds

| Key | Action |
|-----|--------|
| `Super + Return` | Terminal |
| `Super + D` | Fuzzel launcher |
| `Super + Q` | Close window |
| `Super + Escape` | Lock screen |
| `Super + Home` | Logout menu |
| `Super + Shift + R/T/Y` | Screenshots |


## 🎨 Customization

**Wallpaper**: Edit `~/.config/sway/config` line with `output * bg`  
**Colors**: Modify `~/.config/waybar/style.css` for Gruvbox variants  
**Blur**: Adjust `blur_passes` in sway config (current: 8)

## 🔧 Quick Fixes

```bash
# Audio issues
sv up pipewire

# Screenshot not working  
sudo xbps-install -S shotman

# Foot daemon not starting
foot -s &
```

## 📁 File Structure

```
config/
├── sway/config          # Main sway config
└── waybar/
    ├── config           # Bar modules  
    └── style.css        # Gruvbox styling
```

---

⭐ **Star** if you like this setup!  
