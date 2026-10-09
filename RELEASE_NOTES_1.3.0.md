# MusicNote Haven MIDI Manager 1.3.0 stable release

**Windows application:** 1.3.0
**Microsoft Store package:** 1.3.0.0
**Linux application:** 1.3.0
**Debian package:** 1.3.0-1, built and accepted on Ubuntu 26.04 LTS amd64
**Accepted source:** `435fd675b18eac2e1b3efef76ba59e50ec424052`

## Availability

Windows 1.3.0 is available through the official Microsoft Store listing. The Store update was installed on the Windows 11 ZBOOK test system and runtime-accepted: startup, Settings, Version 1.3.0, the existing licence and playback all passed.

Linux 1.3.0-1 is available as the verified direct `.deb`. The final package was installed on KANTOOR and runtime-accepted with the existing Professional Version 1.x licence and playback.

## Organization analysis and identity evidence

Version 1.3 strengthens Organization analysis by reconciling filename evidence with embedded MIDI/KAR metadata instead of treating the filename as automatically authoritative. Candidate artist/title identities are checked against the installed offline music reference first. Embedded identity evidence can override a misleading filename when the evidence supports a different artist/title pair.

## Offline-first discovery and privacy

The installed local music reference is the first lookup route when it is usable. When no usable local result exists, optional Online Artist & Song Discovery can send only candidate artist/title text. MIDI/KAR bytes, local paths, filenames, collection contents and profile data are not sent.

## Truthful progress and reuse

Long-running analysis exposes phase, elapsed-time and heartbeat feedback. Verified MIDI facts and reference results are reused more effectively so repeated work avoids unnecessary parsing and lookup while preserving evidence and trust information.

## Review and correction safety

Manual artist/title/filename corrections and explicit musical approvals remain authoritative. Review and Re-evaluate workflows preserve provenance, while archive/rename handling now reconciles stale database reservations with physical filesystem truth. Real collision protection remains in place, including guarded filename-only and case-only rename behavior and rollback-safe failure handling.

## Licensing and Trial / Free

Version 1.x licences are lifetime licences and remain usable offline after successful local verification. Existing valid 1.x licences remain active across the 1.3 update.

Trial / Free allows up to 100 lifetime unique successfully verified Organized Library outputs. Analysis, planning, preview, review and failed copy operations do not consume an output slot. The 101st new unique verified output is blocked before copy.

## Release provenance

Windows Store MSIX:
- file: `MusicNote-Haven-MIDI-Manager-1.3.0.0-x64-store.msix`
- size: 67716400 bytes
- SHA-256: `abec10f30ce086532b4028069afb98e1032f508d50db2ae074e735b8bf80319c`

Linux Debian package:
- file: `musicnote-haven-midi-manager_1.3.0-1_amd64.deb`
- size: 78246750 bytes
- SHA-256: `9cf6b403f6325e774ec43abd77c595c047c4ff392a6d255d8c827fe047c58c24`

Both release packages were built from clean pushed source commit `435fd675b18eac2e1b3efef76ba59e50ec424052`.
