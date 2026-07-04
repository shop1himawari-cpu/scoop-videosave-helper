# VideoSave Helper Scoop Bucket

Scoop bucket for VideoSave Helper - Video Downloader.

## Manifest

- `videosave-helper.json`
- Package name: `videosave-helper`
- Version: `2.0.2`

## Important

The current installer is a custom Windows setup EXE. This bucket manifest downloads the official installer and runs it with:

```powershell
--quiet --no-start
```

The app installs into:

```text
%LocalAppData%\VideoLatchHelper\2.0.2
```

That means this is not a fully portable Scoop-style package. It is suitable for a developer-owned bucket after testing, but a public Scoop bucket maintainer may ask for a portable ZIP or a cleaner layout.

## Install

After installing Scoop:

```powershell
scoop bucket add videosave-helper https://github.com/shop1himawari-cpu/scoop-videosave-helper
scoop install videosave-helper
```

## Uninstall

```powershell
scoop uninstall videosave-helper
```

## Local Test Result

Tested on 2026-07-04:

- `scoop install .\videosave-helper.json` succeeded.
- Hash check passed.
- Installer script ran successfully.
- Helper files appeared under `%LocalAppData%\VideoLatchHelper\2.0.2`.
- `scoop uninstall videosave-helper` succeeded.
- `%LocalAppData%\VideoLatchHelper\2.0.2` was removed by the uninstaller.
