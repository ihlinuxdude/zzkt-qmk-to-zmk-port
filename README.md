# zzkt-qmk-to-zmk-port

This repository is a ZMK firmware fork configured to build a ported QMK layout (zzkt) with specific customization for a Charybdis 4x6 keyboard.

## 🔧 Key Features
- Based on ZMK firmware
- External config repo: [`zzkt-to-zmk-port`](https://github.com/ihlinuxdude/zzkt-to-zmk-port)
- Left-click and right-click trackball mapping
- BT Clear key added on Layer 2 (blue) of the `1` key

## 📆 Layout Screenshots

### Layer 0 - Base (Dvorak)
![Layer 0 - Base](https://raw.githubusercontent.com/ihlinuxdude/zzkt-to-zmk-port/main/docs/layer0_base.png)

### Layer 1 - Symbols/Nav
![Layer 1 - Symbols](https://raw.githubusercontent.com/ihlinuxdude/zzkt-to-zmk-port/main/docs/layer1_symbols.png)

### Layer 2 - Mouse/BT
![Layer 2 - Mouse](https://raw.githubusercontent.com/ihlinuxdude/zzkt-to-zmk-port/main/docs/layer2_mouse_bt.png)

## 📦 Firmware Builds
Each commit triggers a GitHub Actions workflow that:
- Initializes West with this manifest
- Pulls external config
- Builds firmware for:
  - `charybdis_4x6_left`
  - `charybdis_4x6_right`
- Uploads `.uf2` files as build artifacts

## ✅ Status
[![Build ZMK Firmware](https://github.com/ihlinuxdude/zzkt-qmk-to-zmk-port/actions/workflows/build.yml/badge.svg)](https://github.com/ihlinuxdude/zzkt-qmk-to-zmk-port/actions/workflows/build.yml)

## 🍜 Download Firmware
1. Click on the latest successful run under [Actions](https://github.com/ihlinuxdude/zzkt-qmk-to-zmk-port/actions)
2. Download `firmware` artifact
3. Flash the `.uf2` to your Nice Nano boards

## ✨ Flashing Instructions (Windows)

### 🛠️ Requirements
- A USB-C cable
- Your `.uf2` firmware files (from GitHub Actions > Artifacts)
- Windows 10 or newer

### 🔧 Steps
1. Plug your Nice Nano into your computer via USB-C
2. Double-tap the **reset** button on the Nice Nano:
   - The device should appear as a drive called `NICENANO`
3. Drag the `.uf2` firmware file onto the `NICENANO` drive
4. Wait for the device to reboot
5. Repeat for both halves

---
Built using ZMK and a custom QMK conversion layout.
