# MusicNote Haven MIDI Manager

**MusicNote Haven MIDI Manager 1.3.3** is local desktop software for musicians, keyboard players, MIDI collectors and digital music archivists who manage `.mid`, `.midi` and `.kar` collections.

## Current production releases

| Platform | Current build | Public status |
|---|---|---|
| Windows desktop/laptop | App `1.3.3`, Microsoft Store package `1.3.3.0` | **Microsoft Store distribution** |
| Ubuntu 26.04 LTS amd64 | App `1.3.3`, Debian package `1.3.3-1` | **Available as verified direct download** |

Both packages were built from accepted shared source `c0b2ab8682ff9c6191acfd0354743959dc315297`.

### Linux 1.3.3-1

- File: `musicnote-haven-midi-manager_1.3.3-1_amd64.deb`
- Size: `76,014,084` bytes
- SHA-256: `88b948664265215fc2707663ff8cfd42587dd7b5aed18be3344ac68339634e8b`
- Accepted source: `c0b2ab8682ff9c6191acfd0354743959dc315297`

### Windows 1.3.3

- Microsoft Store package: `1.3.3.0`
- Store ID: `9P9PKX8XNDWF`
- Windows package SHA-256: `f859da12c494f17cbde769706594ca3a9d0869071ead7522ef84c848daeb2fbc`
- Windows 11 packaged runtime smoke test: passed on ZBOOKWIN

## Version 1.3.3 maintenance highlights

- Organized Library planning and execution now reject byte-identical output content, even when distinct source paths refer to the same MIDI/KAR bytes.
- Content identity is verified with BLAKE3; different performances with different bytes remain eligible.
- Large Organization analysis result sets are handled in bounded batches while keeping Stop Safely responsive.
- Splashscreen click and size handling is more robust.
- Stable Linux network-interface selection helps retain legitimate signed Professional activation across supported runtime changes.
- Linux 1.3.3-1 was installed and functionally accepted on KANTOOR; Windows 1.3.3.0 packaged runtime was accepted on ZBOOKWIN.

## Lifetime licence terms

**One payment, lifetime access** for Personal and Professional, including future major versions 2.x, 3.x and later without another upgrade fee or subscription. Existing 1.x offline use remains protected; support for future major versions will be implemented when those versions are released.

Trial / Free keeps its 100 lifetime unique verified Organized Library output allowance. You may browse, index, analyze and review a large source library without consuming this allowance.

## Version 1.3.2 stability highlights

- Corrected Qt background-worker cleanup across app workflows for improved reliability during long-running scans.
- Faster Organization analysis candidate selection for large MIDI/KAR libraries, including files returned to Analyzer.
- Stop Safely can interrupt candidate-selection database work rather than waiting for the entire query to finish.
- At the time of 1.3.2, the lifetime licensing implementation applied to the 1.x generation; the commercial lifetime update policy was subsequently extended to future major versions with 1.3.3 website communications.

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
- Personal and Professional now carry the lifetime all-future-versions commitment described above; the current 1.x signed licence remains usable offline after successful local verification.
- Trial / Free can index/analyse large source folders and copy up to 100 lifetime unique verified files into Organized Library; preview, review and failed operations do not count.
- Tested with libraries approaching 200,000 MIDI/KAR files.

## Local-first safety and privacy

Core library work is local. If the optional Online Artist & Song Discovery fallback is used, only candidate artist/title text is sent. MIDI/KAR contents, local paths, filenames and profile data are not sent.

## Release notes in this repository

- [1.3.3 maintenance release](RELEASE_NOTES_1.3.3.md)
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
