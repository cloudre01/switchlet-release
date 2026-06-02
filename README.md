# switchlet-release

Distribution repository for **Switchlet** — a macOS menu bar app that routes http/https links to the Chrome or Firefox profile you want.

## Download

The latest signed and notarized build is on the [Releases page](../../releases).

- **macOS 13+** · Apple Silicon and Intel
- Signed with Developer ID · Notarized by Apple
- Auto-updates via [Sparkle](https://sparkle-project.org)

This repo contains the shipping build and the Sparkle appcast feed. Source code is not public.

## Install

1. Download `Switchlet.dmg` from the [latest release](../../releases/latest).
2. Open the DMG and drag `Switchlet.app` into `/Applications`.
3. Launch Switchlet and grant the default-browser permission when prompted.

## Verifying a build

Each release ships with a `.sha256` file:

```sh
shasum -a 256 -c Switchlet.dmg.sha256
```

## Reporting a problem

Open an [issue](../../issues). Include your macOS version, the build number (visible in the Switchlet menu → About), and steps to reproduce.

## Release artifacts

| File | Purpose |
| --- | --- |
| `Switchlet.dmg` | Notarized install image (manual download) |
| `Switchlet.zip` | Sparkle auto-update payload |
| `appcast.xml` | Sparkle update feed |
| `Switchlet.dmg.sha256` | DMG checksum |

## License

Switchlet is closed-source software. All rights reserved.
