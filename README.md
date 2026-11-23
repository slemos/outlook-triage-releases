# Outlook Triage — releases

This repository contains only signed release packages of Outlook Triage. There is no source tree or history here.

Each release has three files:

- `outlook-triage-v<version>-<commit>.zip` — the package
- `last_release.txt` — manifest (version, file name, sha256)
- `last_release.txt.sig` — Ed25519 signature of the manifest

Installations read the latest release from:

```
https://github.com/slemos/outlook-triage-releases/releases/latest/download
```

The updater verifies the manifest signature before downloading the package, then checks the package sha256 against the signed manifest.
