---
type: resource
os: arch-linux
tablet: huion-hs610
---

# Krita & Arch Linux Setup

## 🐧 System Configuration (Arch)

Ensure you have the correct drivers. While the modern kernel supports Huion, `digimend` helps with extra buttons.

```bash
# Install Krita and tablet tools
sudo pacman -S krita xf86-input-wacom libwacom kcm-wacomtablet
```

### Pressure Fix (Huion HS610)
If pressure doesn't work or the cursor jumps:
1. Open Krita.
2. Go to `Settings` -> `Configure Krita` -> `Tablet`.
3. In Linux, ensure **Windows 8+ Pointer Input (Windows Ink)** is selected if using Wayland, or **WinTab** for X11.
4. **IMPORTANT:** Open the "Tablet Tester" in Krita and draw. You should see blue lines (pressure) and red lines (tilt).

## 🎨 Krita Workspace

### Essential Dockers
Activate these panels (`Settings` -> `Dockers`):
- **Tool Options:** (Keep it always visible).
- **Layers:** (Essential).
- **Advanced Color Selector:** Set it to triangle mode.
- **Overview:** To see your drawing at a distance.

### Recommended Shortcuts
Edit in `Configure Krita` -> `Keyboard Shortcuts`:
- **R:** Pick Layer (Select layer of the touched pixel).
- **Q:** Invert selection (Useful for shadows).
- **~ (Tilde):** Eraser Mode (Turns any brush into a temporary eraser).
- **Shift + Space:** Rotate Canvas.

## 🖌️ Recommended Brushes (Default Tags)
Krita 5 includes everything you need:
1. **Sketch:** `b) Pencil-2` (Tilt shading).
2. **Lineart:** `b) Basic-5 Size` (Stable and clean).
3. **Paint:** `d) Wet Knife Acrylic` (Mixes color while painting).
4. **Shadows:** `f) Charcoal Rock Soft` (Light texture for anime shadows).
5. **Soft:** `b) Airbrush Soft`.
