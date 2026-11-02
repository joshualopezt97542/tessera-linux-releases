# Tessera Linux Early Access — v0.6.1-beta1

**Free desktop block-puzzle game by Case Sensitive Computers, LLC.**

This is a UI readability update for the public Linux Early Access release.

## What's improved

- Theme/skin names now use **16 sp semibold text** (up from 10 sp), with extra-bold text for the selected world.
- Every theme name has a **dark translucent background** for contrast against the changing theme artwork.
- Selected themes have a **colored outline and checkmark** for easier identification.
- The world selector wraps across multiple rows to avoid clipping labels in narrower windows.
- These improvements appear wherever the world selector is shown, including **Settings**, Home and the game view.

## Still included

- Endless mode and deterministic Daily Challenges, six themed worlds plus Original.
- Mouse piece placement, clear animations, local game saves and scores.
- CSC-controlled house advertisements. No login, payment, or separate Java installation required.

## Still not included

- Live Duel, cross-platform play, Stripe purchases, ad removal, sign-in, push notifications, automatic updates and ARM64 builds.

**Platform:** Linux x86-64. Validated on Linux Mint; other distributions remain subject to compatibility testing.

## Install or upgrade (Debian/Ubuntu/Mint)

Download `tessera-early-access_0.6.1-1_amd64.deb` and run:

```bash
sudo apt install ./tessera-early-access_0.6.1-1_amd64.deb
```

This package upgrades v0.6.0-beta1; saved games remain under `~/.local/share/tessera-linux-early-access/`.

For other compatible Linux systems, extract the portable `tessera-linux-early-access_0.6.1-beta1_x86_64.tar.gz` archive, then run `./run-tessera.sh` from the extracted directory.

For download integrity, download `SHA256SUMS.txt` from the same official release and run `sha256sum -c SHA256SUMS.txt` with the downloaded files in the current directory.

**Publisher:** Case Sensitive Computers, LLC — https://casesensitivecomputers.com
