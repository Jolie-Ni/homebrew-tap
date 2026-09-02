# Jolie-Ni/homebrew-tap

Homebrew tap for [DeskMate](https://github.com/Jolie-Ni/DeskMate).

```sh
brew install --cask --no-quarantine jolie-ni/tap/deskmate
```

`--no-quarantine` is doing real work, and Homebrew will warn you about it.
DeskMate is not notarized — that needs a paid Apple Developer certificate —
so without the flag macOS refuses the app as "damaged". With it, Homebrew
skips the Gatekeeper check for this download.

If you would rather not pass it, install the DMG from
[Releases](https://github.com/Jolie-Ni/DeskMate/releases) and approve the app
once under System Settings → Privacy & Security → Open Anyway.
