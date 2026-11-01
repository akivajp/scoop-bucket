# akivajp's Scoop bucket

[![Tests](https://github.com/akivajp/scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/akivajp/scoop-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/akivajp/scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/akivajp/scoop-bucket/actions/workflows/excavator.yml)

A [Scoop](https://scoop.sh) bucket for these apps:

| App | Description |
|---|---|
| [FlexFlyout](https://github.com/akivajp/flexflyout) | A media flyout for Windows 11: cover art, title, position, playback controls and volume, sized and placed where you want |
| [rigtop](https://github.com/akivajp/rigtop) | A system monitor (terminal UI and native GUI) with storage health, GPU usage and many hosts over SSH |

## Install

```powershell
scoop bucket add akivajp https://github.com/akivajp/scoop-bucket
scoop install akivajp/flexflyout
scoop install akivajp/rigtop
```

`scoop update <app>` updates an app. The manifests follow each new release within a few hours (the Excavator workflow checks every 4 hours).

### Switching from the manifest URL

If you installed an app from the URL of its manifest (`scoop install https://raw.githubusercontent.com/...`), switch to the bucket so that updates keep coming from here. Quit the app first; the settings (in `%APPDATA%`) are kept:

```powershell
scoop uninstall flexflyout   # or rigtop
scoop bucket add akivajp https://github.com/akivajp/scoop-bucket
scoop install akivajp/flexflyout
```

## License

The manifests and the scripts are under the [Unlicense](LICENSE), as in Scoop's bucket template. The apps have their own licenses.
