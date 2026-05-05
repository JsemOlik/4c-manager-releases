<p align="center">
  <img src="https://raw.githubusercontent.com/JsemOlik/4c-manager-releases/refs/heads/main/public/img/manager-logo.svg" alt="Manager Logo" width="220" />
</p>

<p align="center">
  <a href="https://github.com/JsemOlik/4c-manager-releases/releases/latest">
    <img alt="Latest Release" src="https://img.shields.io/github/v/release/JsemOlik/4c-manager-releases?display_name=release&label=latest%20release" />
  </a>
  <a href="https://github.com/JsemOlik/4c-manager-releases/tags">
    <img alt="Latest Tag" src="https://img.shields.io/github/v/tag/JsemOlik/4c-manager-releases?label=latest%20tag" />
  </a>
</p>

---

## Overview

4CAMPS Manager je aplikace postavená na **Tauri + React** pro správu 4CAMPS počítačů

## Tech Stack

- **Frontend:** React 19 + TypeScript + Vite
- **Desktop runtime:** Tauri v2 (Rust backend)
- **Komunikace:** Socket.IO
- **Package manager:** Bun

## Quick Start

```bash
bun install
bun run tauri dev
```

## Scripts

- `bun run tauri dev` - Spustí aplikaci v dev režimu
- `bun run tauri build` - Vytvoří produkční desktop build (nefunguje pro aktualizace)


## Project Structure

- `src/` - React frontend
- `src/routes/` - Routy
- `src/components/` - Sdílené UI komponenty
- `src/lib/` - Sdílené frontend utility a typy
- `src-tauri/src/` - Rust commandz a runtime logika
- `src-tauri/capabilities/` - Konfigurace Tauri capabilities

## Releasing

1. Připrav změny:
   ```bash
   git add .
   ```
2. Commit:
   ```bash
   git commit -m "chore: release vX.Y.Z"
   ```
3. Push:
   ```bash
   git push origin main
   ```
4. Tag:
   ```bash
   git tag vX.Y.Z
   git push origin vX.Y.Z
   ```
