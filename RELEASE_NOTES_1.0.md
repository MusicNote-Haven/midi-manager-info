# MusicNote Haven MIDI Manager 1.0 production generation

Publication phase: 2026-08-14

| Platform | Application version | Package | Release source |
|---|---:|---|---|
| Windows | **1.0.0** | Microsoft Store package `1.0.0.0` | `d081632e19524b1d733aa627e52007433f0a5c7d` |
| Linux | **1.0.1** | Debian package `1.0.1-1` | `796422678a886de68d23df33904a0c57e38a6ab2` |

The platform version difference is intentional. Windows 1.0.0 and Linux 1.0.1 are the paired production generation.

## Platform status

### Linux 1.0.1-1

The verified Ubuntu/Kubuntu 24.04 amd64 package is available as a direct MusicNote Haven download.

- Artifact: `musicnote-haven-midi-manager_1.0.1-1_amd64.deb`
- Size: `74,217,972` bytes
- SHA-256: `22d0abc281dde24277e0af9137666eadaa3c5d5d55f76d2e01d64acf0439f3d8`
- Package/runtime acceptance: passed

### Windows 1.0.0

The corrected Windows production package has been submitted through the existing Microsoft Store listing.

- Application version: `1.0.0`
- Store package version: `1.0.0.0`
- Package size: `67,520,390` bytes
- SHA-256: `39a5349947aea0eb211ffe821c049b802aee8f99e0fc7140ad625398f0f6a8d2`
- Corrected production source: `d081632e19524b1d733aa627e52007433f0a5c7d`
- Status at publication preparation: Microsoft Store certification/publication

Microsoft Store manages package signing and publication.

## Major 1.0 changes

### Current Search & Filter workflow

The current sidebar workflow uses **Search** rather than the former separate MIDI Files by Device navigation item. Search & Filter now covers combined discovery including filename/metadata criteria, MIDI device information, MIDI Type/mode and analysis-oriented filters.

### Analysis trust and targeted reanalysis

- Indexed, successfully analyzed, failed and pending states are presented distinctly.
- Analysis provenance and evidence are surfaced instead of presenting a score without context.
- File Detail explains current analysis evidence and score interpretation.
- Review Queue and Failed Analysis Review provide targeted reanalysis paths.

### Library Organizer

- Preview and analysis remain separate from execution.
- Planned organized targets are visible before applying changes.
- Normal organization is copy-first.
- Execution verifies resulting copies and keeps source preservation explicit.
- Trial/Free guidance distinguishes source analysis from the Organized Library output limit.

### Organized Library and Playback Queue

- Organized Library browsing is incremental and database-backed for large libraries.
- Search, selection and liked-state operations remain responsive while more rows load.
- Playback Queue uses database-backed library data and supports queue/shuffle workflows without requiring the entire organized library to be materialized at once.

### Floppy Image Studio and IMG workflows

- Disk Image Creator supports standard FAT12 720 KB and 1.44 MB image workflows.
- Machine profiles provide appropriate defaults for supported workflows.
- IMG Viewer supports single-image inspection and multi-image folder catalogs.
- PDF, CSV and JSON report outputs remain available.
- Existing IMG editing retains conservative Save As, backup and rollback behavior.

### Localization and interface

- English, Dutch, German, French and Spanish runtime localization is completed across the main workflows.
- Responsive layouts, table resizing and command placement were hardened.
- Wrapped contextual help and tooltip presentation are used across current workflows.

### Database and maintenance

- Database lifecycle handling includes health checks, backup, integrity verification, repair and rollback paths.
- Project Health and maintenance tools are report-first and explicit about preview/planning before changes.
- Runtime/package work was exercised on both Windows and Linux during the Road to 1 process.

## Safety and privacy

MIDI Manager is local desktop software. It does not upload the user's MIDI/KAR collection to MusicNote Haven. Public packages exclude private administration material, local databases, private configuration, SoundFonts and MIDI/KAR collections.

Independent backups remain recommended before major archive operations.

## Early Access

The tester recruitment phase is closed to new free-licence applicants.

The Early Access page continues as a limited launch offer for the first 50 confirmed reservations:

- Personal: €19 instead of €39
- Professional: €49 instead of €89

Reservation is not purchase; confirmation of the email address is required before the place is counted.

## Official links

- Downloads: https://musicnotehaven.ethercomm.eu/downloads/
- Windows Store: https://musicnotehaven.ethercomm.eu/downloads/windows-store/
- Public checksums: https://musicnotehaven.ethercomm.eu/downloads/SHA256SUMS.txt
- Website release notes: https://musicnotehaven.ethercomm.eu/release-notes/
- User manual: https://musicnotehaven.ethercomm.eu/manual/
- Early Access: https://musicnotehaven.ethercomm.eu/early-access/

Historical 0.3.0, 0.9.0 and 0.9.5 release notes remain preserved in this repository.
