# Network

DAGS VB6 ActiveX DLL `drNetwork.dll` (project drNetwork) exposing class `clsSpeed`. Connects a UNC share with MPR `WNetAddConnection2`, measures link speed via `MultinetGetConnectionPerformance`, and disconnects with `WNetCancelConnection2`; companion module `modWNetError` maps WNet error codes. A small Test harness (`Project1.exe`) polls `GetConnectionSpeed` on a timer and shows Mb/s.

**Source last updated:** 2026-08-27 · **Language:** VB6 · **Target:** VB6 Win32 · **Output:** ActiveX DLL, WinForms exe

_Note: original OneDrive LastWriteTime values were wiped to 2026-08-27 by a zip transfer; date above uses best available evidence (headers/copyright where helpful)._

## Solution structure

| Project | Language | Type | Purpose |
|---------|----------|------|---------|
| `drNetwork` (`Network.vbp`) | VB6 | ActiveX DLL | WNet connect/disconnect and MultinetGetConnectionPerformance speed helper |
| `Project1` (`Test/Project1.vbp`) | VB6 | WinForms exe | Timer demo that displays network speed in Mb/s |

## How to open

Open the `.vbp` in Visual Basic 6.0 IDE:
- `Network.vbp`
- `Test/Project1.vbp`

## Requirements

- Visual Basic 6.0 IDE
- Registered `drNetwork.dll` for the Test project reference
- Windows MPR (`mpr.dll`) for connection and performance queries

## Attribution and provenance

Working copy from my Historical Dev folder `VB/Old/Network`.
Company names in project files: DAGS.

## License

MIT (c) 2026 VaderConsulting for Dave Robinson's code. See `LICENSE`.
