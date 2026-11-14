# StremCompat for Samsung TVs (Tizen)

Your Stremio or Nuvio account and addons on Samsung TVs with Tizen 4 and newer. Unofficial and free.

*Sua conta Stremio ou Nuvio e seus addons nas TVs Samsung com Tizen 4 ou mais novo. Não oficial e gratuito.*

> **Test versions.** Samsung support is newer than LG's and has been tried on few TVs. Please report how it went with your model in [Discussions](https://github.com/StremCompat/samsung/discussions).

## Which version?

| | **StremCompat** | **StremCompat Native** |
|---|---|---|
| | The more tested one | **Faster**, newer |
| How it is made | Web interface | The native app compiled for the TV's browser (WebAssembly) |

Both can be installed together; the native one brings your account and library from the web one on its first start.

## Install

1. Download the `.wgt` of the version you want from [Releases](https://github.com/StremCompat/samsung/releases).
2. Install it with **Tizen Studio** (Device Manager) or another tool that installs Tizen packages on a TV in developer mode. The release page has the steps.

## Compatibility

| Samsung TVs | Tizen | Status |
|---|---|---|
| 2018, N series | 4.0 | Tested on one TV |
| 2017, M series | 3.0 | Should work, not tested yet |
| 2019 and 2020, R and T series | 5.0 and 5.5 | May work, not tested |
| 2021 and 2022 | 6.0 and 6.5 | May work; these TVs can use the official Stremio app |
| 2023 and newer | 7.0 and newer | The package has to be signed again with your own Samsung certificate |
| 2015 and 2016 | 2.x | Not supported |

**Differences from LG:** torrents need a streaming server on another computer (Settings > Streaming server); debrid and direct links work without one.

StremCompat is not affiliated with Stremio, Nuvio or Samsung. If it has been useful to you, you can [buy me a coffee ☕](https://buymeacoffee.com/Alexesmm).
