# Loop Connect Controller

Unofficial Windows installer for the **Loop Connect** hub (fans, pump, RGB). Not affiliated with EKWB.

This repository contains **releases only** — no source code. Source is maintained privately by TheCrazyLounge.

## Requirements

- Windows 10 or 11 (64-bit)
- Loop Connect hub on USB
- EK-Connect closed and not starting with Windows (see below)
- Administrator rights: the app always asks for them (needed for CPU/GPU temperature sensors)

## Before you install: EK-Connect

Only one app can talk to the hub at a time. EK-Connect starts with Windows and grabs the hub first, so Loop Connect Controller shows **Not connected** ("EK Loop Connect hub not found") while EK-Connect is running.

1. Exit EK-Connect from its tray icon (closing the window only hides it).
2. Stop it starting with Windows: **Task Manager → Startup apps → EK-Connect → Disable**, or uninstall EK-Connect.

## Install

1. Open [Releases](https://github.com/TheCrazyLounge/loop-connect/releases).
2. Download the latest `LoopConnectController-Setup.exe`.
3. Run the installer and follow the prompts.

Notes:

- The installer isn't code-signed yet, so Windows SmartScreen may say **"Windows protected your PC"**. Click **More info → Run anyway**.
- **Create a desktop shortcut** and **Start with Windows** are ticked by default. Start with Windows uses a Task Scheduler task so the app can start as administrator, minimized to the tray. Turn it off any time in the app.
- Only one copy runs at a time. Opening it again brings the existing window forward.

## Configuration

Settings are stored under:

`%LocalAppData%\EkHubController\`

On first run, an existing EK-Connect `config.json` can be imported automatically if placed next to the executable before launch.

## Uninstall

Use **Settings → Apps → Installed apps → Loop Connect Controller → Uninstall**. You'll be asked whether to also delete your fan curves and settings. The default keeps them for a reinstall.

## Support

Report bugs and request features on the [Issues](https://github.com/TheCrazyLounge/loop-connect/issues/new/choose) page. Please pick a template and fill it in. Do not expect EKWB support for this tool.
