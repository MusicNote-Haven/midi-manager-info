# MusicNote Haven MIDI Manager 1.3.1 maintenance release

- **Windows application:** 1.3.1
- **Microsoft Store package:** 1.3.1.0
- **Linux application:** 1.3.1
- **Debian package:** 1.3.1-1 for Ubuntu 26.04 LTS amd64
- **Accepted shared source:** `28c224063d08525c64d9b838b59a387636d6d6fa`

## Availability

Windows 1.3.1 is available through the existing Microsoft Store listing (`9P9PKX8XNDWF`). The 1.3.1.0 Store candidate was built from the accepted shared source and runtime-smoke-tested on Windows 11.

Linux 1.3.1-1 is available as the verified direct `.deb`. The package was installed on KANTOOR and the packaged Source Index workflow was runtime-accepted on Ubuntu 26.04 LTS.

## Source Index stability

Version 1.3.1 corrects the Source Index background-worker lifetime and cleanup ordering that could cause an unexpected native application exit during long Linux Source Index runs. Resume and Stop Safely preserve completed work and cleanup now follows the Qt worker/thread lifetime correctly.

## MIDI/RMID recovery and diagnostics

The semantic parser can recover additional valid RIFF/RMID files and can use controlled tolerant parsing for the specific out-of-range MIDI data-byte case after strict parsing fails. Clearly malformed or non-MIDI files remain fail-closed, with more actionable parser failure reasons.

## Startup window sizing

The application reapplies its intended initial geometry after the main window is shown. This improves first-open sizing on desktop environments where the window manager applies geometry after the initial resize request.

## Compatibility and upgrade

Existing Version 1.x licences remain valid. The maintenance update does not change the copy-first Organizer safety model or the Trial / Free lifetime-output policy introduced in the 1.x release line.

## Release provenance

Windows Store MSIX:
- file: `MusicNote-Haven-MIDI-Manager-1.3.1.0-x64-store.msix`
- size: 67,719,288 bytes
- SHA-256: `0bf34163c61375ffc68b916de887c37436f9c28b246c406f4caf12706fa1788e`

Linux Debian package:
- file: `musicnote-haven-midi-manager_1.3.1-1_amd64.deb`
- size: 78,247,846 bytes
- SHA-256: `dac0a26aa757666ffc4ba67261f1f495d5109782acf770503f92222c13a83f8c`

Both packages were built from clean pushed source commit `28c224063d08525c64d9b838b59a387636d6d6fa`.
