# Morse Light Webapp

Installationsfreie Webapp für iPhone-Morse über Licht: senden per Bildschirm und optional per LED, empfangen per Kamera und live dekodieren.

## Überblick

Diese Webapp ist für zwei iPhones gedacht:

- **Sender-iPhone**: sendet Morsecode als Lichtpulse
- **Empfänger-iPhone**: erkennt die Lichtpulse mit der Kamera und dekodiert sie zu Text

Die App läuft direkt im Browser und muss nicht installiert werden.

https://tbr-brd.github.io/morse-light-webapp/

## Funktionen

- Texteingabe und automatische Umwandlung in Morse
- Senden per **Bildschirmblitz**
- Optionaler Versuch, die **iPhone-LED** im Browser zu schalten
- Empfang per Kamera auf einem zweiten iPhone
- Live-Anzeige von Morsecode und dekodiertem Text
- **Auto-Kalibrierung** des Helligkeits-Schwellwerts

## Wichtiger Hinweis zu iPhones

Die Taschenlampen-/LED-Steuerung im mobilen Browser ist auf iPhones nicht auf jedem Gerät und nicht in jeder Safari-Version zuverlässig verfügbar. Deshalb ist der **Bildschirmblitz** als robuster Fallback eingebaut.

## Dateien im Repository

- `index.html` – die komplette Webapp in einer einzelnen Datei
- `README.md` – diese Anleitung
- `LICENSE` – MIT-Lizenz
- `repo-description.txt` – kurze Beschreibung für GitHub

## GitHub Pages Schritt für Schritt

### 1. Repository erstellen

1. Auf GitHub anmelden
2. Auf **New repository** klicken
3. Als Namen zum Beispiel `morse-light-webapp` vergeben
4. Repository auf **Public** setzen
5. Repository erstellen

### 2. Dateien hochladen

1. Im neuen Repository auf **Add file** → **Upload files**
2. Diese Dateien hochladen:
   - `index.html`
   - `README.md`
   - `LICENSE`
   - `repo-description.txt`
3. Commit speichern

### 3. GitHub Pages aktivieren

1. Im Repository auf **Settings**
2. In der linken Navigation auf **Pages**
3. Unter **Build and deployment**
   - **Source**: `Deploy from a branch`
   - **Branch**: `main`
   - **Folder**: `/(root)`
4. Speichern

Nach kurzer Zeit ist die Seite unter einer URL wie dieser erreichbar:

`https://DEIN-NAME.github.io/morse-light-webapp/`

## Nutzung mit zwei iPhones

### Sender-iPhone

1. Seite öffnen
2. Text eingeben
3. Optional **LED vorbereiten** drücken
4. **Senden starten**

### Empfänger-iPhone

1. Seite öffnen
2. **Empfang starten**
3. Kamera auf den Sender richten
4. **Auto-Kalibrierung** drücken
5. Morsecode empfangen

## Empfohlene Testeinstellungen

- Erst mit kurzen Wörtern testen, zum Beispiel `SOS` oder `HALLO`
- Tempo auf **180–300 ms pro Punkt**
- Eher dunkle Umgebung
- Konstanter Abstand zwischen Sender und Empfänger

## Fehlerbehebung

### Kamera funktioniert nicht
- Prüfen, ob die Seite über **HTTPS** geöffnet wurde
- Kamera-Berechtigung in Safari erlauben
- Seite neu laden

### LED funktioniert nicht
- Das ist auf iPhones im Browser nicht immer unterstützt
- In diesem Fall den **Bildschirmblitz** verwenden

### Dekodierung ist unzuverlässig
- Tempo langsamer stellen
- Dunklere Umgebung wählen
- Kamera besser auf den Sender ausrichten
- Auto-Kalibrierung erneut ausführen
- Schwellwert manuell nachjustieren

## Alternative zu GitHub Pages

Die Datei kann auch direkt bei **Vercel** gehostet werden. Da alles in einer einzelnen HTML-Datei steckt, ist kein Build-Prozess nötig.

## GitHub-Kurzbeschreibung

Der Inhalt aus `repo-description.txt` kann in GitHub als Repository-Beschreibung verwendet werden.
