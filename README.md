# CUE Studio Releases

Public Sparkle update feed and release downloads for CUE Studio.

This repository hosts public release metadata and downloadable app assets only.
The application source repository is:

```text
https://github.com/muzium-emu/cue-studio
```

## Current Release

- CUE Studio v1.0.0
- DMG: https://github.com/muzium-emu/cue-studio-releases/releases/download/v1.0.0/CUE_Studio_v1.0.0.dmg
- Release page: https://github.com/muzium-emu/cue-studio-releases/releases/tag/v1.0.0

## Sparkle Appcast

```text
https://raw.githubusercontent.com/muzium-emu/cue-studio-releases/main/appcast.xml
```

## Compatibility Notes

- The macOS app is now CUE Studio.
- The existing Chrome extension remains `CUE Controller Rewire` at version `1.0.1`.
- Older CUE Controller release assets are retained only as legacy archives.

## Release Flow

1. Build and sign `CUE Studio.app` from the app repository.
2. Notarize and staple the app.
3. Package the signed DMG as `CUE_Studio_v<version>.dmg`.
4. Upload the DMG to the matching GitHub Release.
5. Generate and publish `appcast.xml` with Sparkle's `generate_appcast`.