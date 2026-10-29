# homebrew-tap

Homebrew tap for Kaito Soeno's apps.

## Install

```sh
brew install --cask pockanoodles/tap/sigwald
```

Or tap it first and use the short name:

```sh
brew tap pockanoodles/tap
brew install --cask sigwald
```

## Contents

| Path | What |
| --- | --- |
| `Casks/sigwald.rb` | Sigwald, a desktop planner for your calendar, courses and goals. https://kaitosoeno.com/sigwald |
| `Formula/` | Command-line tools. Empty for now. |

## Updates

`brew upgrade --cask sigwald` installs each new release. Until releases are
signed by Apple, Sigwald can't update itself on macOS, so the cask clears the
quarantine flag on the app it just checked against its sha256.

`Casks/sigwald.rb` is a copy of `packaging/homebrew/sigwald.rb` in
https://github.com/pockanoodles/sigwald. That repo's
`scripts/release/update-manifests.mjs --tap` writes it after each release, so
change it there.
