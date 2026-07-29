# Unreal Engine scene — Berlin Str. des 17. Juni

Packaged **Unreal Engine** build for visualizing the sample corridor along **Str. des 17. Juni** (Brandenburg Gate → Victory Column).

The scene is derived from the **OpenDRIVE (`.xodr`) map** and **sensor / drive data** shared in this repository:

- Map: [`../maps/opendrive/`](../maps/opendrive/)
- Drive data: [`../drive-data/`](../drive-data/)

This is a **visualization** build (packaged Unreal application), not the editable Unreal Editor project source.

| | |
| :--- | :--- |
| **Application** | Berlin (`Berlin_Drive`) |
| **Engine** | Unreal Engine **5.3.2** |
| **Platform** | Windows 10 / 11 (64-bit) |
| **Executable** | [`Berlin.exe`](Berlin.exe) |

## What’s included

Keep this layout intact — `Berlin.exe` relies on relative paths to the `Berlin/` and `Engine/` folders:

```
unreal-engine/
├── Berlin/       # Application content, assets, and binaries
├── Engine/       # Unreal Engine 5 runtime and dependencies
└── Berlin.exe    # Main launch executable
```

| Path | Contents |
|------|----------|
| [`Berlin.exe`](Berlin.exe) | Packaged Windows (Win64) executable |
| [`Berlin/`](Berlin/) | Game content, config, and binaries |
| [`Engine/`](Engine/) | Runtime engine files required by the packaged build |

Do **not** rename or delete `Berlin/` or `Engine/`.

## System requirements

| Requirement | Minimum | Recommended |
| :--- | :--- | :--- |
| **OS** | Windows 10 64-bit (1909+) | Windows 11 64-bit |
| **CPU** | Intel Core i5-8400 / AMD Ryzen 5 2600 | Intel Core i7-10700K / AMD Ryzen 7 3700X |
| **RAM** | 8 GB | 16 GB or higher |
| **GPU** | NVIDIA GTX 1060 (6 GB) / AMD RX 580 (8 GB) | NVIDIA RTX 3060 / AMD RX 6700 XT |
| **DirectX** | 12 | 12 |
| **Storage** | ~6 GB available SSD space | Fast NVMe SSD |

macOS / Linux packages are not included here.

## Prerequisites

Before launching `Berlin.exe`:

**Graphics drivers**

- **NVIDIA:** GeForce Game Ready **526.47** or newer (latest recommended)
- **AMD:** Radeon Software Adrenalin **22.11.1** or newer
- **Intel:** latest Arc Graphics driver

**Runtime dependencies**

- DirectX 12 support (Feature Level 12_0+)
- [Microsoft Visual C++ Redistributable 2015–2022 (x64)](https://aka.ms/vs/17/release/vc_redist.x64.exe) — also available under [`Engine/Extras/Redist/en-us/`](Engine/Extras/Redist/en-us/) as `UEPrereqSetup_x64.exe` / `vc_redist.x64.exe`

Missing VC++ runtimes often show up as `VCRUNTIME140.dll` or `MSVCP140.dll` not found.

## How to launch

1. Ensure `Berlin.exe`, `Berlin/`, and `Engine/` stay together under `unreal-engine/`.
2. On **Windows**, double-click [`Berlin.exe`](Berlin.exe).
3. If Windows permission prompts appear, try **Run as administrator**.

## Controls

| Action | Input |
| :--- | :--- |
| Move forward / backward | `W` / `S` |
| Strafe left / right | `A` / `D` |
| Move up / down | `E` / `Q` |
| Look / rotate camera | Mouse |
| Sprint / speed up | Hold `Shift` |
| Pause / menu | `Esc` |
| Toggle fullscreen | `F11` |

## Troubleshooting

**`VCRUNTIME140.dll` / `MSVCP140.dll` not found**  
Install the [Visual C++ Redistributable x64](https://aka.ms/vs/17/release/vc_redist.x64.exe), or run the redistributable under `Engine/Extras/Redist/en-us/`.

**Direct3D 12 / DirectX 12 crash**  
Update GPU drivers to a current official release and confirm the GPU supports DirectX 12 (Feature Level 12_0+).

**Freezes or low FPS**  
Close other GPU-/RAM-heavy apps and run the build from an SSD for faster asset streaming.

## Contact

For project source, integration support, or commercial licensing related to this scene, contact **[sales@aai-innovations.com](mailto:sales@aai-innovations.com)**.

For repository-wide context, see the root [`README.md`](../README.md).
