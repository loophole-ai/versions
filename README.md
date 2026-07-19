# Loophole Versions

Update feed for [Loophole IDE](https://github.com/loophole-ai/loophole-ide).

## Structure

```
oss/{platform}/{arch}/{target}/latest.json
```

Each `latest.json` tells the IDE what the latest version is and where to download it.

## Updating

When a new version is released, update the relevant `latest.json` files with the new `productVersion` and download `url`.

---

Made by [Garv Agnihotri](https://github.com/GarvAgnihotri)