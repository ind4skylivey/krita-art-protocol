---
type: resource
tags: [fix, optimization, linux]
---

# Troubleshooting & Optimization

## 🛠️ Common Fixes

### 1. Tablet Lag or "Jitter"
- **Cause:** Interference with other input drivers or high stabilizer settings.
- **Fix:** 
  - Ensure `digimend-drivers-git` is installed (AUR).
  - In Krita, set `Stabilizer` to 'Basic' instead of 'Weighted' for sketching.
  - Disable "Touch" if your tablet supports it and you don't use it.

### 2. Canvas Flickering
- **Fix:** Go to `Settings` -> `Configure Krita` -> `Display`. 
  - Change **Renderer** from OpenGL to **Software** (if on old hardware) or ensure **Vulkan** is selected if your Arch setup supports it.

### 3. Pressure Dies after Wake-up
- **Fix:** Restart the Wacom/input service.
  ```bash
  # Quick fix command
  sudo modprobe -r hid_uclogic && sudo modprobe hid_uclogic
  ```

## 🚀 Performance Tips
- **Memory Limit:** `Settings` -> `Configure Krita` -> `General` -> `Performance`. Set "Memory Limit" to 70-80% of your RAM.
- **Instant Preview:** Enable `View` -> `Instant Preview Mode` for large brushes.
- **Auto-save:** Set to 15 minutes to avoid losing work without constant disk thrashing.

## 🔗 External Links
- [Krita Documentation](https://docs.krita.org/)
- [DIGImend Tablet Support](https://digimend.github.io/tablets/)
