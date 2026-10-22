<img src="icon-256.png" width="96" align="right" alt="">

# Roomly — downloads

Roomly is a real-time 3D social platform from [DCtech.](https://dctech.live),
available in the browser, on desktop and on Android. This repository hosts the
installers only; the source code for each release is attached to that release
(see [Source code](#source-code)).

Web version, nothing to install: **https://roomly.life/app**

## Download

| Platform | File | Where |
| --- | --- | --- |
| Windows 10/11 | `roomly-desktop-setup.exe` | [v1.8.0](https://github.com/dc-tech-inc/roomly-releases/releases/tag/v1.8.0) (latest) |
| macOS, Apple Silicon | `Roomly-1.8.0-arm64.dmg` | [v1.8.0](https://github.com/dc-tech-inc/roomly-releases/releases/tag/v1.8.0) |
| macOS, Intel | `Roomly-1.8.0-x64.dmg` | [v1.8.0](https://github.com/dc-tech-inc/roomly-releases/releases/tag/v1.8.0) |
| Linux x86_64, any distro | `Roomly-1.8.0-anylinux-x86_64.AppImage` | [v1.8.0](https://github.com/dc-tech-inc/roomly-releases/releases/tag/v1.8.0) |
| Linux x86_64, Debian/Ubuntu | `roomly-desktop_1.8.0_amd64.deb` | [v1.8.0](https://github.com/dc-tech-inc/roomly-releases/releases/tag/v1.8.0) |
| Linux x86_64, Flatpak | `life.roomly.RoomlyDesktop_stable_x86_64.flatpak` | [v1.8.0](https://github.com/dc-tech-inc/roomly-releases/releases/tag/v1.8.0) |
| Linux ARM64 | `Roomly-1.7.0-anylinux-aarch64.AppImage`, `roomly-desktop_1.7.0_arm64.deb`, `life.roomly.RoomlyDesktop_stable_aarch64.flatpak` | [v1.7.0](https://github.com/dc-tech-inc/roomly-releases/releases/tag/v1.7.0) |
| Android | [`Roomly-android.apk`](https://github.com/dc-tech-inc/roomly-releases/releases/download/android/Roomly-android.apk) (sideload; always the newest build) | [android](https://github.com/dc-tech-inc/roomly-releases/releases/tag/android) |

Linux ARM64 builds are currently only available up to v1.7.0; v1.8.0 ships
Linux x86_64, Windows and macOS.

Not sure which Mac you have? Apple menu → **About This Mac**: "Apple M1/M2/..."
is Apple Silicon, "Intel" is Intel.

## Unsigned installers

The installers are not code-signed yet, so Windows and macOS show a warning.

- **Windows (SmartScreen):** click **More info**, then **Run anyway**.
- **macOS (Gatekeeper):** try to open the app once and dismiss the warning. Then open
  **System Settings → Privacy & Security**, scroll down, click **Open Anyway**,
  and confirm with **Open**. Only needed the first time. See Apple's guide,
  [Safely open apps on your Mac](https://support.apple.com/en-us/102445).

## Auto-update

The desktop app updates itself through
[`update.electronjs.org`](https://update.electronjs.org), which reads the
latest release from the public GitHub API. That is why this repository is
public. The `RELEASES`, `.nupkg`, `.zsync` and darwin `.zip` files are
updater files; you do not need to download them.

## Source code

Each release attaches `roomly-desktop-<version>-src.tar.gz`, the complete
corresponding source of the Roomly Desktop app in that release, licensed under
the GNU AGPL-3.0. Each archive is made with `git archive` from the source commit
that built the binaries. It has the sources, build scripts, `forge.config.ts`,
the GitHub workflows, the lockfile and the build guide in `README.md`. It has no
git history. v1.5.3 mixes several commits; its release notes map each asset to
its commit.

Every release also attaches a `SHA256SUMS` file. To verify a download, put the
archive and `SHA256SUMS` in the same folder and run:

```sh
sha256sum -c SHA256SUMS
```

## License and credits

Roomly Desktop is distributed under the GNU Affero General Public License
v3.0. It is a fork of
[`stoatchat/for-desktop`](https://github.com/stoatchat/for-desktop) by Pawel
Makles.
