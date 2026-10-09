# MusicNote Haven MIDI Manager 1.2.1 — Windows stable release

**Windows application:** 1.2.1
**Microsoft Store package:** 1.2.1.0 for Windows Desktop x64
**Distribution:** Available through Microsoft Store
**Linux:** remains 1.1.0 / Debian 1.1.0-1

## Recognition 2.0

MIDI Manager 1.2.1 substantially strengthens the way MIDI and KAR filenames are interpreted and checked. Recognition keeps structured artist/title evidence and analysis provenance, rather than treating a filename as an unexplained final answer. Filename parsing is more resilient around karaoke suffixes, parenthetical title text, release and edition markers, guest credits, and other technical or non-identity fragments. Artist-folder evidence can corroborate a proposed identity.

When a local Music Reference Database is installed, local lookup is used first.

## Online Music Reference fallback

If local reference data cannot provide a usable match, the optional online reference fallback can query only the proposed artist and title. It does not send MIDI/KAR bytes, file paths, filenames, profile data or your collection to the online music reference service. The online service is therefore not a hidden dependency.

Strong evidence is deliberately not treated as automatic permission to rename or copy every ambiguous file. The Organizer separates independently corroborated **Auto-safe** results from **Needs Review** results. Manual corrections remain authoritative.

## Offline Music Reference Database

The optional local reference database supports high-volume and offline recognition. Installation is an explicit user action: the app downloads the selected verified snapshot, checks its SHA-256 checksum, publishes it atomically and can resume safely. It never starts a background database download on its own.

The accepted reference snapshot is `20260903-080002` and contains approximately 31,962,546 reference records. Local lookup is preferred whenever that database is available; the online fallback is only considered when the local database is absent or cannot provide a useful result.

## Re-evaluate and review

Existing libraries can be re-evaluated in place. New recognition logic can mark older analysis evidence as stale, create a durable preview and keep proposed changes reviewable before any reconciliation is applied. Re-evaluation is versioned and resumable; it does not require discarding a profile or rebuilding the database.

Recognition work uses one metadata parse per work unit, improving throughput while preserving analysis provenance. Analyzer pipeline v3, the Canonical FTS-miss correction and local lookup hot-path work reduce unnecessary work. Safe stop and recovery preserve durable progress, and list position is retained more reliably after actions.

## Organizer and safer recognition

Organization remains copy-first. Source MIDI/KAR files are not moved, renamed or deleted by normal Organizer use. You can analyse a batch, review uncertain identities, plan safe copies and execute only approved work. Saved copy-job details make completed and interrupted work inspectable.

Planning now includes all currently eligible safe copies and preserves the correct artist/filename identity. Real acceptance runs demonstrated repeated 50-file batches with clear Auto-safe versus Needs Review separation.

## Organized Library

The reset action in **Settings → Library Health** can empty the configured Organized Library after two confirmations and clears derived Organizer state without damaging the source library. Trial / Free may use this maintenance action.

## Trial / Free

Trial / Free uses the same Recognition quality as paid tiers. Analysis is not artificially capped at 25 files. The commercial limit is **100 lifetime unique successfully verified Organized Library outputs**:

- preview, analysis, review and planning consume no output slot;
- a failed copy consumes no slot;
- a duplicate or re-output of already counted content consumes no new slot;
- the 100th unique verified output is allowed;
- the 101st new unique output is blocked before copy.

The Trial boundary and saved copy accounting were verified at runtime.

## Reliability and performance

Recognition and Organizer work now avoid repeated metadata parsing within the same work unit, while local-reference hot-path and FTS-miss handling reduce unnecessary lookup work. Analyzer pipeline v3 improves throughput on larger libraries without weakening review thresholds. Safe Stop and recovery preserve durable progress across long-running analysis and organization work, and list position is retained more reliably after review and apply actions.

## UI and usability

The Light and Dark startup presentation, Dashboard and contextual feedback were refined. Library Health gives clearer routine versus advanced maintenance actions and safer preview-first feedback. Project Health newline rendering and Disk Image Creator theme-state behavior were corrected where applicable. The application continues to support English, Nederlands, Deutsch, Français and Español.

## Platform availability

Windows 1.2.1 is distributed through Microsoft Store package 1.2.1.0 for Windows Desktop x64. The Microsoft Store is the official Windows installation route; this website does not offer the Store MSIX as a direct download. Linux remains on the separately verified 1.1.0-1 Debian release until a Linux 1.2.1 artifact has been accepted.

Historical 1.1.0, 1.0.x, 0.9.x and 0.3.0 release material remains unchanged in the archive.
