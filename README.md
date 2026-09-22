# Loophole Versions

Update feed for [Loophole IDE](https://github.com/loophole-ai/loophole-ide).

## Structure

```
stable/{platform}/{version or arch}/{target}/latest.json
```

Each `latest.json` tells the IDE what the latest version is and where to download it.

### Platform Structure

**Windows:**
```
stable/win32/{version}/user/latest.json     (User installer)
stable/win32/{version}/system/latest.json   (System installer)
stable/win32/{version}/archive/latest.json  (ZIP)
stable/win32/{version}/msi/latest.json      (MSI)
```

**macOS:**
```
stable/darwin/{loopholeVersion}/latest.json
```

**Linux:**
```
stable/linux/{version}/latest.json
```

## Updating

The `loophole-builder` repository automatically updates these files when a new version is released.

## Format

```json
{
  "url": "https://github.com/loophole-ai/loophole-ide/releases/download/2.2.3/LoopholeUserSetup-x64-2.2.3.exe",
  "name": "2.2.3",
  "version": "abc123...",
  "productVersion": "2.2.3.0",
  "timestamp": 1234567890,
  "sha256hash": "abc123..."
}
```

---
