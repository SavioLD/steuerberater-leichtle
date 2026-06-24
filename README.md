# Steuerkanzlei Christoph Leichtle – Karriere-Landingpage

Bewerbungs-Landingpage für Meta-Kampagnen.
Ausgeschriebene Stelle: **Finanzbuchhaltung & Lohnabrechnung in Teilzeit** (Rottweil).

Erstellt von **Ländle Digital**.

## Inhalt

| Datei / Ordner | Beschreibung |
|---|---|
| `index.html` | Die Landingpage (lädt `css/` + `assets/`, Schriften via Google Fonts CDN) |
| `css/style.css`, `css/landing.css` | Design – CI-Crimson, **Oswald** (Überschriften/Logo) + **Open Sans** (Fließtext) |
| `assets/og.png` | Social-Preview-Bild (Link-Vorschau) |
| `assets/creatives/` | 3 Anzeigen-Creatives für Meta (4:5, 1080×1350 px, PNG) |
| `landingpage-einzeldatei.html` | Komplette Seite als **eine** Datei (CSS **und** Schriften eingebettet) – ideal zum schnellen Teilen oder Hochladen, funktioniert auch offline |

## Vorschau / lokal öffnen

- **Schnell:** `landingpage-einzeldatei.html` doppelklicken.
- **„Richtig" (mit css/ + assets/):** im Ordner einen kleinen Webserver starten:
  ```bash
  python3 -m http.server
  # dann http://localhost:8000 öffnen
  ```

## Deployment

Reine statische Seite – **kein Build nötig**. Den Ordnerinhalt einfach auf einen
Webspace bzw. Static-Host laden (Netlify, Vercel, Cloudflare Pages, klassisches
Hosting). Einstiegsdatei ist `index.html`.

## Bewerbungsformular

Der Versand läuft über **Web3Forms** (Access-Key + Logik am Ende von `index.html`).
Die Empfänger-Adresse ist im Web3Forms-Dashboard hinterlegt; für eine eigene
Empfänger-Adresse dort einen eigenen Key anlegen und eintragen.

## Vor dem Livegang bestätigen

- **Impressum-/Datenschutz-Links** im Footer (zeigen aktuell auf
  `steuerberater-leichtle.de/impressum` bzw. `/datenschutz`).
- **Stundenumfang / Gehalt / Eintrittstermin** je nach finalem Stellenprofil.

## Als eigenes GitHub-Repo pushen

Dieses Verzeichnis ist bereits ein Git-Repo mit erstem Commit. Neues, leeres
Repo auf GitHub anlegen und dann:

```bash
git remote add origin git@github.com:<DEIN-USER>/<REPO-NAME>.git
git branch -M main
git push -u origin main
```
