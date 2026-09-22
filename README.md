# Loophole Versions

Update feed for [Loophole IDE](https://github.com/loophole-ai/loophole-ide).

## Structure

```
stable/{platform}/{arch}/{target}/latest.json
```

Each `latest.json` tells the IDE what the latest version is and where to download it.

### Platform Structure

**Windows:**
```
stable/win32/{arch}/user/latest.json     (User installer, e.g. x64, arm64)
stable/win32/{arch}/system/latest.json   (System installer)
stable/win32/{arch}/archive/latest.json  (ZIP)
stable/win32/{arch}/msi/latest.json      (MSI)
```

**macOS:**
```
stable/darwin/{arch}/latest.json         (DMG, e.g. arm64, x64, universal)
```

**Linux:**
```
stable/linux/{arch}/latest.json          (Tarball, e.g. x64, arm64)
```

## Updating

The `loophole-builder` repository automatically updates these files when a new version is released.

## Format

```json
{
  "url": "https://github.com/loophole-ai/loophole-ide/releases/download/2.2.3/LoopholeUserSetup-x64-2.2.3.exe",
  "name": "2.2.3",
  "version": "2.2.3",
  "productVersion": "2.2.3",
  "timestamp": 1234567890,
  "sha256hash": "abc123..."
}
```

---
