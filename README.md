# KVIK PP portal configuration

This public repository is the free, static configuration source for KVIK PP.

Edit `portals.json` whenever either IPTV portal changes. Use only the portal base URL; do not put customer usernames or passwords in this repository.

Example:

```json
{
  "portals": [
    { "name": "Portal 1", "baseUrl": "https://portal-one.example.com" },
    { "name": "Portal 2", "baseUrl": "https://portal-two.example.com" }
  ]
}
```

The Android app reads:

`https://raw.githubusercontent.com/SupMaMates/kvik-pp-config/main/portals.json`

Keep the repository public so the app can read the file without a GitHub token.

## Android app

The current release is **KVIK PP 1.1.6** (`com.kvik.perfect`). It includes the
compact Serbian portal login, transparent KVIK branding, corrected Serbian
characters, Android 4.4+ compatibility, `.ts` portal streams, and an upgraded
ExoPlayer 2.19.1 HW+ engine selected as the default decoder. Version 1.1.6
restores the original channel-list mini-player and full-screen surface sizing.

APK downloads are published under this repository's Releases section.
