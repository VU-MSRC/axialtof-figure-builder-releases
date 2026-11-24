<!-- This is the README for the PUBLIC releases-only repository. Copy it there
     as README.md. The source repository stays private; this public repo holds
     nothing but this file and the Releases. -->

# AxialTOF Figure Builder

Read Bruker flex-series (axial time-of-flight) spectra — autoflex, ultraflex,
microflex, neofleX — and build clean, publication-ready figures from them. It
opens the classic XMASS folder layout (`fid` + `acqus`), reconstructs the m/z
axis from the calibration stored in the folder, lists the peaks, and exports
labelled figures as **PNG, PDF, or SVG** at exact centimetre sizes.

Everything runs locally. No spectrum data leaves your computer.

## Download

Get the latest version from the **[Releases](../../releases/latest)** page:

| File | For |
| --- | --- |
| `AxialTOF-Setup-<version>.exe` | Windows installer (Windows 10 21H2+ / 11) |
| `AxialTOF-macOS.dmg` | macOS disk image |
| `AxialTOF-Windows.zip` / `AxialTOF-macOS.zip` | the raw app, no installer |

## Install

- **Windows** — run the Setup `.exe` and follow the wizard. It installs
  per-user (no admin password) and adds a Start-menu entry. *First launch
  only:* Windows SmartScreen may warn because the app isn't code-signed —
  click **More info → Run anyway**.
- **macOS** — open the `.dmg` and drag the app into **Applications**. *First
  launch only:* the app isn't notarized, so **right-click the app → Open →
  Open** (a plain double-click is refused with a misleading "can't be checked"
  message). After that it opens normally.

## Use

Drag a zipped flex folder — or the folder itself (the one holding `fid` and
`acqus`, or any folder above it) — onto the window, or use **Open .zip** /
**Open folder**. Tick or click the peaks you want labelled, set the figure
size in centimetres, and **Export** as PNG (300–1200 dpi), vector PDF, or SVG.
The peak list and the full spectrum also export as CSV.

Bruker `.d` folders (TSF/TDF/BAF) aren't supported yet; load the flex folder
for the same spectrum instead.

## Issues

Questions and bug reports are welcome in this repository's
[Issues](../../issues).
