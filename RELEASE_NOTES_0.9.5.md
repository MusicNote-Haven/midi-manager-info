# MusicNote Haven MIDI Manager 0.9.5

Publication phase: 2026-08-10  
Verified application source: `71928dab173851b804b87fd72ba70d1b5585cb97`  
Release channel: controlled Road-to-1.0 release

## Platform status

| Platform | Artifact | Status |
|---|---|---|
| Ubuntu/Kubuntu 24.04 amd64 | `musicnote-haven-midi-manager_0.9.5-1_amd64.deb` | **Publicly available** |
| Windows 11 | `MusicNote-Haven-MIDI-Manager-Setup-0.9.5.exe` | **Packaged runtime accepted; public distribution pending code signing** |

### Linux 0.9.5-1

- Size: `74,159,456` bytes
- SHA-256: `b858d635592b2163d8f8a0f1ded5115d396503f223bf0bfe0d407c5226bdb70a`
- Package: `musicnote-haven-midi-manager`
- Version: `0.9.5-1`
- Architecture: `amd64`
- Upgrade/runtime acceptance: passed over the existing 0.9.0-1 package-test profile with profile/index data retained and Database Healthy.

### Windows 0.9.5

The accepted Windows 0.9.5 package was built and installed from the same source commit and passed real packaged startup/runtime testing with existing profile/index data retained, Database Healthy and application version 0.9.5 confirmed.

The public Windows installer is withheld until code signing is complete for Windows Smart App Control compatibility. Users are **not** asked to disable Windows security controls.

Accepted test-build evidence:

- Size: `49,315,906` bytes
- SHA-256: `f71bf9f0587b76f272391b477e14179e8ded0f0f74773b1d586d26a26ea8ba65`
- Signing status: unsigned / not publicly distributed

The official public checksum list intentionally contains only currently available public artifacts.

## Major changes since 0.9.0

### Five-language runtime localization

The runtime interface and user guidance were completed and hardened across English, Dutch, German, French and Spanish. Work included Dashboard/status text, Library Organizer, Licensing, Maintenance, First Run, FAT12/IMG and USB/Gotek report/output/error messages, plus consistent wrapped tooltip presentation.

### Large-library performance

Organized Library now uses incremental database-backed browsing instead of materializing the full library up front. Runtime acceptance covered 5,375 rows with fast opening, incremental scrolling/loading, search, selection and liked-state handling.

Playback Queue now reads its library source from the database and received adaptive command/layout polish.

### Responsive desktop UI

Dashboard cards and command rows were hardened for available width. Database tables expose clear resizable columns with accepted width persistence. Command-button rows were corrected across Organized Library, Disk Image Creator, Playback Queue, File Detail, Library Organizer and IMG Viewer.

### Analysis trust and recovery

Analysis-count semantics were clarified so indexed records, successful enriched/deep-analysis results, failures and remaining work are not presented as the same thing. Dashboard/source-index invalidation was hardened, failed-analysis items remain reviewable, and user-facing recovery guidance was simplified.

### MIDI Files by Device

Device discovery gained:

- result paging for large collections;
- MIDI Type 0/1 filtering;
- GM2 detection and filtering;
- database-backed counts and filtering.

### Library Organizer and Trial/Free clarity

Library Organizer controls/status wording was made clearer and safer around review/execute and long-running database work.

Trial/Free guidance now makes clear that large source folders may be indexed and analyzed normally; the 100-file cap applies to Organized Library output, not source analysis. Professional users no longer see Trial/Free limit wording where it is irrelevant.

### Floppy Image Studio, IMG and Gotek

FAT12 720 KB and 1.44 MB IMG creation/inspection remain available. Existing IMG editing retains Save As, verified backup and rollback safeguards. USB/Gotek export planning remains preview-first and does not silently format or overwrite targets. Korg/Gotek and Roland guidance remains deliberately conservative within supported standard FAT12 workflows.

### Safety and package integrity

Cross-platform path/runtime behavior and remembered browse locations were validated on Linux and Windows. Public-package privacy auditing excludes Admin components, private keys/signing keys, local databases, private configuration, SoundFonts and MIDI/KAR collections.

Release-readiness validation passed Python compilation, language consistency, release/backlog/manifest contracts, public-package audit, Linux `.deb` readiness/dry-run, Windows installer dry-run and targeted runtime contracts before packaging.

## Tester feedback and remaining roadmap

0.9.5 incorporates concrete usability and clarity improvements based on external testing, including Trial/Free behavior, Organizer wording, responsive Dashboard behavior, resizable tables and more consistent help/status presentation.

Not every tester suggestion is claimed as completed. Broader DAW integration, richer contextual online help, score explainability, additional device/market ideas and other post-1.0 work remain on the roadmap.

## Road to 1.0

The next controlled milestones are:

- **Windows 1.0.0**
- **Linux 1.0.1**

During the final tester phase, genuine release blockers and useful tester evidence guide the remaining changes.

## Official links

- Downloads and Windows status: https://musicnotehaven.ethercomm.eu/downloads/
- Current public checksums: https://musicnotehaven.ethercomm.eu/downloads/SHA256SUMS.txt
- Website release notes: https://musicnotehaven.ethercomm.eu/release-notes/
- Tester programme: https://musicnotehaven.ethercomm.eu/midi-manager-testers/
- Manual: https://musicnotehaven.ethercomm.eu/manual/
