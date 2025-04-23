# redstar upscaler
Leistungsstarkes Video-Upscaling-Tool mit FFmpeg, Real-ESRGAN, Flowframes - unterstützt jetzt **mehrsprachige UI**!

🌐 Sprache:
[한국어](https://github.com/redstar-programmer/upscaler/blob/main/README.md) | [English](https://github.com/redstar-programmer/upscaler/blob/main/README/README.en.md) | [日本語](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ja.md) | [中文](https://github.com/redstar-programmer/upscaler/blob/main/README/README.zh.md) |
[Français](https://github.com/redstar-programmer/upscaler/blob/main/README/README.fr.md) | [Deutsch](https://github.com/redstar-programmer/upscaler/blob/main/README/README.de.md) | [Español](https://github.com/redstar-programmer/upscaler/blob/main/README/README.es.md) | [Português](https://github.com/redstar-programmer/upscaler/blob/main/README/README.pt.md) |
[Русский](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ru.md) | [Italiano](https://github.com/redstar-programmer/upscaler/blob/main/README/README.it.md) | [Tiếng Việt](https://github.com/redstar-programmer/upscaler/blob/main/README/README.vi.md) | [Bahasa Indonesia](https://github.com/redstar-programmer/upscaler/blob/main/README/README.id.md) |
[ภาษาไทย](https://github.com/redstar-programmer/upscaler/blob/main/README/README.th.md) | [العربية](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ar.md)

<p align="center">
  <img src="https://github.com/user-attachments/assets/632c3a83-5416-46c3-8d38-0e1bf153b633" height="250"/>
</p>

<p align="center">
  <strong>Video-Upscaling-Tool basierend auf fmpeg, realesrgan, flowframes</strong><br>
  <em>Moderne GUI-basierte, voreingestellte Einstellungen, Unterstützung für Multi-File-Verarbeitung</em>
</p>

---.

Download: [Release](https://github.com/redstar-programmer/upscaler/releases/)

## ✨ Bitte unterstützen Sie 'redstar' Upscaler

Gefällt Ihnen dieses Projekt oder möchten Sie seine Entwicklung unterstützen?
Machen Sie eine kleine Spende, um uns zu helfen, bessere Funktionen und zuverlässige Updates zu entwickeln!

- <img src="https://img.shields.io/badge/Donate-PayPal-blue.svg?logo=paypal" height="20"/><br>**PayPal** : [https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR](https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR)
- <img src="https://img.shields.io/badge/Sponsor-GitHub%20Sponsors-ff69b4?logo=githubsponsors" height="20"/><br>**GitHub-Sponsoren** : [https://github.com/sponsors/redstar-programmer](https://github.com/sponsors/redstar-programmer)


> 💡 Ihr Sponsoring von Serverkosten, Entwicklungszeit und einer Tasse Kaffee hilft uns sehr weiter. Vielen Dank dafür!

## Inhaltsverzeichnis

- [👋 Einführung](#Einführung)
- [💾 Installation und Vorbereitung](#Installation-undVorbereitung)
- [🔧 Hauptmerkmale](#Main-Features)
- [🚀 Hinweise zur Verwendung (Schnellstart)](#How-to-use-quick-start)
- [⚙️ Detaillierte Funktionsbeschreibung](#detailed-feature-description)
- [🙏 Danksagungen](#Acknowledgements)
- [📜 Geschichte](#Geschichte)

## 👋 Einleitung
**Redstar Upscaler ist ein Python-basiertes GUI-Tool zum automatischen Hochskalieren von Videos auf höhere Auflösungen unter Verwendung von "ffmpeg", "Real-ESRGAN" und "Flowframes".

- Extrahieren von Videoframes → Hochskalieren → Zusammenführen von Videos in einem Schritt
- Unterstützt verschiedene Realsrgan-Modelle
- Optionale Interpolation über Flowframes
- Automatische Extraktion und Verarbeitung von Audiocodecs
- Arbeit am Quellort oder an einem bestimmten Pfad

> ⚠️ Entwickelt und getestet in einer Windows-Umgebung.

Nachfolgend finden Sie eine einfache Anwendungsdemo, klicken Sie darauf, um zu YouTube weitergeleitet zu werden:<br>
[![Watch the demo](https://img.youtube.com/vi/G-JTWRws3co/0.jpg)](https://youtu.be/G-JTWRws3co "Watch on YouTube")

## 💾 Installation und Vorbereitung

1. Installieren Sie die folgenden externen Tools (beachten Sie, dass die Distributionsdatei ffmpeg, Real-ESRGAN und Flowframes-Installationsdateien enthält (siehe Ordner "Programme" im Pfad)) und suchen Sie diese.
   - [ffmpeg](https://www.ffmpeg.org/download.html)
   - [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN/releases)
   - [Flowframes](https://github.com/n00mkrad/flowframes) *(optional)*.
2. entpacken Sie readstars upscaler.exe und führen Sie es aus
3. Im Falle von Flowframes können die geladenen Modelle je nach Umgebung unterschiedlich sein. Starten Sie daher Flowframes und stellen Sie sicher, dass die Interpolation AI und AI Model in der Registerkarte Interpolation mit der Version von resources/flowframes_models.ini von redstar upscaler übereinstimmen. <br>Kommentieren Sie die nicht geladenen Modelle aus, indem Sie sie mit # markieren und stellen Sie sicher, dass die Reihenfolge der Modelle im Einstellungsfenster von redstar upscaler mit der Reihenfolge der Modelle in <br>Flowframes übereinstimmt, bevor Sie fortfahren.

## 🔧 Hauptmerkmale.

![Image](https://github.com/user-attachments/assets/93dc232e-8742-4ae3-b335-9395c26a61f4)
- ✅ Mehrfache Videoauswahl und sequenzieller Betrieb
- ✅ Hinzufügen von Drag/Drop-Videos
- ✅ Verfügbarkeit der Hauptprogramme und direkte Auswahl
- Disc-Spar-Modus
- ✅ Mehrsprachige Unterstützung (15 Sprachen)
<br><br>
![Image](https://github.com/user-attachments/assets/3341f4ca-af20-4647-93d0-484146dc6757)
- Speichern Sie Voreinstellungen und wenden Sie sie automatisch an
- Automatische Audiocodec-Erkennung und Bitrateneinstellung
- Automatische Erkennung und Auswahl von Realesrganmodellen
- ✅ Detaillierte Einstellungen für FFMPEG, real-ESRGAN und Flowframes
- ✅ Änderung der Optionseinstellungen je nach Flowframes-Version<br>(Die Version kann durch Angabe des Versionspfades in Flowframes auf der Hauptseite geändert werden)
<br><br>
![Image](https://github.com/user-attachments/assets/25d60d82-53a2-4064-bbef-d439d9a9d3d6)
- ✅ Überprüfen Sie den Befehl zur Ausführung von Upscale (kann kopiert und separat auf CMD ausgeführt werden)
<br><br>
![Image](https://github.com/user-attachments/assets/2fd69862-d038-401d-a9a6-83dc84c769f0)
- Überwachen Sie den Gesamtfortschritt des Upscale-Vorgangs
- ✅ Überprüfen der Upscale-Protokollierung (Protokolldateien werden nach Datum im Protokollordner im Live-Ordner erstellt)
- Automatisches Bereinigen der Ergebnisse nach Abschluss des Auftrags (mit dem Präfix [REDSTAR])
- ✅ Aktion nach Aufgabenabschluss festlegen<br>(Nichts tun / Programm beenden / Ruhezustand / Fenster schließen)
<br><br>
## 🚀 Wie man es benutzt (Quick Start)

1. Videodateien hinzufügen (MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV unterstützt)
2. Geben Sie den Arbeitsspeicherort an oder aktivieren Sie das Kontrollkästchen "Originaldateipfad verwenden".
3. Klicken Sie auf die Schaltfläche "Einstellungen" für das hinzugefügte Video
4. ffmpeg, realESRGAN, Flowframes detaillierte Einstellungen
5. Klicken Sie auf "Batch apply to all files / Apply to selected files only".
6. Klicken Sie auf die Schaltfläche "Bestätigen".
7. Überprüfen Sie die auszuführenden Befehle und klicken Sie auf die Schaltfläche "Task starten".

> Das Ergebnis des Auftrags sind zwei Dateien: hochskaliertes Video und interpoliertes Video im ausgewählten Ordner.
> ✨ Die fertigen Dateien werden mit dem Präfix [REDSTAR] gespeichert.
---]

## ⚙️ Detaillierte Funktionsbeschreibung

| Element | Beschreibung |
|------|------|
| **Arbeitspfad festlegen** | Standardpfad oder Option "Originaldateipfad verwenden" bereitstellen |
| **Unterstützung von Videoformaten** | Die meisten Formate werden unterstützt, darunter MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV usw.
| **Upscale-Modelle** | Erkennt automatisch realesr-animevideov3, realesr-general, 4xplus, etc.
| **Audioverarbeitung** | Unterstützung für die Kodierung verschiedener Formate wie `aac`, `mp3`, `flac`, usw.
| **Flowframes-Integration** | Interpolation (FPS ×2, ×4, ×8) kann eingestellt werden
| **Disk Saving Mode** | Automatische Löschung von Zwischenbildern

## 🙏 Danksagungen

- realesrgan von [xinntao](https://github.com/xinntao/Real-ESRGAN)
- flowframes von [n00mkrad](https://github.com/n00mkrad/flowframes)
- Wenn Sie zu diesem Projekt beitragen oder eine Funktion vorschlagen möchten, hinterlassen Sie bitte einen Kommentar unter [Issues](https://github.com/redstar-javscraper/redstar_upscaler/issues).

# 📜 Geschichte

v 1.1.0
 > 1. Menükonfiguration (Datei öffnen, Datei schließen, Log-Einstellungen, Spracheinstellungen)
 > 2. mehrsprachige Einstellungen hinzugefügt (verfügbare Sprachen: Koreanisch, Englisch, 日本語, 中文, Français, Deutsch, Español, Português, Русский, Tiếng Việt, Bahasa Indonesia, ไทย, Italiano, العربية)
 > 3. geänderte Meldungen und etwas Code, um die hinzugefügten Spracheinstellungen zu berücksichtigen
 > 4. einige Änderungen an der UI-Konfiguration
 > 5. ffmpeg, real-ESRGAN, Flowframes Versionsinformationen werden angezeigt (Hauptbildschirm)
 > Unterstützung der Flowframes-Version 1.41.0 (derzeit sind nur die Versionen 1.40.0 und 1.36.0 verfügbar, da der cmd-Befehl in der Version 1.41.0 nicht funktioniert)
 > 7. ein Problem behoben, bei dem AI-Modelle in Kleinbuchstaben angezeigt wurden
 > 8. zusätzliche FFMPEG-Optionen (Pixel, Videocodec) - die Optionen werden je nach PC des Benutzers angezeigt
 > 9. verbesserte CUDA-Prüfung für jeden Benutzer-PC - Überprüfung der Verfügbarkeit und des GPU-Typs (Hauptbildschirm)

v 1.0.0
 > 1. komplette Überarbeitung des Codes
 > 2. änderungen an der Benutzeroberfläche
 > 3. die Bandbreite der verarbeitbaren Videos/Audios wurde erhöht
 > 4. zusätzlicher Disk-Spar-Modus
 > 5. der Vertrieb umfasst die wichtigsten Programme

v 0.1.92
 > 1. behebt ein Problem, das dazu führte, dass die Interpolation aufgrund von doppelten Einträgen in der AI-Modell-Combobox fehlschlug, wenn der Flowframes-Pfad geändert wurde.
 > 2. ein Prüfcode für den Auswahlstatus der Combo-Box beim Interpolieren hinzugefügt.

v 0.1.91
 > 1. einige Funktionen zur Aktualisierung von Comboboxen in Verbindung mit Flowframes hinzugefügt
 > 2. einige Verteilungsdateien angepasst

v 0.1.9
 > 1. Änderungen am Flowframes-Modell übernommen
 > 2. neues Flowframes 1.36.0 Modell, 1.40.0 Modell Implementierung
 > 3: Flowframes-Befehlszeilenfehler treten nicht mehr auf
 > 4: Dateien können jetzt durch Ziehen/Ablegen hinzugefügt werden
 > 5: Flowframes-Einstellungen werden nicht mehr übernommen

v 0.1.8
 > 1. behobener Fehler bei der Versionsprüfung
 > 2. wenn Flowframes im Standardpfad installiert ist (z.B. C:\Benutzer\Administrator\AppData\Local\Flowframes\), muss der Pfad vor dem Start als Standard festgelegt werden.
 > 3. beim Hinzufügen mehrerer Dateiauswahlen stürzt die Anwendung aufgrund eines Fehlers ab.
 > 4. ein Fehler beim Starten der Aufgabe nach dem Hinzufügen mehrerer Dateien wurde behoben

v 0.1.7
 > 1. die Programmgröße kann geändert werden
 > 2. behobener Fehler bei der Arbeit mit Dateien ohne Stimme
 > 3. die gesamte UI-Konfiguration wurde geändert (neu konfiguriert, um die Größenänderung zu berücksichtigen)

v 0.1.6
 > 1. behobenes Problem mit unterschiedlichen Schriftgrößen je nach Bildschirmauflösung
 > 2. ein Problem behoben, bei dem der Programmtitel die Versionsinformationen nicht als neue Version anzeigte
 > 3. ein Problem wurde behoben, bei dem die Datei config.ini in einem anderen Pfad gespeichert wurde
 > 4. wenn der Realesrgan-Upscaling-Multiplikator geändert wird, wird auch das Upscaling-Modell-Kombinationsfeld geändert.
 > 5. die Funktion zur Überprüfung der Aktualisierung wurde hinzugefügt
 > 6. einige Logikfehler behoben
 > 7. die Farbe der Auflösungs- und fps-Tabellen wurde geändert
 > 8. dem Benutzer die Möglichkeit gegeben, die Auflösung zu bearbeiten (muss als 1024x768 eingegeben werden)

v 0.1.5
 > 1. ein Problem wurde behoben, bei dem das AI-Modell nicht automatisch geändert wurde, wenn FLOWFRAMES Interpolation AI ausgewählt wurde
 > 2. behebt ein Problem, bei dem die Interpolation von Flowframes nicht entsprechend der gewählten Option interpoliert wurde
 > 3. das Kombinationsfeld "FPS-Berechnungsmethode" wurde hinzugefügt, um eine falsche FPS-Berechnung für einige Videos zu verhindern.
        -> r_frame_rate / avg_frame_rate, Standard ist r_frame_rate
 > 4. Anzeige des Fortschritts beim Abrufen von Videoinformationen bei der Auswahl einer Videodatei
 > 5. Ändern Sie die Voreinstellung, dass der zuletzt ausgewählte Ordner geöffnet wird, wenn Sie eine Datei erneut auswählen, nachdem Sie sie geöffnet haben.

v 0.1.4
 > 1. Änderung der Art und Weise, wie die Datei config.ini gelesen wird
 > 2. die Art und Weise, wie Videoinformationen von Python AV zu ffmpeg übertragen werden, wurde geändert
 > 3. Fenster wird geschlossen, wenn die Aufgabe beendet ist
 > 4. zeige den vollen Dateinamen als Tooltip bei Mouseover in der Aufgabenliste
 > 5. zeige Auflösung(vorher) / Auflösung(nachher) / FPS(vorher) / FPS(nachher) für jede Datei in der Aufgabenliste
 > 6. FPS-Eingabefeld entfernen (wegen der obigen Beschriftung für jede Datei)
 > 7. die geschätzte Größe der Ausgabe-FPS entfernen (aufgrund der oben genannten dateispezifischen Beschriftung)
 > 8. den Fortschritt als zwei Fortschrittsbalken für alle Dateien/Aufgaben anzeigen

v 0.1.3
 > 1) Fehler bei der FPS-Berechnung von Dateien behoben, bei dem einige FPS-Informationen beim Laden von Dateien falsch waren

v 0.1.2
 > 1. Änderungen an der UI-Konfiguration
 > 2. interne Logikänderungen
 > 3. behebt das Problem, dass das Realesrgan-Modell nicht läuft, wenn zwei der folgenden Modelle ausgewählt werden
 > 4. geänderte Methode zur Verwendung von Realesrgan-Modellen
 > -> Kopieren Sie die neue Modelldatei (*.param) in den Ordner models im realesrgan-Installationsordner und Sie können sie verwenden.
 > 5. Anzeige der Breite, Höhe und geschätzten Größe der letzten Datei des Zielbildes, mit der gearbeitet werden soll
 > 6. den Code für die Migration der Datei config.ini schreiben
 > 7. Änderung des FFMPEG-Zerlegungsbildes AAC -> FLAC
 > 8. andere Fehlerbehebungen

v 0.1.1
 > 1. erstmaliges Schreiben eines Video-Upscaling-Programms mit ffmepg, realesrgan und flowframes