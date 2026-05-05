<p align="center">
  <img src="https://raw.githubusercontent.com/JsemOlik/4c-manager-releases/refs/heads/main/public/img/manager-logo.svg?token=GHSAT0AAAAAAD4KD2JO7TT23FYVKQSOAD4K2P2JOCQ" alt="Manager Logo" width="220" />
</p>

<h1 align="center">4CAMPS Manager</h1>
<p align="center">Desktop control client for 4CAMPS computer rooms.</p>

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

4CAMPS Manager is a **Tauri + React** desktop app used to manage 4CAMPS PCs in real time.
It verifies the local machine through the API, connects to Socket.IO, and reacts to remote actions (block, ping, forms, power actions).

## Tech Stack

- **Frontend:** React 19 + TypeScript + Vite
- **Desktop runtime:** Tauri v2 (Rust backend)
- **Realtime:** Socket.IO client
- **Package manager:** Bun

## Quick Start

```bash
bun install
```

Tauri development mode:

```bash
bun run tauri dev
```

## Scripts

- `bun run tauri dev` - Run desktop app in dev mode
- `bun run tauri build` - Build production desktop binaries (Won't work for updates)


## Project Structure

- `src/` - React frontend
- `src/routes/` - Route pages
- `src/components/` - Shared UI components
- `src/lib/` - Shared frontend utilities and types
- `src-tauri/src/` - Rust commands and app runtime logic
- `src-tauri/capabilities/` - Tauri capability config

## Releasing

1. Stage changes:
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
