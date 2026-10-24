# Albadry XRM Studio 0.1.0-alpha.2

This is the first main-based Alpha candidate for Albadry XRM Studio. It is
experimental, unsigned, and not notarized. It is intended for user-led
evaluation only; do not use it with production Dataverse data or for
business-critical work.

## Provenance

- Source repository: `Albadry-Esmat/Albadry-XRM-Studio`
- Source branch: `main`
- Source commit: `f09bf928afd0834fca8d5ddd27f1c377081c8138`

## Available archives

- Windows x64 portable ZIP
- macOS Apple silicon (arm64) app ZIP
- macOS Intel (x64) app ZIP
- Linux x64 portable ZIP

Each ZIP has a matching `.sha256` sidecar. Verify it before extracting or
running the package.

## Validation and limitations

The source test suite passed with 5,868 tests and no failures. The four final
archives passed checksum, ZIP-integrity, path-safety, duplicate-entry,
symlink, debug-artifact, and executable-architecture checks.

These checks do not prove native runtime compatibility. No native launch test
is claimed for any target in this Alpha packaging run. The Windows archive is
unsigned; macOS archives are unsigned and not notarized. There is no automatic
update channel.
