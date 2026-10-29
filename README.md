# Plate|Fold update feeds

This repository holds the release information the [Plate|Fold](https://github.com/maxfield-allison/platefold) desktop app reads when you check for updates. GitHub Pages serves it at `https://maxfield-allison.github.io/platefold-updates/`.

- `stable.json` describes the current stable release.
- `prerelease.json` describes the newest release for people who opted into prereleases.

Both files are signed with the metadata key pinned in the app. The app refuses a file whose signature does not verify, whose validity has run out, or that offers a version older than the one installed. Each signed payload is valid for seven days. A renewal updates the issue and expiry times and signs the payload again, keeping the release information unchanged. A new version appears here only with a new release.

The installers are attached to the [main repository's releases](https://github.com/maxfield-allison/platefold/releases) and carry their own signatures, which the app checks before it installs anything.

This repository holds nothing else and takes no issues or pull requests. Report problems in the [main repository](https://github.com/maxfield-allison/platefold/issues), and security issues through its [security policy](https://github.com/maxfield-allison/platefold/security/policy).
