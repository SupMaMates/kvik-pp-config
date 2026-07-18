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

The current release is **KVIK PP 1.1.10** (`com.kvik.pp`). It is one universal
APK for `arm64-v8a`, `armeabi`, `armeabi-v7a`, `x86`, and `x86_64`. Every
application-owned class, manifest component, remote identifier, preference,
and launcher resource is now branded as KVIK PP. Required third-party library
namespaces remain unchanged.

The app includes the compact Serbian portal login, transparent KVIK branding,
correct Serbian characters, Android 4.4+ compatibility, `.ts` portal streams,
provider-supplied Xtream channel order, and ExoPlayer 2.19.1 with HW+ selected
as the default decoder.

> **Package change:** `com.kvik.pp` is a new Android app identity. It cannot
> update an installed `com.kvik.perfect` build or automatically inherit its
> saved settings and logins.

APK downloads are published under this repository's Releases section.

## Download KVIK PP

### Direct download

[**Download the latest KVIK PP APK**](https://github.com/SupMaMates/kvik-pp-config/releases/latest/download/KVIK-PP.apk)

### Branded download page

[**pp.kvik.ovh**](https://pp.kvik.ovh)

### Downloader app

Enter this code in the Downloader app:

```text
9459698
```

Short URL: [**aftv.news/9459698**](https://aftv.news/9459698)
