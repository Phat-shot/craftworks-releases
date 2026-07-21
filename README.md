# AR Ops — Releases

Öffentliche Downloads für **AR Ops**, das GPS+Kompass-basierte Outdoor-Spiel
(Hide&Seek, Domination, CTF, Seek&Destroy) aus der Craftworks-Plattform.

Quellcode: [github.com/Phat-shot/craftworks](https://github.com/Phat-shot/craftworks)

> Diese Seite wird automatisch bei jedem Release (Merge auf `main`) aktualisiert.

<!-- AUTO-GENERATED:START -->
**Version:** 1.4 · **Commit:** `4b70af9` · **Stand:** 2026-07-21 12:15 UTC
<!-- AUTO-GENERATED:END -->

## Download

| | |
|---|---|
| 📱 **Handy-App (Android)** | [ar-ops-android.apk](https://github.com/Phat-shot/craftworks/releases/download/apk-android-main/ar-ops-android.apk) |
| ⌚ **Wear-OS-Companion** | [ar-ops-wear.apk](https://github.com/Phat-shot/craftworks/releases/download/apk-wear-main/ar-ops-wear.apk) |
| 🐳 **Server (Docker)** | `docker pull ghcr.io/phat-shot/craftworks:latest` |

Die APK-Links zeigen immer auf den aktuellsten `main`-Build (fester
Release-Tag, wird bei jedem Merge überschrieben) — kein manuelles
Versions-Suchen nötig. Installation: unbekannte Quellen für den Browser/
Dateimanager erlauben, APK öffnen. Selbst signiert (Android-Debug-Keystore),
kein Play-Store-Release.

## Server selbst hosten

```bash
docker pull ghcr.io/phat-shot/craftworks:latest
docker run -d -p 4000:4000 \
  -e DATABASE_URL=postgres://... \
  -e JWT_SECRET=... -e JWT_REFRESH_SECRET=... \
  ghcr.io/phat-shot/craftworks:latest
```

Die App verbindet sich standardmäßig mit dem offiziellen Server
(`arops.srz.one`) — ein selbst gehosteter Server braucht einen eigenen
APK-Build mit angepasster `SERVER_URL` (siehe Hauptrepo).
