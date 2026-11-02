# nachtschicht.studio

Statische Website von Nachtschicht Studio, gehostet über GitHub Pages.

| Datei | Seite |
| --- | --- |
| `index.html` | Startseite |
| `fernsy.html` | Fernsy – App-Seite |
| `homelab.html` | homelab.ad – Projektseite |
| `impressum.html` | Impressum & Datenschutz |

Gemeinsame Styles (inkl. Mobil-Layout) liegen in `assets/site.css`, das mobile Menü in `assets/site.js`.

## Veröffentlichen

Das Deployment übernimmt die GitHub Action `.github/workflows/pages.yml`: Jeder Push auf `main` veröffentlicht die Seite, manuell geht es über *Actions → Deploy to GitHub Pages → Run workflow*.

Einmalig einrichten:

1. Repository auf GitHub anlegen und den Inhalt dieses Ordners auf `main` pushen.
2. *Settings → Pages → Build and deployment*: Source „GitHub Actions“ wählen.
3. Optional eigene Domain: unter *Pages → Custom domain* eintragen, beim DNS-Anbieter die GitHub-Pages-Einträge setzen und zusätzlich eine `CNAME`-Datei mit der Domain ins Repo legen (die Action übernimmt sie mit).

## Lokal ansehen

```sh
python3 -m http.server 8000
```
