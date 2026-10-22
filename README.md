<img alt="nadelacruz-00 · mainline Linux on a Snapdragon tablet, and the tools around it" src="assets/header.svg" width="100%">

Daily driver is a OnePlus Pad 3 (`erhai`, Snapdragon 8 Elite) running Ubuntu on the [mainline port](https://github.com/TheMojoMan/oneplus-erhai-linux). Most of what is here either fixes something on that tablet, or builds a tool that did not ship for Linux aarch64. Everything is built on GitHub Actions and published as a release.

### Pad 3 on mainline Linux

| | |
|---|---|
| [erhai-charging-lab](https://github.com/nadelacruz-00/erhai-charging-lab) | USB-C charging test lab. CI-built candidate kernels, each with the numbers it must produce; only a passing candidate becomes a PR. |
| [erhai-sleep-lab](https://github.com/nadelacruz-00/erhai-sleep-lab) | Suspend/resume test lab. An on-device flight recorder files every failed sleep into a failure class before any fix is tried. |
| [oneplus-erhai-linux](https://github.com/nadelacruz-00/oneplus-erhai-linux) | Fork of the port. [PR #2](https://github.com/TheMojoMan/oneplus-erhai-linux/pull/2) merged upstream: 39 W PPS charging by running the SC8547A charge pump like the vendor path. |

### Android side of the same tablet

| | |
|---|---|
| [status-bar-guard](https://github.com/nadelacruz-00/status-bar-guard) | KernelSU module with a WebUI. Per-app suppression of the status bar and notification shade so a full-screen Linux desktop in Termux:X11 keeps focus. |
| [erhai-x11-keyboard-remap](https://github.com/nadelacruz-00/erhai-x11-keyboard-remap) | LSPosed + KernelSU remap for the official keyboard: a real Escape, an F1–F12 row, the bot key as Super. |
| [OnePlus_KernelSU_SUSFS-OPD2415](https://github.com/nadelacruz-00/OnePlus_KernelSU_SUSFS-OPD2415) | Single-device KernelSU + SUSFS kernel build (6.6.89) derived from WildKernels, with a build-time guard on required config. |

### Desktop and tooling

| | |
|---|---|
| [magnetize](https://github.com/nadelacruz-00/magnetize) | GNOME extension with macOS Magnet shortcuts, drag-to-edge snapping and a top bar menu. Shortcuts follow the physical keys on any layout. |
| [aarch64-re-tools](https://github.com/nadelacruz-00/aarch64-re-tools) | Ghidra native components and a static Rizin, built for Linux aarch64 and checked against upstream checksums. |
| [librepods](https://github.com/nadelacruz-00/librepods) | Fork adding a native Linux aarch64 release of the LibrePods Rust app. |
| [claude-usage-band](https://github.com/nadelacruz-00/claude-usage-band) | Claude Code plugin that puts context fill and plan usage limits under the text input. |
| [WorkLens](https://github.com/nadelacruz-00/WorkLens) | Windows app that records the screen while you work and has a vision model write up what you did. Encrypted on disk, per-app privacy rules, no telemetry. |
