# homebrew-tap

Homebrew tap for Kaito Soeno's apps.

## Install

```sh
brew install --cask pockanoodles/tap/erwin
```

Or tap it first and use the short name:

```sh
brew tap pockanoodles/tap
brew install --cask erwin
```

## Contents

| Path | What |
| --- | --- |
| `Casks/erwin.rb` | Erwin, a desktop planner for your calendar, courses and goals. https://kaitosoeno.com/erwin |
| `Formula/` | Command-line tools. Empty for now. |

## Updates

Erwin updates itself. `brew upgrade --cask --greedy erwin` also works.

`Casks/erwin.rb` is a copy of `packaging/homebrew/erwin.rb` in
https://github.com/pockanoodles/erwin. That repo's
`scripts/release/update-manifests.mjs --tap` writes it after each release, so
change it there.
