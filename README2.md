# zzkt-qmk-to-zmk-port

This repository is a ZMK firmware fork configured to build a ported QMK layout (zzkt) with specific customization for a Charybdis 4x6 keyboard.

## 🔧 Key Features
- Based on ZMK firmware
- External config repo: [`zzkt-to-zmk-port`](https://github.com/ihlinuxdude/zzkt-to-zmk-port)
- Left-click and right-click trackball mapping
- BT Clear key added on Layer 2 (blue) of the `1` key

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

## 📥 Download Firmware
1. Click on the latest successful run under [Actions](https://github.com/ihlinuxdude/zzkt-qmk-to-zmk-port/actions)
2. Download `firmware` artifact
3. Flash the `.uf2` to your Nice Nano boards

---
Built with ❤️ using ZMK and a custom QMK conversion layout.
