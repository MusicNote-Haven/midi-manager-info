# MusicNote Haven MIDI Manager 1.1.0

Publication date: 2026-08-23

| Platform | Application version | Package | Status |
|---|---:|---|---|
| Windows | **1.1.0** | Microsoft Store package `1.1.0.0` | **Available in Microsoft Store** |
| Linux | **1.1.0** | Debian package `1.1.0-1` | **Verified direct download** |

Both platforms are based on accepted release source `2f2255fb38610c59913f78c0ebe24a4ed46ef0b6`.

## Verified release artifacts

### Windows 1.1.0

- Distribution: Microsoft Store
- Store product ID: `9P9PKX8XNDWF`
- Store package version: `1.1.0.0`
- Architecture: `x64`
- Submitted Store-package SHA-256: `d25b1733aba05a99acd88e9eabb5b3e607c268a1906e3b36bf5d8cc73e0e7038`
- Status: available through the existing official Microsoft Store listing
- Microsoft Store manages package signing and delivery.

### Linux 1.1.0-1

- Artifact: `musicnote-haven-midi-manager_1.1.0-1_amd64.deb`
- Size: `67,927,402` bytes
- SHA-256: `beff31a2ad1a9687f0fa379829be2acc73f4a8674bad79f114c14f27dfa3116e`
- Architecture: `amd64`
- Public-package audit: passed with no reported problems
- Upgrade acceptance: in-place `1.0.1-1` → `1.1.0-1` passed; the installed runtime showed Version 1.1.0 and retained the existing package-test profile, configured paths and settings.

## Changes since the 1.0 production generation

## Professional product shell and new branding

- Navigation is now organized around Dashboard, Analyze, Review, Organize, Library, MIDI Player, Floppy Image Studio and Settings, with the former scattered functions grouped under clear product destinations.
- The sidebar, splash screen and website use the new approved MusicNote Haven MIDI Manager branding with coordinated Dark and Light assets. Settings has the proper gear icon and the sidebar includes a direct full-manual link.
- Dashboard is an information cockpit rather than a launcher. Duplicate analysis-summary content was removed and the remaining cards use clearer semantic green/orange/red status cues.
- Initial Dashboard work no longer leaves the interface looking frozen: noticeable startup/refresh waits get localized “Please wait…” feedback while fast work remains unobtrusive.

## Search, filters and large-library browsing

- Typing in the main search fields no longer starts database/filesystem searches on every keystroke. Search is executed explicitly with Search or Enter, reducing accidental expensive work on large libraries.
- Library search is case-insensitive and tolerant of common Latin diacritics, and the shared search/index foundations cover filename/path, artist/title identity evidence, genre and stored lyrics where available.
- Library → Organized Library keeps incremental database-backed browsing for large collections and now combines compact details, shared advanced filters, explicit search controls, liked state and playback actions in the professional shell.
- Search result materialization and busy feedback were hardened so large result sets can be presented without a blank or apparently unresponsive interface.
- Shared structured filters now make it easier to narrow the Organized Library by device/mode evidence, performance/content characteristics, structure/analysis characteristics, liked state and genre without creating separate competing search screens.
- Ordinary data tables use typed header sorting where row order is only presentation; workflow-order tables such as playback positions and floppy/IMG slots deliberately keep their semantic order.

## Recognition, identity evidence and re-evaluation

- The recognition/identity layer now keeps structured artist/title evidence and provenance instead of reducing every result to an opaque name guess.
- Existing libraries can be re-evaluated in place through Library Health workflows. Users do not need to create a new profile or throw away the existing database just to apply newer analysis/recognition logic.
- Re-evaluation tracks old trust/provenance as stale when appropriate, prepares a persistent preview and keeps changes reviewable before any name/folder reconciliation is applied.
- Targeted reanalysis paths connect Review, File Detail and maintenance actions so repaired or questionable files can be reassessed without blindly rebuilding the entire collection.
- File Detail brings the current recognition identity, analysis evidence and content provenance together so the user can inspect why a value or identity is present before choosing a corrective action.
- Compatibility evidence remains explicit: GM/GS/XG modes and manufacturer/device signals are exposed as evidence for filtering and review rather than being treated as an unexplained opaque label.

## Lyrics and content enrichment

- Lyrics are now first-class local database content rather than only transient MIDI text. Embedded MIDI/KAR lyrics can be extracted and stored with source/provenance information.
- Adjacent local .txt/.lrc lyrics, manual paste/edit and per-file Lyrics workflows are supported, including synced-text metadata when it is available.
- A provider-neutral, user-configured HTTP/HTTPS JSON adapter can perform an explicit lookup by artist/title/filename/query, show the result for review and save only after user approval with provenance.
- Lyrics enrichment is available both per file and through maintenance-oriented workflows, so a long-lived library can be enriched without requiring files to be reorganized again.
- Search/filter integration can use stored lyrics and lyric-state metadata where available, while 'no lyrics' remains distinct from 'not yet classified/indexed'.
- MIDI Manager does not bundle a commercial lyrics provider or scraper. Provider access/rights remain the user’s responsibility, and provider-specific commercial integration is not claimed as part of 1.1.0.

## Review and Organizer safety/recovery

- Review Queue, Failed analysis and File Detail provide clearer reassessment paths and keep failures visible instead of hiding them or retrying endlessly.
- Organizer copy planning, approval and execution remain separate. Normal organization is copy-first, with planned targets visible before execution and verification after copies are created.
- Long Organizer operations received safer cancellation/progress and stronger busy-state/navigation handling so users can see what is running and stop only at defined safe points.
- Deterministic recovery support can inspect unfinished Organizer work, distinguish already verified copies from conflicts and resume/repair internal state without casually overwriting source MIDI/KAR files.

## Library Health and maintenance

- Settings now exposes a dedicated Library Health tab. Routine Library Health actions are separated from Advanced maintenance groups for Database, Organized Library check, Library intelligence & metadata, Organized Library planning and Archive & cleanup.
- Database Hygiene and Organized Library planning use preview/report-first workflows. The refreshed manual shows the exact visible action names, including Settings → Library Health → Organized Library planning → Preview.
- Refresh analysis database can re-run current analysis over existing indexed records with protected backup/transaction behavior while preserving the user profile and database rather than forcing a new setup.
- Database schema, hygiene, genre-cache and maintenance-report foundations were expanded and localized. Permanent archive/delete/compaction actions remain safety-sensitive and are not presented as automatic background cleanup.
- Library Health separates normal user tasks from support/developer diagnostics. For example, Project Health is a support diagnostic rather than a normal user-facing menu destination.
- Archive/cleanup lifecycle work follows archive-first safety: physical source/Organized Library files are not silently deleted as a side effect of database maintenance.

## Playback and shared controls

- Playback ownership is centralized so one MIDI playback session drives the visible controls across playback-capable views instead of individual screens silently owning competing processes.
- Pause/Stop behavior is synchronized across the MIDI Player, Organized Library, Review/File Detail and related playback views; a newly started session can replace the previous one without stale controls continuing to target it.
- FluidSynth discovery/process lifecycle and application shutdown handling were hardened, while the user-selected SoundFont remains external to the package.

## Usability, tooltips and contextual help

- A native Qt design-system foundation defines consistent spacing, compact table density, delayed busy feedback, action limits and focusable context-help controls without adding a web-style runtime dependency.
- Application tooltips are bounded and word-wrapped centrally, including item-view tooltips, so long translated explanations no longer create extremely wide popups. Tooltip lifecycle handling was hardened for dynamically replaced widgets.
- Question-mark help controls are keyboard-focusable and deep-link to the matching online manual topic. Legacy help routes remain compatible where needed.
- Adaptive command rows and button/label sizing reduce clipping in translated interfaces and on narrower windows.
- Shared delayed operation feedback avoids flashing overlays for very short tasks but explains perceptibly long searches, loads and maintenance operations.
- Dynamic widgets are replaced cleanly during language/UI refreshes so stale translated controls do not linger in the live hierarchy.

## Licensing, limits and customer guidance

- Licensing wording now distinguishes Trial / Free, Personal and Professional more clearly. Trial / Free can work with large source collections; the 100-file limit applies to Organized Library output rather than source indexing/analysis.
- Professional Organized Library capacity is shown as Unlimited where appropriate instead of exposing Trial/Free limit semantics to paid tiers.
- Purchase/upgrade and support/device-transfer destinations were clarified, and user-content responsibility guidance was added for lyrics/MIDI material supplied by the user.

## Localization, privacy and reliability hardening

- English, Dutch, German, French and Spanish remain aligned across the professional shell, maintenance actions, reports/status text, lyrics workflows, Floppy Image Studio and context help.
- Public screenshots for 1.1.0 were rebuilt against the final interface. Customer identity, licence keys, Device IDs, device bindings and private local paths are redacted before publication.
- Release/package contracts, public-package privacy audits and exact artifact provenance were tightened. The Linux package audit passed with no reported problems, and Windows/Store packaging derives from the same accepted 1.1.0 source.
- Both platforms now share application version 1.1.0; platform package formats remain Microsoft Store 1.1.0.0 and Debian 1.1.0-1.
- Floppy Image Studio remains fully integrated in the 1.1 shell, including the Disk Image basket/creator, Single IMG, Folder Catalog and Reports workflows; their visible labels, status text and contextual guidance are aligned across the five supported languages.

## Platform acceptance and upgrade behavior

- Linux 1.1.0-1 was installed as an in-place upgrade over 1.0.1-1. The installed runtime showed Version 1.1.0 and retained the existing package-test profile, configured paths and settings.
- Windows 1.1.0 was built as Microsoft Store package 1.1.0.0 from the accepted 2f2255f release source and is now available through the existing official Store listing.
- Historical 1.0.x, 0.9.x and 0.3.0 checksums and release records remain preserved rather than being rewritten with 1.1 facts.

## What is deliberately not part of 1.1.0

- The planned replaceable local MusicBrainz reference cache is a post-1.1 project and is not bundled in this release.
- Provider-specific bundled lyrics services remain rights/commercial-terms gated. 1.1.0 ships the local/user-supplied/provider-neutral workflow, not a bundled scraping service.
- Future MIDI Studio editing features and wider MIDI-repair/version-consolidation work remain later roadmap items; the current explicit playback destination remains MIDI Player.

## Safety and privacy

MIDI Manager is local desktop software. It does not upload the user's MIDI/KAR collection to MusicNote Haven. Keep independent backups before large archive/cleanup operations and review preview/planning reports before applying changes. Public screenshots intentionally hide private customer/licence/device values and local paths.

## Official links

- Downloads: https://musicnotehaven.ethercomm.eu/downloads/
- Windows Store: https://musicnotehaven.ethercomm.eu/downloads/windows-store/
- Checksums: https://musicnotehaven.ethercomm.eu/downloads/SHA256SUMS.txt
- User manual: https://musicnotehaven.ethercomm.eu/manual/
- Release notes: https://musicnotehaven.ethercomm.eu/release-notes/

Historical 1.0.x, 0.9.x and 0.3.0 release records/checksums remain preserved.
