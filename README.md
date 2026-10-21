# Android Rust Files

A small, quick file manager for Android, written in Rust.

Uses little memory, starts fast, asks for as few permissions as it can, and keeps everything on the
phone. See [PRIVACY.md](PRIVACY.md).

## Features

- Browse, search, copy, move, rename and delete with progress and cancel
- Storage overview and a scan for what takes the most space
- Thumbnails for pictures and videos, natural sorting, long-press swipe select
- A 30 day trash and protection for system folders

## Install

Download the APK from the releases page and follow [docs/INSTALL.md](docs/INSTALL.md).

## Build

Needs Rust with the `aarch64-linux-android` target, `cargo-ndk`, the Android SDK (build-tools 34,
platform 34), NDK r27c and a JDK 17. Then, from `apps/files` (Windows PowerShell):

```
cargo test
powershell -File build-apk.ps1
```

APKs are signed with your own key, see [docs/SIGNING.md](docs/SIGNING.md).

## Layout

- `apps/files/` the app
- `tools/build/` the shared APK build script

## More apps

- [Android Rust Gallery](https://github.com/HusniHeartnet/android-rust-gallery)
- [Android Rust Notes](https://github.com/HusniHeartnet/android-rust-notes)
- [Android Rust Home](https://github.com/HusniHeartnet/android-rust-home)

## Licence

Copyright (C) heartnetapps. Licensed under the GNU General Public License, version 3 or (at your
option) any later version. See [LICENSE](LICENSE). The names and logos are not covered by the licence.
