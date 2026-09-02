# Jolie-Ni/homebrew-tap

Homebrew tap for [DeskMate](https://github.com/Jolie-Ni/DeskMate).

```sh
brew install --cask jolie-ni/tap/deskmate
xattr -dr com.apple.quarantine /Applications/DeskMate.app
```

The second line is not optional. DeskMate is not notarized — that needs a paid
Apple Developer certificate — and Homebrew marks every download as quarantined,
so macOS refuses to launch it until the attribute is cleared. Homebrew 6 removed
the `--no-quarantine` flag that used to handle this at install time.

If you would rather not run that, install the DMG from
[Releases](https://github.com/Jolie-Ni/DeskMate/releases) and approve the app
once under System Settings → Privacy & Security → Open Anyway.
