# MusicNote Haven MIDI Manager 1.3.3 maintenance release

- **Windows application:** 1.3.3
- **Microsoft Store package:** 1.3.3.0
- **Linux application:** 1.3.3
- **Debian package:** 1.3.3-1 for Ubuntu 26.04 LTS amd64
- **Accepted shared source:** `c0b2ab8682ff9c6191acfd0354743959dc315297`

## Why this release was made

Real-world Organizer use showed that several different source filenames could contain **exactly the same MIDI/KAR file bytes**. Earlier Safe Copy planning protected against repeated source paths but could still create unnecessary, numbered byte-identical outputs in Organized Library. Version 1.3.3 closes that gap and includes targeted stability improvements.

## What improved

- The copy-first Organizer checks verified file content while **planning and executing** Safe Copies, including previously created plans. Exact duplicate content is skipped rather than copied again.
- Different MIDI arrangements or performances remain eligible when the file content differs; verified originals and source folders remain untouched.
- Organization analysis processes large result sets in bounded batches and retains Stop Safely responsiveness.
- The splashscreen resists clicks and keeps its intended dimensions.
- Linux device enumeration is more stable, protecting existing signed Professional licences when supported Python runtimes change. License verification is not weakened.

The Linux 1.3.3-1 package was installed and runtime-accepted on KANTOOR. The Windows 1.3.3.0 packaged application was launched and runtime-accepted on ZBOOKWIN. The packages share the same accepted private source commit.

## Licensing

Personal and Professional are sold as **one-time lifetime licences that include future major releases** (including 2.x, 3.x and beyond), without upgrade fees or subscriptions. Existing Version 1.x offline-safe activation is preserved; future major-version compatibility will be delivered when those versions are released. Trial / Free remains limited to 100 lifetime unique successfully verified Organized Library outputs.

## Availability

- [Official downloads](https://musicnotehaven.ethercomm.eu/downloads/)
- [Windows Microsoft Store listing](https://musicnotehaven.ethercomm.eu/downloads/windows-store/)
- [Linux Debian download](https://musicnotehaven.ethercomm.eu/downloads/linux-deb/)
- [Licensing](https://musicnotehaven.ethercomm.eu/licensing/)

## Package provenance

**Windows Store MSIX**
- File: `MusicNote-Haven-MIDI-Manager-1.3.3.0-x64-store.msix`
- Size: 67,726,441 bytes
- SHA-256: `f859da12c494f17cbde769706594ca3a9d0869071ead7522ef84c848daeb2fbc`

**Linux Debian package**
- File: `musicnote-haven-midi-manager_1.3.3-1_amd64.deb`
- Size: 76,014,084 bytes
- SHA-256: `88b948664265215fc2707663ff8cfd42587dd7b5aed18be3344ac68339634e8b`

Source code and private build records remain in private repositories. This public information repository contains no private source or licence material.
