# Albadry XRM Studio 0.1.0-alpha.3

This draft refreshes only the macOS packages to correct the app-bundle layout
and add verifiable ad-hoc code signatures. It is an experimental Alpha for
user-led evaluation only; do not use it with production Dataverse data or for
business-critical work.

## Provenance

- Source repository: `Albadry-Esmat/Albadry-XRM-Studio`
- Source branch: `main`
- Source commit: `f09bf928afd0834fca8d5ddd27f1c377081c8138`
- Refreshed macOS archives: Apple silicon (arm64) and Intel (x64)

## Platform availability

- macOS arm64 and x64: refreshed in this draft as `0.1.0-alpha.3`.
- Windows x64 and Linux x64: continue to use the existing `0.1.0-alpha.2`
  release assets; they were not rebuilt in this macOS-only refresh.

Each macOS ZIP has a matching `.sha256` sidecar. Verify the checksum before
extracting or running the package.

## Validation and limitations

Both final ZIPs pass checksum and archive-integrity checks. Their app bundles
pass strict recursive code-signature verification and contain sealed resource
manifests. The ARM64 app was launched from its extracted ZIP and reached Help &
Support. The Intel app's architecture was inspected, but native Intel launch
was not tested.

The bundles use ad-hoc signatures only. They are not signed with an Apple
Developer ID and are not notarized; macOS may show or enforce Gatekeeper
warnings. The ARM64 smoke test restored a saved workspace and began its normal
environment connection flow. No environment operation was performed. Source
tests were not rerun for this packaging-only rebuild; the same source commit
had passed the Alpha.2 suite.
