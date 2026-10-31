# PORK Emulatribe 2 – Downloads

**Zum Installieren: das Setup unter [Releases](https://github.com/APOTHEKKER/emulatribe-releases/releases/latest) herunterladen und starten.**

Hier liegt kein Quellcode, nur was das Setup selbst herunterlädt:

| Ort | Inhalt |
| --- | --- |
| `version.txt` | neueste Version (`v1.26.106`), ohne Zeilenumbruch |
| `app/v<Version>/emulatribe2.exe` | die App dieser Version, daneben `.sha256` – das Setup lädt sie beim Installieren und beim Update |
| `changelogs/` | ein Changelog pro Release, Name `TT.MM.JJJJ.txt` |
| `languages/` | Sprachdateien des Setups (`de`, `es`, `fr`, `ru`) |
| `assets/` | KORG-Treiber, Schriften, WebView2-Installer und die WebView2-Laufzeit (in Teilen unter 50 MB, `.parts` = Anzahl + SHA-256) |
| Release `v<Version>` | nur das Setup `PORK-Emulatribe-2-Setup.exe` |

Veröffentlicht wird mit `npm run release` im Projekt.
