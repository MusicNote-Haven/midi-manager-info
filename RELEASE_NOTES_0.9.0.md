# MusicNote Haven MIDI Manager 0.9.0 Release Candidate

Publication phase: 2026-07-25
Platforms: Windows 11 Setup.exe and Ubuntu/Kubuntu 24.04 amd64 `.deb`
Release channel: controlled external test / release candidate
Verified source: `48c620068626e3df7b4b8da37b3d7d8740cf7a27`

## Official downloads

- [Windows Setup.exe 0.9.0](https://musicnotehaven.ethercomm.eu/downloads/windows-setup/)
- [Linux `.deb` 0.9.0](https://musicnotehaven.ethercomm.eu/downloads/linux-deb/)
- [SHA256SUMS.txt](https://musicnotehaven.ethercomm.eu/downloads/SHA256SUMS.txt)
- [Multilingual release notes](https://musicnotehaven.ethercomm.eu/release-notes/)
- [Protected tester programme](https://musicnotehaven.ethercomm.eu/founding-testers/)

## Accepted artifacts

| Platform | Filename | Size | SHA-256 |
|---|---|---:|---|
| Windows | `MusicNote-Haven-MIDI-Manager-Setup-0.9.0.exe` | 49,036,376 bytes | `75ea885abcba47cb9372ae6f6f982353a75998ea7d5aeb4d15dade32d8909583` |
| Linux | `musicnote-haven-midi-manager_0.9.0-1_amd64.deb` | 73,886,566 bytes | `3a3dfdbb0112b3b60ca49c92010caefedb2c23503e0bdb5287c8e38cdf03e0e4` |

## Highlights since 0.3.0

- Five-language First-Run Setup Wizard and safer cross-platform folder handling.
- Hardened Library Organizer task coordination, safe stop, verified copy/archive and recovery behavior.
- Managed playback and Playback Queue shuffle/replacement/Now Playing workflows.
- Floppy Image Studio machine profiles, verified existing-IMG editing and preview-first USB/Gotek export planning.
- Signed license validation, offline grace and current-device release/transfer.
- Verified database backup, retention, migration rollback and healthy startup.
- Public-package privacy auditing and exact Windows/Linux artifact provenance.

## Acceptance

The Windows installer passed strict readiness, installation over an existing test setup and real packaged startup with existing profile/index data retained and Database Healthy. The Linux `.deb` was rebuilt from the same final source commit and passed package scope, checksum and provenance verification.

## Known limitations

- Windows 0.9.0 is unsigned; security/reputation warnings may appear.
- Linux targets Ubuntu/Kubuntu 24.04 amd64.
- Hardware profiles do not guarantee universal Korg/Gotek, Roland or proprietary-format compatibility.
- Keep backups and begin with test copies.

## Route to 1.0

0.9.0 is functionally frozen. No ordinary features are planned before 1.0.0. Controlled external feedback may produce only genuine release-blocker fixes in an optional 0.9.1 or 0.9.2.
