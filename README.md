# MusicNote Haven MIDI Manager

**MusicNote Haven MIDI Manager** is local desktop software for musicians, keyboard players, MIDI collectors and digital music archivists who manage large `.mid`, `.midi` and `.kar` collections.

## Current release status: 0.9.5

The current controlled release uses one verified application source commit for both platforms:

`71928dab173851b804b87fd72ba70d1b5585cb97`

| Platform | Current build | Public status |
|---|---|---|
| Ubuntu/Kubuntu 24.04 amd64 | `musicnote-haven-midi-manager_0.9.5-1_amd64.deb` | **Available now** |
| Windows 11 desktop/laptop | `MusicNote-Haven-MIDI-Manager-Setup-0.9.5.exe` | **Packaged runtime accepted; public installer pending code signing** |

Current public Linux artifact:

- Size: `74,159,456` bytes
- SHA-256: `b858d635592b2163d8f8a0f1ded5115d396503f223bf0bfe0d407c5226bdb70a`

The unsigned Windows 0.9.5 package is not offered as a public download. Code signing is being completed for Windows Smart App Control compatibility, and users are not asked to disable Windows security controls to install MIDI Manager.

- [Downloads and current Windows status](https://musicnotehaven.ethercomm.eu/downloads/)
- [Current public SHA-256 checksums](https://musicnotehaven.ethercomm.eu/downloads/SHA256SUMS.txt)
- [Complete website release notes](https://musicnotehaven.ethercomm.eu/release-notes/)
- [Detailed 0.9.5 GitHub release notes](RELEASE_NOTES_0.9.5.md)
- [Protected tester programme](https://musicnotehaven.ethercomm.eu/midi-manager-testers/)
- [Complete user manual](https://musicnotehaven.ethercomm.eu/manual/)

## 0.9.5 highlights

### Five-language runtime interface

Runtime localization and guidance were completed and hardened across English, Dutch, German, French and Spanish. This includes Dashboard/status text, Library Organizer, Licensing, Maintenance, First Run, FAT12/IMG and USB/Gotek report, output and error messages. Central tooltip behavior now uses wrapped rich text with a consistent maximum width.

### Large libraries and responsive UI

- Organized Library now uses incremental database-backed browsing instead of loading the full library up front.
- Runtime acceptance covered 5,375 rows with fast opening, incremental scrolling/loading, search, selection and liked-state handling.
- Dashboard cards and command rows adapt to available width.
- Database tables expose clear resizable columns with accepted width persistence.
- Playback Queue reads its library source from the database and received command/layout polish for queue workflows.

### Analysis trust, review and recovery

- Indexed records, successfully enriched/deep-analyzed files, failures and remaining work are presented as distinct states.
- Dashboard/source-index invalidation was hardened so status does not keep presenting stale analysis or source-state information after relevant changes.
- Failed-analysis and review/recovery paths keep problem files visible for inspection.
- User-facing recovery wording was simplified so the next safe action is clearer.

### MIDI device discovery

- MIDI Files by Device supports result paging for large collections.
- MIDI Type 0/1 filtering is available.
- GM2 detection and filtering are available.
- Device-oriented counts and filtering use the indexed database rather than depending on one fully materialized result view.

### Library Organizer and Playback Queue

- Library Organizer controls and status text use clearer review/execute wording and safer feedback around long-running database work.
- Large source folders may be indexed and analyzed normally. Trial/Free guidance now makes clear that the 100-file cap applies to Organized Library output, not source analysis.
- Incremental Organized Library browsing keeps search, row selection and liked-state actions available while more rows load.
- Playback Queue command rows are adaptive and its database-backed source avoids depending on a fully materialized Organized Library view.

### Floppy, IMG and Gotek workflows

- Floppy Image Studio supports FAT12 720 KB and 1.44 MB IMG creation and inspection.
- Existing IMG editing remains source-safe with Save As, verified backup and rollback behavior.
- USB/Gotek export planning remains preview-first and does not silently format or overwrite targets.
- Korg/Gotek and Roland guidance remains deliberately conservative and describes supported standard FAT12 workflows rather than claiming universal proprietary-format compatibility.
- PDF, CSV and JSON disk/catalog reports and sidecar manifests remain available.

### Safety, licensing and package integrity

- Professional users no longer see Trial/Free limit wording where it is not relevant.
- Cross-platform path/runtime behavior and remembered browse locations were validated on Linux and Windows.
- Public-package privacy auditing excludes Admin components, private keys, signing keys, local databases, private configuration, SoundFonts and MIDI/KAR collections.
- Windows Setup.exe and Linux `.deb` provenance remain tied to the same clean pushed source commit and centralized application version.
- Release-readiness validation covered Python compilation, language consistency, release/backlog/manifest contracts, package audits and targeted runtime contracts before packaging.

## Tester-driven Road to 1.0

Current tester evidence now drives the final path to:

- **Windows 1.0.0**
- **Linux 1.0.1**

No ordinary feature expansion is planned during the final tester phase. Genuine release blockers and useful tester evidence determine any remaining changes before those milestones.

Not every tester suggestion is claimed as completed in 0.9.5. Broader DAW integration, richer contextual online help, score explainability, additional device/market ideas and other post-1.0 work remain roadmap items.

## Safety and privacy

MIDI Manager runs locally and does not upload the user's MIDI/KAR collection. Normal organization is copy-first, but independent backups and small test folders remain recommended. SoundFonts are not bundled.

## Tester programme

Confirmed Early Access is required before a personal expiring test link can be requested. The protected workflow uses anti-spam and rate-limiting controls without storing raw IP addresses with reports. Newsletter consent is separate. Up to 10 manually reviewed useful reports may qualify for a free Personal licence for the 1.0 generation; signup alone is insufficient.

## Official links

- Website: https://musicnotehaven.ethercomm.eu
- Downloads: https://musicnotehaven.ethercomm.eu/downloads/
- Tester programme: https://musicnotehaven.ethercomm.eu/midi-manager-testers/
- Manual: https://musicnotehaven.ethercomm.eu/manual/
- Release notes: https://musicnotehaven.ethercomm.eu/release-notes/
- Support: musicnotehaven@ethercomm.eu

## Repository scope

This repository provides public product information for MusicNote Haven MIDI Manager. The application source repository remains private during active development and controlled testing.
