## Install Packages

`apm install --packages-file ~/.atom/packages.txt`

## Export Packages List

`apm list --installed --bare > ~/.atom/packages.txt`


## Hacks

1. Replace `packages/atom-spotify2/lib/atom-spotify-status-bar-view.coffee` with `hacks/atom-spotify-status-bar-view.coffee` to show music notation for `atom-spotify2`


## Package `atom-ctags`

1. Install ctags by running `brew install ctags`
2. Add

```
alias ctags="`brew --prefix`/bin/ctags"
```

to `~/.config/fish/config.fish`

## Issue with Atom & macOS Mojave (Text too dimmed)

Fix:

```
defaults write -g CGFontRenderingFontSmoothingDisabled -bool NO
```

See https://github.com/atom/atom/issues/17486
