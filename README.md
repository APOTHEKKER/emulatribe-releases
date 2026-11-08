<div align="center">

# 🎛️ PORK Emulatribe 2

### Der KORG electribe 2 / electribe sampler Emulator für Windows

Synth, Sampler und Groovebox in einem – mit echten KORG-Systemen, MIDI-Anbindung an deine Hardware und originalgetreuer Bedienung.

[![Neueste Version](https://img.shields.io/github/v/release/APOTHEKKER/emulatribe-releases?style=for-the-badge&label=Version&color=e4572e)](https://github.com/APOTHEKKER/emulatribe-releases/releases/latest)
[![Plattform](https://img.shields.io/badge/Windows-10%20%2F%2011-0078D6?style=for-the-badge&logo=windows&logoColor=white)](#-download--installation)
[![Downloads](https://img.shields.io/github/downloads/APOTHEKKER/emulatribe-releases/total?style=for-the-badge&label=Downloads&color=2ea44f)](https://github.com/APOTHEKKER/emulatribe-releases/releases)
[![Sprachen](https://img.shields.io/badge/Sprachen-DE%20·%20EN%20·%20ES%20·%20FR%20·%20RU-8957e5?style=for-the-badge)](#-sprachen)

**[⬇️ Jetzt herunterladen](https://github.com/APOTHEKKER/emulatribe-releases/releases/latest)** &nbsp;·&nbsp;
[Features](#-features) &nbsp;·&nbsp;
[Systeme](#-mehrere-systeme-installieren) &nbsp;·&nbsp;
[MIDI](#-echte-electribe-per-midi-verbinden) &nbsp;·&nbsp;
[SD-Karte](#-sd-karte--dateien) &nbsp;·&nbsp;
[FAQ](#-faq)

<!--
  💡 Tipp: Hier ein Screenshot oder GIF der App einfügen, z. B.:
  <img src="assets/screenshot.png" alt="PORK Emulatribe 2" width="800">
-->

</div>

---

## ✨ Was ist PORK Emulatribe 2?

PORK Emulatribe 2 bildet die **KORG electribe 2** und den **electribe 2 sampler** am Computer nach – Bedienfeld, Display, Menüs, Pads, Regler und Touchpad inklusive. Du kannst damit komplette Tracks bauen, samplen, Patterns bearbeiten und alles mit deiner echten Hardware austauschen.

Das Besondere: Der Emulator führt auf Wunsch die **echte Firmware** des Geräts aus. Dadurch sehen Display, Menüs und Abläufe exakt so aus wie am Original – und du kannst zwischen verschiedenen Systemen wechseln, von KORG-Originalen bis zu Community-Firmwares wie **Hacktribe** und **BLECH**.

---

## 🚀 Features

| | |
|---|---|
| 🎹 **Synth & Sampler** | Beide Varianten (electribe und electribe sampler) mit allen Parts, Pattern-Sequencer, Motion Sequencing, Gate Arp, Touch Scale und Pads |
| 🔌 **Echte electribe per MIDI** | Verbinde deine Hardware per USB oder DIN: Regler, Noten, Clock und Patterns lassen sich in beide Richtungen abgleichen |
| 💿 **Mehrere Systeme** | KORG-Originalsysteme, **Hacktribe**, **BLECH (Blechtribe)** und weitere Firmwares nebeneinander installieren und wechseln |
| 💾 **SD-Karte wie am Original** | DATA UTILITY mit Export/Import von Patterns, Samples, Audio, Pattern-Sets und Chains – dieselben Dateien und Ordner wie am Gerät |
| 🔄 **System-Update wie am Gerät** | `SYSTEM.VSB` per SOFTWARE UPDATE installieren, mit den Original-Bildschirmen |
| 🎚️ **Effekte & Klang** | 38 Insert- und 32 Master-Effekte, 72 Modulationstypen, Preset-Samples, Analog-Oszillatoren, Audio In |
| 🎤 **Sampling** | Aufnehmen, Sample Edit, Time Slice, WAV-Import, Sample-Speicher als `e2sSample.all` |
| ⏱️ **Sample-genaues Timing** | Die Klangerzeugung läuft als Rust/WebAssembly-Engine im AudioWorklet |
| 📤 **Export** | Pattern-Audio, Pattern-Sets und Chains inklusive Ableton Live Set (`.als`) |
| 🌍 **Mehrsprachig** | Setup in Deutsch, Englisch, Spanisch, Französisch und Russisch |

---

## ⬇️ Download & Installation

1. Öffne die Seite **[Releases](https://github.com/APOTHEKKER/emulatribe-releases/releases/latest)**.
2. Lade **`PORK-Emulatribe-2-Setup.exe`** herunter.
3. Starte das Setup und folge den Schritten. Benötigte Komponenten (z. B. WebView2, KORG-Treiber, Schriften) lädt das Setup selbst nach.
4. Starte **PORK Emulatribe 2** und leg los.

**Updates:** Das Setup kennt die jeweils neueste Version und lädt sie beim Installieren bzw. Aktualisieren automatisch. Die Änderungen jeder Version findest du im Ordner [`changelogs/`](changelogs).

**Deinstallieren:** direkt in der App über das Menü → *Deinstallieren* oder wie gewohnt über die Windows-Einstellungen.

> **Aktuelle Version:** siehe [`version.txt`](version.txt)

---

## 💿 Mehrere Systeme installieren

Der Emulator führt die Firmware (`SYSTEM.VSB`) auf einer nachgebildeten Hardware aus (ARM926-Prozessor mit der gesamten Peripherie). Das System wird – wie am echten Gerät – über **SOFTWARE UPDATE** installiert.

| System | Beschreibung |
|---|---|
| **KORG electribe** (1.17 · 1.18 · 1.19 · 2.02) | Original-Firmware der electribe 2 |
| **KORG electribe sampler** (1.14 · 1.16 · 2.02) | Original-Firmware des electribe 2 sampler |
| **Hacktribe** | Community-Firmware mit eigener Oszillatorliste (274 Oszillatoren) |
| **BLECH / Blechtribe** | Kuhler's GELUMPE, inklusive Startbild-Funktionen (SPLASH) |

**So installierst du ein System:**

1. Lege die `SYSTEM.VSB` bzw. das KORG-Update-ZIP per **Drag & Drop** auf das Gerät, oder kopiere sie über *Menü → SD-Karte & System* auf die Karte.
2. Öffne am Gerät **SOFTWARE UPDATE** und bestätige die Installation.
3. Schalte das Gerät aus und wieder ein – der Emulator startet mit dem neuen System neu.

Identität, Dateitypen, Menüs und Funktionen (z. B. Sampling nur beim Sampler, CHAIN und UNDO ab System 2.0) richten sich danach, welches System installiert ist. Das Werks-System kannst du jederzeit über *Menü → SD-Karte & System* wiederherstellen.

> ⚠️ **Hinweis:** KORG-Firmware ist nicht Teil dieses Downloads. Lade die offiziellen Updates von [korg.com](https://www.korg.com) bzw. die Community-Firmwares bei ihren Entwicklern herunter.

---

## 🔌 Echte electribe per MIDI verbinden

PORK Emulatribe 2 kommuniziert per **Web MIDI** mit einer echten **electribe 2**, **electribe 2 sampler** oder electribe 1 über **USB oder DIN-MIDI**. Grundlage ist die offizielle *KORG MIDI Implementation*.

**Das geht:**

- **Anschlüsse** getrennt für Ein- und Ausgang wählen. Sie werden gespeichert und beim Einstecken automatisch wiedergefunden. „electribe automatisch wählen“ nimmt die richtigen Ports für dich.
- **Regler spiegeln:** Drehst du am Gerät, bewegt sich der Emulator – und umgekehrt, auch für Parts, die gerade nicht ausgewählt sind. Eine Rückkopplungssperre verhindert Endlosschleifen.
- **Noten, Controller und Clock:** Lampen und ein MIDI-Monitor zeigen den Datenverkehr. Der Emulator kann **Clock-Master oder -Slave** sein, inklusive Latenzausgleich.
- **Pattern-Wechsel** per Bank Select und Program Change.
- **Pattern per SysEx übertragen:** Patterns vom Gerät holen, im Emulator bearbeiten und zurückschreiben. Ebenso Sichern und Laden als `.syx`.

**Tipps:**

- Unter Windows hält der Standardtreiber einen USB-MIDI-Anschluss nur für **ein** Programm. Schließe andere MIDI-Programme oder wähle dort „Aus“.
- SysEx muss einmalig erlaubt werden („SysEx erlauben“).
- Dumps zum Gerät **überschreiben Patterns** in der Hardware. Sichere vorher deine Daten!

> ℹ️ Die MIDI-Anbindung folgt der offiziellen KORG-Dokumentation. Einige Details (z. B. Pattern-Zählung bei Program Change) lassen sich nur mit echter Hardware klären. Rückmeldungen und Erfahrungen sind sehr willkommen, siehe [Feedback](#-feedback--support).

---

## 💾 SD-Karte & Dateien

Die DATA UTILITY arbeitet wie am Gerät mit einer Speicherkarte und den **Original-Pfaden**. Exportierte Dateien sind byte-identisch zu den importierten – auch die KORG-Bonus-Patterns 2016 bleiben unverändert.

| Funktion | Datei / Ordner |
|---|---|
| Pattern exportieren / importieren | `KORG/electribe sampler/[Nr]_[Name].e2spat` bzw. `KORG/electribe/….e2pat` |
| Alle Patterns | `electribe_sampler_allpattern.e2sallpat` bzw. `electribe_allpattern.e2allpat` |
| Audio / Pattern-Set / Chain | WAV-Dateien plus Ableton Live Set (`.als`) |
| Alle Samples | `KORG/electribe sampler/Sample/e2sSample.all` |
| System-Update | `KORG/<Modell>/System/SYSTEM.VSB` |

Die Karte kann **intern** im Emulator liegen oder ein **eingebundener Ordner bzw. eine echte SD-Karte** sein. Über *Menü → SD-Karte & System* kannst du Dateien hinzufügen, herunterladen, löschen und die ganze Karte als **ZIP** sichern.

---

## 🔊 Klang & Technik

- **Eigene Klangerzeugung in Rust/WebAssembly** mit Analog-Oszillatoren (PolyBLEP), Sample-Stimmen, Filtern, Hüllkurven, Unison, Sync und Glide.
- **Sample-genaues Timing**: Der Sequencer plant 120 ms voraus wie das Original; jede Note wird mit ihrer exakten Zeit an die Engine übergeben.
- **Weicher Master-Limiter** statt hartem Clipping.
- **Firmware-Ausführung**: Die ARM-Firmware läuft rund 4- bis 5-mal schneller als Echtzeit. Display, LEDs, Tasten, Encoder, Regler, Pads und Touchpad verhalten sich wie am Gerät.
- **Latenz-Messung** unter *Menü → Audio & Latenz*, inklusive Rundlauf-Test über Lautsprecher und Mikrofon.

**Verbesserungen gegenüber dem Original**

- Sample-genaues Schalten von IFX On und MFX Send
- Looper und Pitch Looper nehmen das Signal schon vor dem Antippen auf
- Repeater und Roller starten taktweise neu, statt einzufrieren
- XY/LFO Phaser arbeiten tatsächlich, Short Delay hat eine begrenzte Rückkopplung
- Motion „Level“ hebt die Stummschaltung eines Parts nicht mehr auf

---

## ⚠️ Gut zu wissen

- Der **Blackfin-DSP** der Hardware ist nicht emuliert. Beim Ausführen einer Firmware übernimmt die Klangerzeugung des Emulators die Sounds des aktuellen Patterns. Der Klang ist eine **Nachbildung**, nicht bit-genau zum KORG-DSP.
- Reverbs sind algorithmisch (Freeverb-Topologie) und daher etwas dezenter als beim Original.
- Der Event Recorder schreibt ein eigenes Format. Echte `.e2sev`/`.e2ev`-Dateien werden angezeigt, aber noch nicht abgespielt.
- Der Pixel-Editor *SPLASH DRAW* von BLECH ist nicht nachgebildet. *SPLASH IMPORT* und *SPLASH RESET* funktionieren.
- Die MIDI-Anbindung wurde bisher nicht an allen Hardware-Varianten geprüft.

---

## 🌍 Sprachen

Das Setup gibt es in **Deutsch, Englisch, Spanisch, Französisch und Russisch**. Die Sprachdateien liegen im Ordner [`languages/`](languages).

---

## ❓ FAQ

<details>
<summary><b>Brauche ich eine echte electribe?</b></summary>

Nein. Der Emulator funktioniert komplett eigenständig. Eine echte electribe ist nur nötig, wenn du Regler, Noten und Patterns per MIDI abgleichen willst.
</details>

<details>
<summary><b>Wo bekomme ich die KORG-Firmware her?</b></summary>

Die offiziellen Updates gibt es kostenlos bei KORG. Sie werden nicht mitgeliefert. Das KORG-Update-ZIP kannst du direkt auf das Gerät im Emulator ziehen.
</details>

<details>
<summary><b>Kann ich mehrere Systeme parallel nutzen?</b></summary>

Ja. Du kannst unter anderem KORG-Originalsysteme, Hacktribe und BLECH installieren und zwischen ihnen wechseln. Flash-Daten (Patterns, Globals …) werden je Hardware gespeichert: rot für den Sampler, blau für die electribe.
</details>

<details>
<summary><b>Meine Patterns sind weg, was nun?</b></summary>

Gespeicherte Patterns und Samples liegen je nach Version intern in der App bzw. auf der emulierten SD-Karte. Sichere sie regelmäßig über *Menü → SD-Karte & System → Karte als ZIP sichern*. *Flash löschen* setzt den Flash-Speicher der Firmware bewusst zurück.
</details>

<details>
<summary><b>Das MIDI-Gerät wird nicht gefunden.</b></summary>

Schließe andere Programme, die den USB-MIDI-Anschluss belegen (Windows-Standardtreiber), und stecke das Gerät neu ein. Wähle dann „electribe automatisch wählen“.
</details>

---

## 💬 Feedback & Support

Fehler gefunden, Wunsch oder Erfahrung mit deiner Hardware? Eröffne ein **[Issue](https://github.com/APOTHEKKER/emulatribe-releases/issues)** und beschreibe kurz:

- Version (siehe Menü bzw. [`version.txt`](version.txt))
- installiertes System (electribe, Sampler, Hacktribe, BLECH …)
- Was du gemacht hast und was passiert ist

Gefällt dir das Projekt? Ein ⭐ auf dem Repository freut mich!

---

## 📁 Inhalt dieses Repositories

Hier liegt **kein Quellcode**, sondern nur das, was das Setup selbst herunterlädt:

| Ort | Inhalt |
|---|---|
| [Releases](https://github.com/APOTHEKKER/emulatribe-releases/releases) | das Setup `PORK-Emulatribe-2-Setup.exe` je Version |
| `version.txt` | neueste Version, ohne Zeilenumbruch |
| `app/v<Version>/emulatribe2.exe` | die App dieser Version mit `.sha256`, vom Setup bei Installation und Update geladen |
| `changelogs/` | ein Changelog pro Release, Name `TT.MM.JJJJ.txt` |
| `languages/` | Sprachdateien des Setups (`de`, `es`, `fr`, `ru`) |
| `assets/` | KORG-Treiber, Schriften, WebView2-Installer und -Laufzeit (in Teilen unter 50 MB, `.parts` = Anzahl + SHA-256) |

---

## 📜 Rechtliches

PORK Emulatribe 2 ist ein unabhängiges Projekt und steht in keiner Verbindung zu KORG Inc. *KORG*, *electribe* und weitere genannte Namen sind Marken ihrer jeweiligen Inhaber. Es wird keine KORG-Firmware mitgeliefert. Nutze nur Firmware, für die du die Rechte besitzt.

<div align="center">

<sub>Mit ❤️ für die electribe-Community</sub>

</div>
