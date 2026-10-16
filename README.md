# Optima Desktop — releases

Installers and auto-update files for **Optima Desktop**, the softphone for Optima contact center agents.

This repository holds **releases only** — no source code. Every version is a [GitHub Release](../../releases) with three files:

| File | Purpose |
| --- | --- |
| `Optima_<version>_x64-setup.exe` | Windows installer |
| `Optima_<version>_x64-setup.exe.sig` | Update signature |
| `latest.json` | Update manifest read by the app |

## Install

1. Download `Optima_<version>_x64-setup.exe` from the [latest release](../../releases/latest).
2. Run it. No administrator rights are needed — Optima installs for the current user.
3. If Windows shows **"Windows protected your PC"**, click **More info → Run anyway**.

You only need to do this once. After that, Optima checks for updates on its own and asks before installing — it never restarts during a call.

## Updates

The app reads:

```
https://github.com/sunvone/optima-v3-dialer/releases/latest/download/latest.json
```

which always points to the latest **published** release. Drafts and pre-releases are not offered to agents.
