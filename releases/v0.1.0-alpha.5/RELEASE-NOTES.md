# Albadry XRM Studio 0.1.0-alpha.5

This is an experimental Alpha release for tester feedback. Do not use it with
production Dataverse data or for business-critical work. This release includes
the forced-update and single-instance startup behavior. Once the signed Alpha
channel manifest is promoted, versions below `0.1.0-alpha.5` will be required to
update before continuing.

## Provenance

- Source repository: `Albadry-Esmat/Albadry-XRM-Studio`
- Source branch: `main`
- Source commit: `34d64528ca8204523d3d3daf8d2657f9e3a95112`
- Release workflow: built, tested, packaged, and verified locally; GitHub Actions
  is not a release prerequisite.

## Platform packages

- macOS Apple silicon (arm64): portable ZIP
- macOS Intel (x64): portable ZIP; native Intel launch was not tested
- Windows x64: portable ZIP; native Windows launch was not tested
- Linux x64: Flatpak package; native Linux installation and launch were not
  tested

Each downloadable package has a SHA-256 checksum. macOS updater archives and
their metadata are provided separately for the in-app updater.

## Validation and limitations

The source Release build, CLI build, source-generator build, and complete unit
test suite passed locally. The Apple-silicon app launched on macOS. A second
launch exited without creating a second app process. The signed update manifest
and release artifact checksums were verified locally.

Windows, Intel macOS, and Linux packages are supplied for tester feedback; they
were not natively exercised in this release. macOS packages are not Developer
ID signed or notarized. Windows packages are unsigned. Expect platform security
prompts and verify checksums before use.
