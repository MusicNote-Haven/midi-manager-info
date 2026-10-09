# MusicNote Haven MIDI Manager 1.2.2 — Linux stable release

**Linux application:** 1.2.2
**Debian package:** 1.2.2-1 for Ubuntu/Kubuntu 24.04 amd64
**Windows:** remains 1.2.1 / Microsoft Store package 1.2.1.0

## Source and package provenance

Linux 1.2.2-1 was rebuilt from clean pushed app commit `9bffe227a8f0183a549e11dd7848c55dde38de7e`. The final package is `musicnote-haven-midi-manager_1.2.2-1_amd64.deb`, size `69530872` bytes, SHA-256 `f00271a379b8f522455fa1cbf38dcc0fb9d80fc34fe98e6ac97429a09901c398`. Package metadata, release provenance and the public-package audit passed before publication.

## Durable Source Index and Technical MIDI Scan

Large source collections keep a completed Source Index as durable readiness evidence across restarts. Technical MIDI Scan reuses current analysis for unchanged contents, pure moves do not force unchanged MIDI bytes through the full pipeline again, and Stop Safely preserves completed work.

## Incremental Organizer workflow

Organizer can work with the safe current-DONE subset while Technical MIDI Scan is still finishing other files. Pending, stale and failed rows remain excluded; analyzed content must still match the current file hash.

## Library Health and manual

Library Health separates consistency checks, identical-file detection, advanced maintenance and Re-evaluate Library. The online 1.2.2 manual is available in EN/NL/DE/FR/ES and current application ? links resolve to matching manual anchors.

## Platform availability

Windows remains application 1.2.1 through Microsoft Store package 1.2.1.0. Linux is application 1.2.2, Debian package 1.2.2-1. Platform versions are intentionally independent.
