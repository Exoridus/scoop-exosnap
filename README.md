# ExoSnap Scoop Bucket

Official [Scoop](https://scoop.sh) bucket for [ExoSnap](https://github.com/Exoridus/exosnap) —
a Windows-native screen / application / region recorder with an NVIDIA NVENC pipeline,
multi-track audio, webcam overlay, and diagnostics.

## Install

```powershell
scoop bucket add exosnap https://github.com/Exoridus/scoop-exosnap
scoop install exosnap
```

## Requirements

- Windows 10/11 x64
- An NVIDIA GPU with supported NVENC (AMD/Intel/software encoding are not supported in 0.1.x)
- The Microsoft Visual C++ 2015–2022 x64 runtime — install via
  `scoop install extras/vcredist2022` or from
  <https://aka.ms/vs/17/release/vc_redist.x64.exe> if it is not already present

## Updating

Manifests track the portable ZIP of each [GitHub Release](https://github.com/Exoridus/exosnap/releases)
and carry `checkver`/`autoupdate` metadata. The canonical manifest source lives in the main
repository under [`packaging/scoop/`](https://github.com/Exoridus/exosnap/tree/main/packaging/scoop).
