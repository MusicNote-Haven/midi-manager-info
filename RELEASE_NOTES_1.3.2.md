# MusicNote Haven MIDI Manager 1.3.2 stability release

- **Windows application:** 1.3.2
- **Microsoft Store package:** 1.3.2.0
- **Linux application:** 1.3.2
- **Debian package:** 1.3.2-1 for Ubuntu 26.04 LTS amd64
- **Accepted shared source:** `a5d8b02f32ffed9e2a971eb494492a37c319901b`

## What changed

- Improved Qt background-worker cleanup to reduce the risk of unexpected exits during long-running scans and other background tasks.
- Made Organization analysis candidate selection more efficient for large MIDI/KAR collections, including files returned to Analyzer.
- Made **Stop Safely** responsive during candidate-selection SQL queries.

The copy-first Organizer model, Trial / Free limits, and existing Version 1.x licences are unchanged.

## Availability

Windows 1.3.2 is available through the existing Microsoft Store listing (Store ID `9P9PKX8XNDWF`). Linux 1.3.2-1 is available as a verified direct `.deb` download.

- [Official downloads](https://musicnotehaven.ethercomm.eu/downloads/)
- [Windows in Microsoft Store](https://musicnotehaven.ethercomm.eu/downloads/windows-store/)
- [Linux Debian download](https://musicnotehaven.ethercomm.eu/downloads/linux-deb/)

## Package provenance

**Windows Store MSIX**
- File: `MusicNote-Haven-MIDI-Manager-1.3.2.0-x64-store.msix`
- SHA-256: `022443611aa7d17b5d650ae644859ebc9338d739f80a48cc62f469e196513e31`

**Linux Debian package**
- File: `musicnote-haven-midi-manager_1.3.2-1_amd64.deb`
- Size: 78,251,520 bytes
- SHA-256: `0f879a6b82320e023e58a85029e29a89afae6fb1a81c6d68c3f7b5e2f4901917`

Both packages were built from private source commit `a5d8b02f32ffed9e2a971eb494492a37c319901b`. Source code and private build records are not published in this information repository.
