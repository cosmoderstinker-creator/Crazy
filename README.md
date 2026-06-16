# Mit Vergnügen Berlin – App

Eine mobile-first **Progressive Web App (PWA)** im Stil des Berliner Stadtmagazins
[Mit Vergnügen](https://mitvergnuegen.com). Optimiert fürs Handy und installierbar
auf dem Home-Bildschirm.

## Features

- 📱 **Mobile-first** mit App-Feel: Bottom-Navigation, Sticky-Header, Story-Reihe, Karten-Feed
- 🎨 **Mit-Vergnügen-Look**: knallgelbe Navbar (`#ffe200`), schwarzer Handschrift-Schriftzug, weißer Inhalt, serifenlose Headlines
- 🔖 **Tabs**: Entdecken · Guides · Events · Karte · Favoriten
- ❤️ **Favoriten** (im Browser gespeichert via `localStorage`)
- 🔍 **Suche** & Kategorie-Filter (Essen & Trinken, Ausgehen, Kultur, Stadtleben, Shopping, Reisen)
- 📲 **Installierbar** (Web-App-Manifest + Service Worker, funktioniert offline)
- 🏙️ **Stadt-Wähler** (Berlin · Hamburg · München · Köln)

## Starten

Einfach `index.html` im Browser öffnen. Für die PWA-/Service-Worker-Funktionen
über einen lokalen Server starten:

```bash
python3 -m http.server 8000
# dann http://localhost:8000 öffnen
```

Auf dem Handy: Seite öffnen → Browser-Menü → **„Zum Home-Bildschirm hinzufügen"**.

## Dateien

| Datei | Zweck |
|-------|-------|
| `index.html` | Komplette App (HTML, CSS, JS – ohne Build-Schritt) |
| `manifest.webmanifest` | PWA-Manifest (Name, Icon, Theme) |
| `sw.js` | Service Worker (Offline-Cache) |
| `icon.svg` | App-Icon / Logo-Schriftzug |

## Hinweise zum Logo & zu den Inhalten

- Farben & Aufbau orientieren sich an einem **Screenshot der Original-Webseite**
  (gelbe Navbar, schwarzer Handschrift-Schriftzug, Kategorien FOOD · ERLEBNIS ·
  UNTERHALTUNG · AUSGEHEN · AUSFLUG).
- Der Schriftzug **„Mit Vergnügen"** ist als CSS/SVG-Rekonstruktion mit Handschrift-Font
  (Caveat) umgesetzt. Die **Original-Logo-Datei** kann einfach als `icon.svg` ersetzt
  bzw. im Header von `index.html` (Element `.logo`) eingebunden werden.
- Texte, Tipps und Bilder sind **Demonstrations-Inhalte** (Platzhalter, Bilder via Unsplash)
  und kein offizieller redaktioneller Content von Mit Vergnügen.
- „Mit Vergnügen" und das zugehörige Logo sind Eigentum der Mit Vergnügen GmbH.
  Diese App ist ein Stil-/Konzept-Prototyp.
