# MusicNote Haven MIDI Manager

**MusicNote Haven MIDI Manager 1.3.2** is local desktop software for musicians, keyboard players, MIDI collectors and digital music archivists who manage `.mid`, `.midi` and `.kar` collections.

## Current production releases

| Platform | Current build | Public status |
|---|---|---|
| Windows desktop/laptop | App `1.3.2`, Microsoft Store package `1.3.2.0` | **Available in Microsoft Store** |
| Ubuntu 26.04 LTS amd64 | App `1.3.2`, Debian package `1.3.2-1` | **Available as verified direct download** |

Both packages were built from accepted shared source `a5d8b02f32ffed9e2a971eb494492a37c319901b`.

### Linux 1.3.2-1

- File: `musicnote-haven-midi-manager_1.3.2-1_amd64.deb`
- Size: `78,251,520` bytes
- SHA-256: `0f879a6b82320e023e58a85029e29a89afae6fb1a81c6d68c3f7b5e2f4901917`
- Accepted source: `a5d8b02f32ffed9e2a971eb494492a37c319901b`

### Windows 1.3.2

- Microsoft Store package: `1.3.2.0`
- Store ID: `9P9PKX8XNDWF`
- Windows package SHA-256: `022443611aa7d17b5d650ae644859ebc9338d739f80a48cc62f469e196513e31`
- Windows 11 packaged runtime smoke test: passed on ZBOOKWIN

## Version 1.3.2 stability highlights

- Corrected Qt background-worker cleanup across app workflows for improved reliability during long-running scans.
- Faster Organization analysis candidate selection for large MIDI/KAR libraries, including files returned to Analyzer.
- Stop Safely can interrupt candidate-selection database work rather than waiting for the entire query to finish.
- Version 1.x licence terms and the copy-first safety model are unchanged.

## Version 1.3.1 maintenance highlights

- Source Index background-worker lifetime and cleanup were hardened for long Linux runs.
- Resume and Stop Safely keep completed Source Index work and follow the corrected worker/thread cleanup lifecycle.
- Controlled MIDI/RMID recovery now accepts additional valid files while preserving explicit parser diagnostics.
- Initial window sizing was improved without changing the established workflow.

## Version 1.3 highlights

- Stronger Organization analysis using filename clues, embedded MIDI/KAR evidence and the offline music reference.
- Offline reference first, with privacy-minimized Online Artist & Song Discovery fallback when no usable local result is available.
- Clearer truthful phase, elapsed-time and heartbeat progress for long analysis jobs.
- Safer Organized Library rename and Re-evaluate workflows with collision, identity and rollback protections.
- Better manual Artist/Title/Filename reconciliation, including case-only rename/path consistency.
- Personal and Professional Version 1.x licences remain lifetime for the 1.x generation and remain usable offline after successful local verification.
- Trial / Free can index/analyse large source folders and copy up to 100 lifetime unique verified files into Organized Library; preview, review and failed operations do not count.
- Tested with libraries approaching 200,000 MIDI/KAR files.

## Local-first safety and privacy

Core library work is local. If the optional Online Artist & Song Discovery fallback is used, only candidate artist/title text is sent. MIDI/KAR contents, local paths, filenames and profile data are not sent.

## Release notes in this repository

- [1.3.2 stability release](RELEASE_NOTES_1.3.2.md)
- [1.3.1 maintenance release](RELEASE_NOTES_1.3.1.md)
- [1.3.0 stable release](RELEASE_NOTES_1.3.0.md)
- [1.2.2 Linux stable release](RELEASE_NOTES_1.2.2.md)
- [1.2.1 Windows stable release](RELEASE_NOTES_1.2.1.md)
- Historical 1.1.0, 1.0.x and 0.9.x release notes remain preserved.

## Official links

- Website: https://musicnotehaven.ethercomm.eu/
- Downloads: https://musicnotehaven.ethercomm.eu/downloads/
- Windows Store: https://musicnotehaven.ethercomm.eu/downloads/windows-store/
- Linux download: https://musicnotehaven.ethercomm.eu/downloads/linux-deb/
- Manual: https://musicnotehaven.ethercomm.eu/manual/
- Release notes: https://musicnotehaven.ethercomm.eu/release-notes/
- Recorded 1.2 workflow video: https://youtu.be/5q9JugTzUL0
- Newsletter: https://musicnotehaven.ethercomm.eu/newsletter/
