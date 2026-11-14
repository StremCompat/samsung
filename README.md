# StremCompat for Samsung TVs (Tizen)

<p align="center">
  <img src="docs/assets/stremcompat-hero-en.png" alt="StremCompat home screen" width="1200">
</p>

<p align="center">
  <a href="https://github.com/StremCompat/samsung/releases"><img alt="Latest release" src="https://img.shields.io/github/v/release/StremCompat/samsung?display_name=tag&color=0F766E"></a>
  <img alt="Tizen 4 and newer" src="https://img.shields.io/badge/Tizen-4%20and%20newer-0F766E">
  <img alt="Test version" src="https://img.shields.io/badge/status-test%20version-ea345e">
  <a href="https://buymeacoffee.com/Alexesmm"><img alt="Buy me a coffee" src="https://img.shields.io/badge/support-Buy%20me%20a%20coffee-ffdd00?logo=buymeacoffee&logoColor=black"></a>
</p>

StremCompat brings your **Stremio or Nuvio** account and addons to Samsung TVs with Tizen 4 and newer, with an interface made for the remote. It is an independent, unofficial project, not affiliated with or endorsed by Stremio, Nuvio or Samsung, and it plays only what your own addons provide.

> **Test versions.** Samsung support is newer than LG's and has been tried on few TVs, so expect problems. Please tell how it went with your model in [Discussions](https://github.com/StremCompat/samsung/discussions).

## Two versions

| | **StremCompat** | **StremCompat Native** |
|---|---|---|
| Status | The more tested one | Newer, **faster** |
| How it is made | The interface as a web page | The native app (C, SDL2, OpenGL ES) compiled for the TV's browser engine (WebAssembly, with a JavaScript fallback for Tizen 4) |
| App ID | `StrmCompat.App` | `StrmCmpNtv.App` |

Both can be installed together. On its first start the native version brings your account, library and settings from the web one.

## Features

The same app as on LG ([full list](https://github.com/StremCompat/webos#features)):

- Stremio or Nuvio account with QR or email sign-in, Nuvio profiles with PINs, and Nuvio Collections as in Nuvio's apps.
- Home, Discover, Search, Library, Continue Watching, new episodes and, for Stremio accounts, a Calendar.
- Live channels from addons (such as NexoTV) and M3U lists, with what is on now and search.
- An addon store, adding addons and lists by address, typed or pasted from your phone, and organizing the rows of Home.
- Best source, source filters, subtitles and audio remembered per title, Skip intro and the next episode, video with Samsung's own player (AVPlay).
- Eleven languages.

**Differences from LG:**
- **Torrents** need a streaming server on another computer (Settings > Streaming server > Address). Debrid and direct links work without one.
- **Not available:** seek previews, technical badges on the paused screen and background trailers, which depend on FFmpeg.
- **Updates** come as a new package from Releases; the app cannot install them by itself on Samsung.

## Screenshots

The interface is the same as on LG ([more screenshots](https://github.com/StremCompat/webos#screenshots)).

<table>
  <tr>
    <td><img src="docs/assets/screens/home.jpg" alt="Home" width="100%"></td>
    <td><img src="docs/assets/screens/channels.jpg" alt="Live channels" width="100%"></td>
  </tr>
  <tr>
    <td><img src="docs/assets/screens/store.jpg" alt="Addon store" width="100%"></td>
    <td><img src="docs/assets/screens/series.jpg" alt="Series page" width="100%"></td>
  </tr>
</table>

## Installation

1. Download the `.wgt` of the version you want from [Releases](https://github.com/StremCompat/samsung/releases):
   - `StremCompat-v…-Samsung.wgt` (web version);
   - `StremCompat-Native-v…-Samsung.wgt` (native version).
2. Turn on **Developer Mode** on the TV: open Apps, type `12345` with the remote, switch Developer Mode on and enter your computer's IP address, then restart the TV.
3. On the computer, install **Tizen Studio** with the TV extensions, open **Device Manager**, connect to the TV by its IP address, and choose **Install app** with the `.wgt`.
4. On TVs with Tizen 7 and newer (2023 onwards) the package must be signed again with your own Samsung certificate (Certificate Manager in Tizen Studio) before installing.

## Compatibility

| Samsung TVs | Tizen | Status |
|---|---|---|
| 2018, N series | 4.0 | Tested on one TV (UN75NU7100) |
| 2017, M series | 3.0 | Should work, not tested yet |
| 2019 and 2020, R and T series | 5.0 and 5.5 | May work, not tested |
| 2021 and 2022 | 6.0 and 6.5 | May work; these TVs can use the official Stremio app |
| 2023 and newer | 7.0 and newer | Needs your own certificate (see above) |
| 2015 and 2016 | 2.x | Not supported |

## Troubleshooting

- **"The app service did not start":** close the app, unplug the TV for 30 seconds and open it again.
- **Torrents do not play:** set a streaming server address in Settings, or use debrid and direct sources.
- **A source does not play:** try a moderate H.264/AAC source first.

## Feedback and support

Questions and compatibility results in [Discussions](https://github.com/StremCompat/samsung/discussions), reproducible bugs in [Issues](https://github.com/StremCompat/samsung/issues). Source code: [StremCompat/stremcompat](https://github.com/StremCompat/stremcompat) and [StremCompat/native](https://github.com/StremCompat/native).

If StremCompat has been useful to you, you can [buy me a coffee ☕](https://buymeacoffee.com/Alexesmm), entirely optional.

StremCompat is licensed under [GPL-3.0](LICENSE). Stremio, Nuvio and Samsung are trademarks of their owners.
