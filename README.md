# shinyawave/homebrew-tap

Homebrew tap for [**StewardAuth**](https://github.com/shinyawave/stewardauth) — a native macOS Steam Desktop Authenticator (Apple Silicon).

## Install

```bash
brew install --cask shinyawave/tap/stewardauth
```

or:

```bash
brew tap shinyawave/tap
brew install --cask stewardauth
```

## First launch (one time)

StewardAuth is ad-hoc signed and not notarized (no Apple Developer account), so
macOS Gatekeeper blocks the **first** launch. This is a one-time step — the app's
built-in updater handles versions after that:

```bash
xattr -cr "/Applications/StewardAuth.app"
```

…or right-click **StewardAuth** in Applications -> **Open** -> **Open Anyway**.

## Requirements

- macOS 12 (Monterey) or newer
- Apple Silicon (M1-M5)
