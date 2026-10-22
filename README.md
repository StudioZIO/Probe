# StudioZIO Probe

StudioZIO Probe measures supported stereo AUv2 audio effects on macOS. Results are technical measurements, not sound-quality scores, certification, or product acceptance decisions.

## Version 0.18.0

Download the installer and checksums from [release v0.18.0](https://github.com/StudioZIO/Probe/releases/tag/v0.18.0). See [release notes](RELEASE.md) for verification details.

This distribution bundles Python 3.14.9 and uses a universal Apple silicon / Intel build. Homebrew and a separate Python installation are not required. Measurement behavior is unchanged from 0.17.11.

| Environment or feature | Verification status |
| --- | --- |
| Apple silicon, macOS 27 | Tested on the build Mac |
| Intel x86_64 | Built; not executed |
| macOS 13–26 | Deployment target checked statically; not executed |
| Fresh Mac installation | Not tested |
| Full visual UI interactions | Not tested |
| Launch, data-folder creation, clean quit | Previously tested on the build Mac |

The original candidate passed 17 recorded checks covering bundled Python, six self-tests, fixture capture, a default run, report export/import, and unchanged bundle contents. Release packaging was subsequently sanitized; the sanitized app passes all six packaged self-tests and strict signature verification. The final app and DMG are Developer ID signed, Apple notarized, and stapled; signature, Gatekeeper, and staple checks pass. The tests do not establish compatibility with every plugin or configuration.

See [installation instructions](INSTALL.md). Data is stored in `~/Library/Application Support/StudioZIO Probe/` and in user-selected export folders.

This repository is for binary distribution and documentation. It does not grant an open-source license to StudioZIO Probe. Bundled third-party software retains its own licenses; Python notices are included in the app under `Contents/Resources/ThirdPartyLicenses`.
