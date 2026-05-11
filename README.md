# Zapf's Biohof — Website

Statische GitHub Pages Website für den Biohof Zapf, Berghaupten.
Live: https://zapf-bio.github.io/website/ (Custom Domain folgt: zapf-bio.de)

## Verzeichnisstruktur

```
/
├── index.html              ← Landing Page
├── impressum.html
├── datenschutz.html
├── images/
│   ├── Kraeuterseitling.png
│   ├── Austernseitling.png
│   ├── Shiitake.png
│   └── Zitronenseitling.png
└── fonts/                  ← noch anzulegen (siehe unten)
    ├── cormorant-garamond-300.woff2
    ├── cormorant-garamond-400.woff2
    ├── cormorant-garamond-400-italic.woff2
    ├── cormorant-garamond-500.woff2
    ├── cormorant-garamond-600.woff2
    ├── inter-300.woff2
    ├── inter-400.woff2
    └── inter-500.woff2
```

## Schriftarten (lokal, noch ausstehend)

`impressum.html` und `datenschutz.html` laden Schriften lokal aus `/fonts/`. Einmalig herunterladen via [google-webfonts-helper](https://gwfh.mranftl.com/fonts):

1. **Cormorant Garamond** — Gewichte 300, 400, 400 italic, 500, 600 (Format: Modern Browsers / woff2)
2. **Inter** — Gewichte 300, 400, 500

Dateien wie oben angegeben benennen und in `/fonts/` ablegen.

> `index.html` lädt Schriften aktuell noch über Google Fonts. Vor dem Live-Gang auf lokale Fonts umstellen.

## Platzhalter ersetzen

In `impressum.html` und `datenschutz.html` sind offene Stellen mit `[PLATZHALTER: ...]` markiert (visuell hervorgehoben). Noch ausstehend von Max Zapf:

- Vor- und Nachname des Inhabers
- Echte Telefonnummer
- USt-IdNr. oder Steuernummer
- Vollständige Bio-Kontrollstellen-Bezeichnung (z.B. "ABCERT AG, Esslingen")
- Vollständige DE-ÖKO-Nummer
- Datum

## Custom Domain einrichten (wenn bereit)

Max Zapf setzt im Registrar folgende DNS-A-Records:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

Dann unter **Settings → Pages → Custom domain**: `zapf-bio.de` eintragen und "Enforce HTTPS" aktivieren. Max braucht keinen GitHub-Account — nur Zugang zu seinem Registrar.

## Pre-Launch-Checkliste

- [ ] Alle `[PLATZHALTER: ...]` ersetzt
- [ ] Schriftdateien in `/fonts/` liegen
- [ ] `index.html` auf lokale Fonts umgestellt
- [ ] Footer-Links zu Impressum und Datenschutz funktionieren
- [ ] Auf Mobilgeräten getestet
- [ ] Custom Domain eingerichtet und HTTPS aktiv
