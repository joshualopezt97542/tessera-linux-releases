# Tessera Linux Early Access — v0.6.0-beta1

**Free desktop block-puzzle game by Case Sensitive Computers, LLC.**

**Platform:** Linux x86-64. Tested on Linux Mint 22.2; Debian- and Ubuntu-family systems with compatible library dependencies are expected to be supported. Other distributions are not yet verified.

## Included now

- Endless single-player puzzle mode and deterministic Daily Challenges.
- Six themed worlds plus Original, with colored shapes and a clear-move hint.
- Drag-and-drop or select-and-click piece placement, including the final piece of a tray.
- Line-clear explosion animation with shards, shockwaves and smoke.
- Local saved game, scores, streaks, board clear tracking and revive options.
- CSC house advertisements (including optional rewarded Hint/Revive); the ad catalog is delivered from a CSC-controlled HTTPS service and does not require login.
- Bundled Java runtime; no separate Java installation required.

## Explicitly not available in this Early Access edition

- Live Duel hosting/joining and cross-platform matches; these remain in the separately tested internal preview.
- Stripe paid upgrades, including Lifetime Remove Ads and Lifetime Live Duel Hosting; these are not offered in this edition.
- Linux ARM64, Windows, Steam or Flatpak distributions.
- Email sign-in, purchase restoration, push challenge notifications and automatic updates.

The full paid cross-platform edition is under development. This free edition has **no purchases, no account requirement and no test Stripe checkout**.

## Installation (Debian-based systems)

Download `tessera-early-access_0.6.0-1_amd64.deb` and from the directory containing it run:

```bash
sudo apt install ./tessera-early-access_0.6.0-1_amd64.deb
```

Launch via the application menu under **Tessera Early Access** or run `tessera-early-access` if it is on your PATH.

For another distro, the portable archive can be extracted and run with `./run-tessera.sh` on a compatible x86-64 Linux machine. This route has not been tested on every distribution.

### Verify download integrity

Check `SHA256SUMS.txt` against the downloaded file:

```bash
sha256sum -c SHA256SUMS.txt
```

The SHA-256 list must come from the publisher's official release page rather than an untrusted download mirror.

## Data and removal

Gameplay data is saved locally under `~/.local/share/tessera-linux-early-access/`. The early-access save is separate from previous Tessera Linux developer previews.

Uninstall on Debian-based systems with `sudo apt remove tessera-early-access`. Uninstall does not automatically erase your saved games.

## Support

Visit [Case Sensitive Computers](https://casesensitivecomputers.com) for company information and support contact options. Please report crashes, unexpected placements and visual-effect issues with your Linux distribution, desktop resolution and a brief description of how to reproduce them.
