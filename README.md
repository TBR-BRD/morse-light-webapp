# Morse Light Webapp

Installationsfreie Webapp für iPhone-Morse über Licht: senden per Bildschirm und optional per LED, empfangen per Kamera und live dekodieren.

![ohne Hand](01-ohne-Hand.png)

![mit Hand](02-mit-Hand.png)

Mit diesem Setup kann gezeigt werden, was die Unterbrechung des Lichtstrahls in einer Glasfaser für Auswirkungen auf die Datenübertragung hat.

**Project Summary: Morse Light Webapp for iPhone**

This project is a browser-based web application that demonstrates how Morse code can be transmitted and received using light between two iPhones, without installing a native app.

One iPhone acts as the **sender**. It converts user-entered text into Morse code and transmits it as light pulses, using the screen as a reliable fallback and, where supported, the rear LED flash.

The second iPhone acts as the **receiver**. It uses the rear camera to detect incoming light pulses, analyzes brightness changes in real time, and decodes them back into text inside the web app.

The project includes several usability and reliability improvements:

* text-to-Morse conversion
* adjustable transmission speed
* optional rear/front camera selection
* automatic receiver calibration
* simplified receiver interface
* centered detection window for more robust signal capture
* an auto-start receiver mode with one main start button
* GitHub Pages deployment support

The goal of the project is to create an easy-to-understand, installation-free demonstration of **optical communication**, showing how information can be transmitted with light in a simple and visual way.

A second visual concept was also created to illustrate how light transmission could be guided through **fiber optics**, and how the signal can be interrupted if an object blocks the optical path.

<br>
<a href="https://www.buymeacoffee.com/thoralf.brandt" target="_blank">
  <img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174">
</a>
<br>

## Überblick

Diese Webapp ist für zwei iPhones gedacht:

- **Sender-iPhone**: sendet Morsecode als Lichtpulse
- **Empfänger-iPhone**: erkennt die Lichtpulse mit der Kamera und dekodiert sie zu Text

![Aufbau der Morse-Webapp](setup-aufbau.png)

Die App läuft direkt im Browser und muss nicht installiert werden. Nachfolgenden Link auf beiden iPhones öffnen oder QR Code scannen.

https://tbr-brd.github.io/morse-light-webapp/

![QR-Code](morse-light-webapp-qr.png)

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

## Nutzung mit zwei iPhones

## Version mit Auto-Start

- großer Startknopf für den Empfänger
- Kamera startet automatisch
- automatische Kalibrierung direkt nach dem Start
- Messfenster in der Bildmitte
- Fokus auf dekodierten Text

## Testablauf

1. Empfänger: **Empfang automatisch starten**
2. Warten bis **Bereit zum Empfangen**
3. Sender: Nachricht senden
4. Licht im grünen Messfenster halten

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
