# StudioZIO Probe 0.18.0 — installation

**Requirements**
- Build target: macOS 13 Ventura or later, Apple silicon and Intel (Universal app).
- Runtime tested only on Apple silicon with macOS 27. Intel, macOS 13–26, a clean Mac, and full visual UI interactions have not been tested.
- Nothing else is needed: Python is bundled, and Homebrew or Xcode is not required.

**Install**
1. Open `StudioZIO-Probe-0.18.0.dmg`.
2. Drag **StudioZIO Probe** onto **Applications**.
3. Open it from Applications. The app is signed with Developer ID and notarized by Apple. macOS may show its normal first-open confirmation.

**Use**
1. Choose a plugin under **Plugin A**, or use the bundled test fixtures, and choose a test profile (Limiter, EQ, Clipper).
2. Click **Open plugin editor**, set the plugin state, then click **Start testing**. For a comparison, use **Edit / capture A…**, **Edit / capture B…** and **Compare A and B**.
3. **Reveal evidence** opens the run folder. **Export reports…** saves HTML and JSON to a new folder you choose. **Import saved run…** reopens a previous export.

**Where data goes**
- Runs, captures and imports: `~/Library/Application Support/StudioZIO Probe/`.
- Exports: the folder you choose. Existing folders are never overwritten.

**Uninstall**
1. Delete StudioZIO Probe from Applications.
2. Optionally delete `~/Library/Application Support/StudioZIO Probe/`.

**Scope**
- Only AUv2 effects with a stereo float bus are supported.
- Results are technical measurements, not quality scores, certification or product acceptance.
- Bundled third-party software: Python 3.14.9 (PSF License), see `Contents/Resources/ThirdPartyLicenses`.
