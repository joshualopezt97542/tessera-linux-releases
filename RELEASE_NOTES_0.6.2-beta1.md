# Tessera Linux Early Access — v0.6.2-beta1

**Free single-player desktop game · Linux x86-64 · Case Sensitive Computers, LLC**

## Improvements over v0.6.1-beta1

- In-app release checker: checks official GitHub Releases on launch, and provides a **Check for Linux updates** action in Settings. It opens the official release page; it does not download, install or execute updates on its own.
- Improved Debian 13 compatibility: bundles the required JPEG runtime library and its third-party license; package installation no longer requires the Ubuntu-specific `libjpeg-turbo8` package.
- Installer works on headless machines where desktop-menu registration is unavailable, without blocking package installation.
- Retains the larger, high-contrast theme selector labels delivered in v0.6.1-beta1.
- Earlier local saves remain under `~/.local/share/tessera-linux-early-access/`; upgrading the .deb does not intentionally reset your game.

## Features included

- Endless Mode and Daily Challenge; Original and six themed worlds.
- Desktop click-to-place and drag-and-drop pieces, hint and revive gameplay, colorful line-clear effects, scores and locally saved progress.
- CSC house ads (including optional rewarded prompts). No account, payment, or separate Java installation required.

## Limitations

- Live Duel, paid ad-removal upgrades, cross-platform multiplayer, game accounts, purchase restoration, push notifications, ARM64, Windows, and fully automatic updates are **not** available in this Early Access build.
- Compatible Debian-family systems are supported, but broader distributions and graphics drivers may require additional testing.

## Download and install

**Linux Mint / Ubuntu / Debian:** Download `tessera-early-access_0.6.2-1_amd64.deb`; in its directory run:

```sh
sudo apt install ./tessera-early-access_0.6.2-1_amd64.deb
```

**Portable Linux:** Extract `tessera-linux-early-access_0.6.2-beta1_x86_64.tar.gz`, open the extracted directory and run `./run-tessera.sh`.

**Integrity:** Download `SHA256SUMS.txt` from this official release and run `sha256sum -c SHA256SUMS.txt` from the directory containing the downloaded artifacts. Each filename must report `OK`.

## Feedback and privacy

Please report reproducible issues in [public GitHub Issues](https://github.com/joshualopezt97542/tessera-linux-releases/issues/new/choose), including distribution, resolution and the steps to reproduce the problem. Do not include access tokens or sensitive personal information.

The client requests official GitHub release metadata to check for updates; normal network logs of the client IP, headers and request time may be processed by GitHub. No Tessera account identifier is included. Local game progress stays on your device in this edition.

Privacy notice: https://www.casesensitivecomputers.com/tessera/privacy/
Publisher: Case Sensitive Computers, LLC · https://casesensitivecomputers.com
