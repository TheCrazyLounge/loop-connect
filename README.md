# Loop Connect Controller

Unofficial Windows installer for the **Loop Connect** hub (fans, pump, RGB). Not affiliated with EKWB.

This repository contains **releases only** — no source code. Source is maintained privately by TheCrazyLounge.

## Requirements

- Windows 10 or 11 (64-bit)
- Loop Connect hub on USB
- Close **EK-Connect** before running (only one app can use the hub)
- Run as **Administrator** for full CPU/GPU temperature sensors

## Install

1. Open [Releases](https://github.com/TheCrazyLounge/loop-connect/releases).
2. Download the latest `LoopConnectController-Setup.exe`.
3. Run the installer and follow the prompts.

## Configuration

Settings are stored under:

`%LocalAppData%\EkHubController\`

On first run, an existing EK-Connect `config.json` can be imported automatically if placed next to the executable before launch.

## Support

Report issues to the project maintainer. Do not expect EKWB support for this tool.
