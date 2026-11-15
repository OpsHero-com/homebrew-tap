# OpsHero Homebrew tap

Homebrew casks for OpsHero command-line tools, for macOS on Apple silicon and Intel.

## hero

`hero` is the [LaunchPlane](https://launchplane.io) command-line interface.

Install:

```bash
brew install opshero-com/tap/hero
```

Upgrade:

```bash
brew upgrade hero
```

Uninstall. Homebrew cannot remove tokens from the macOS Keychain, so sign out first, then remove the binary and the `~/.hero` settings folder:

```bash
hero auth logout
brew uninstall --zap hero
```

## How this tap is maintained

The casks in `Casks/` are written by the hero release pipeline on every release. Do not edit them by hand; a change would be overwritten by the next release. The binaries they install are published on [OpsHero-com/hero-releases](https://github.com/OpsHero-com/hero-releases/releases).
