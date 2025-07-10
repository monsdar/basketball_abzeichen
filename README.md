# Basketball Abzeichen U10

Eine statische Website für das Basketball-Abzeichen-System für U10-Spieler.

## Features

- **Abzeichen-System** mit verschiedenen Stufen
- **Interaktive Kästchen** zum Abhaken der Aufgaben
- **Ausfüllbare Felder** für Namen, Datum und Trainer
- **Print-optimiert** für gedruckte Abzeichenblätter
- **Responsive Design** für alle Geräte

## Technologie

- **Hugo** - Statischer Site Generator
- **GitHub Pages** - Hosting
- **GitHub Actions** - Automatisches Deployment

## Lokale Entwicklung

```bash
# Hugo installieren (falls noch nicht geschehen)
# https://gohugo.io/installation/

# Repository klonen
git clone https://github.com/monsdar/Basketball_Abzeichen.git
cd Basketball_Abzeichen

# Hugo Server starten
hugo server

# Website unter http://localhost:1313 öffnen
```

## Deployment

Die Website wird automatisch bei jedem Push auf den `main` Branch deployed:

1. GitHub Actions baut die Hugo-Site
2. Deployed automatisch auf GitHub Pages
3. Verfügbar unter: https://monsdar.github.io/Basketball_Abzeichen/

## Neue Abzeichen hinzufügen

1. Neue Markdown-Datei in `content/abzeichen/` erstellen
2. Frontmatter hinzufügen:
   ```markdown
   ---
   title: "Abzeichen Name"
   date: 2024-07-10
   ---
   ```
3. Content hinzufügen
4. Push auf main Branch

## Struktur

```
content/
├── _index.md          # Startseite
├── impressum.md       # Impressum
└── abzeichen/
    └── wurfabzeichen.md  # Wurfabzeichen

themes/basketball-theme/
├── layouts/           # HTML Templates
└── static/css/       # CSS Dateien
```

## Lizenz

© 2024 Basketball Abzeichen U10 