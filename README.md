<div align="center">

<p align="center">
  <img src="docs/assets/hero.svg" alt="zinwa-q25-keyboard" width="100%" />
</p>

# zinwa-q25-keyboard

### FUTO Keyboard fork for the Zinwa Q25 — 720×720 communicator, separate app ID

[![Android](https://img.shields.io/badge/Android-keyboard-3DDC84.svg)](https://developer.android.com/)
[![Fork](https://img.shields.io/badge/upstream-FUTO%20Keyboard-89b4fa.svg)](https://github.com/futo-org/android-keyboard/)

**Device-specific build** of [FUTO Keyboard](https://keyboard.futo.org/) for the **Zinwa Q25** (40% / square 720×720 display): custom application ID, layout sizing, and flash workflow for this hardware class.

> **Upstream:** Based on Android Open Source Keyboard / LatinIME lineage. See [FUTO Keyboard](https://keyboard.futo.org/) for project philosophy (offline-first, no telemetry). This fork documents **Q25-specific deltas** only.

[Build](#build) · [Q25 changes](#q25-specific-changes) · [Upstream](#upstream--license)

</div>

---

## Q25-specific changes

| Area | This fork |
|------|-----------|
| Target device | Zinwa Q25 — 720×720 square screen |
| Packaging | Separate Android application ID from stock FUTO |
| Layout | Sizing adjustments for small square display |
| Goal | Modern offline keyboard on a communicator-class device |

---

## Build

Recursive clone (submodules required):

```bash
git clone --recursive https://github.com/shahzebqazi/zinwa-q25-keyboard.git
cd zinwa-q25-keyboard
git submodule update --init --recursive
```

Android Studio or Gradle:

```bash
./gradlew assembleUnstableDebug
./gradlew assembleStableRelease
```

Flash the appropriate variant to a Q25 (or emulator with matching resolution) per your device docs.

---

## Upstream & license

- Issues / contributions (upstream): [futo-org/android-keyboard](https://github.com/futo-org/android-keyboard/)
- License: [FUTO Source First License 1.1](LICENSE.md) (upstream); fork inherits upstream terms
- Translations: [Pontoon](https://i18n-keyboard.futo.org/) (upstream project)

---

## Related

| Resource | URL |
|----------|-----|
| Portfolio | [sqazi.sh](https://sqazi.sh) |
| FUTO layouts repo | [futo-keyboard-layouts](https://github.com/futo-org/futo-keyboard-layouts) |
