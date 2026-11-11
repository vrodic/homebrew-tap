# vrodic/homebrew-tap

## mpv

mpv built from [vrodic/mpv](https://github.com/vrodic/mpv/tree/no-quicklook-media-controls),
with one patch: on macOS, `--media-controls=no` actually turns off the Now Playing
integration. Upstream mpv always enables it, and it asks QuickLook for a thumbnail
of every file you play to use as cover art.

```sh
brew uninstall mpv            # if the homebrew-core mpv is installed
brew install vrodic/tap/mpv
echo 'media-controls=no' >> ~/.config/mpv/mpv.conf
```
