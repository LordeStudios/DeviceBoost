# Changelog

All notable changes to DeviceBoost are documented here. The format is based on Keep a Changelog and the project uses semantic versioning.

## 0.1.0, 2026-11-09

First public release.

### Added

- Native Windows client (Direct2D / DirectWrite / Direct3D 11) with six screens: dashboard, GPU profiles, app launcher, devices, activity log and settings.
- Opening liquid glass logo animation, skippable with any input.
- GPU identity profiles: seven built-in presets (NVIDIA, AMD, Intel) plus custom vendor and device definitions from the command line.
- Device wide identity persistence read by every hooked application.
- Identity reporting seams for DXGI, Direct3D 9, Vulkan, OpenGL and Windows SetupAPI.
- Proxy deployment of `dxgi.dll` / `d3d9.dll` next to a chosen application, with protected directory and unknown DLL refusal rules.
- Launcher that starts an application with the identity hooks injected and extracts its real icon.
- Host service with a loopback admin API, node pairing tokens, a node registry and a checksum verified job offload protocol (H.265 transcode presets).
- Activity log with timestamps for host transitions, profile changes and launches.
- Stale data model: the client keeps the last known values on screen when the host goes away and marks them until the connection returns.
- Portable distribution: no installer, no registry entries, no runtime DLL dependencies.
