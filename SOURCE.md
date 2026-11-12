# Source code for third-party components

Phi Browser Framework is a compiled build of the Chromium engine with our own changes. Our own code in it is proprietary and is not published. The framework also contains third-party open source components, each under its own license. The full list, with every license text, is in [THIRD_PARTY_NOTICES.html](THIRD_PARTY_NOTICES.html).

Some of those licenses entitle you to the source code of the component. This page says where to get it.

## Which Chromium version a release is built from

Each release is built from one Chromium version. On macOS, the version number is the name of the directory inside the framework bundle:

```
Phi Framework.framework/Versions/<Chromium version>/
```

For example, the macOS framework 2.16.1 is built from Chromium 156.0.8078.93.

## Where the source is

| Component | License | Source |
|---|---|---|
| Chromium, including Blink | BSD 3-Clause, with parts of Blink under LGPL 2.1 | `https://chromium.googlesource.com/chromium/src/+/refs/tags/<Chromium version>` |
| FFmpeg | LGPL 2.1 or later | `https://chromium.googlesource.com/chromium/third_party/ffmpeg`, at the revision pinned in the `DEPS` file of that Chromium tag |
| adblock-rust (`adblock` crate 0.13.3) | MPL 2.0 | https://github.com/brave/adblock-rust |
| Every other component | See the notices file | The home page listed for it in the notices file |

## Written offer

For three years after we publish a release, we will provide, on request, the source code of the components in that release that are licensed under the GNU Lesser General Public License or the Mozilla Public License, including any changes we made to those components. Write to legal@phi.cc and name the release.

This offer covers those third-party components only. It does not cover our own code.
