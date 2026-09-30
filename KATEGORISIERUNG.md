# Kategorisierung des Repositories icyleaf.com (Branch `main`)

**Stand:** 2026-09-30 · **Dateien insgesamt:** 347 (ohne `.git`)

Dies ist der **Quell-Branch** der Website. Aus ihm erzeugt Hugo bei jedem Push
auf `main` den Branch `gh-pages` (siehe `.github/workflows/gh-pages.yml`).
Änderungen sind deshalb nur hier dauerhaft — alles, was direkt in `gh-pages`
liegt, wird vom nächsten Build überschrieben.

---

## Kategorie 1 — Inhalte · 119 Markdown-Dateien

### Artikel · `content/posts/` · 109 Dateien

Benennung: `JAHR-MONAT-TAG-slug.md`

| Jahr | Artikel | Jahr | Artikel |
|------|--------:|------|--------:|
| 2007 | 3  | 2016 | 5 |
| 2008 | 13 | 2017 | 4 |
| 2009 | 13 | 2018 | 6 |
| 2010 | 5  | 2019 | 4 |
| 2011 | 5  | 2021 | 1 |
| 2012 | 19 | 2022 | 5 |
| 2013 | 13 | 2023 | 4 |
| 2014 | 4  | 2024 | 1 |
| 2015 | 3  | 2025 | 1 |

**Inhaltliche Schwerpunkte** (116 Tags, nach Artikelzahl):

- **Web-Entwicklung** — PHP (8), Kohana (4), Python (3), CSS (2), Django, Flask
- **Apple-Plattformen** — macOS (7), iOS (7), Xcode (3), App-Entwicklung (4)
- **DevOps & Infrastruktur** — Git (4), Shell (3), Docker, GitLab, CentOS, Linux (2), CI
- **Homelab & Hardware** — Homelab-Serie, Gen8, OpenWrt, NAS, Notebooks, 4K
- **Android & Mobile** — Android (3), BlackBerry
- **Reise & Persönliches** (chinesisch) — 游记/旅行 Reiseberichte (5),
  年终总结 Jahresrückblicke (5), 美食, 养生

**Serien** (6): `homelab`, `cocoapods-collection`, `dockerdeployrails`,
`fastlane`, `hackintosh`, `brothers-legacy-lasers-are-modernizing`

### Hardware-Vorstellungen · `content/gears/` · 4 Dateien

`xiaoxin-pad-pro-2021`, `rg35xx`, `wujie-14x-8845`,
`itx-coffee-lake-hackintosh-build-for-4k-video-editing`

### Statische Seiten · `content/page/` · 3 Dateien

`about.md`, `apps.md`, `projects.md`

### Unveröffentlichte Entwürfe · `content/draft/` · 3 Dateien

`how-to-homelab-proxmox.md`, `create-talos-vm-with-cloud-init-in-proxmox.md`,
`photo-mechanic.md` — erscheinen nicht im Build, ihre Bilder liegen aber
bereits in `static/`.

## Kategorie 2 — Bild-Assets · `static/` · 114 Dateien (nach Bereinigung)

- `static/uploads/JAHR/MONAT/TAG/` — Artikelbilder nach Upload-Datum
- `static/tutorials/how-to-homelab/` — Bilder der Homelab-Serie, nach Teilen sortiert
- `static/gears/` — Bilder der Hardware-Vorstellungen, nach Gerät sortiert
- `static/images/`, `static/aboutme/` — Seiten-Grafiken, Spenden-QR-Codes, Icons

## Kategorie 3 — Website-Icons · `static/` · 7 Dateien

`favicon.ico`, `favicon-16x16.png`, `favicon-32x32.png`,
`apple-touch-icon.png`, `android-chrome-192x192.png`,
`android-chrome-512x512.png`, `safari-pinned-tab.svg`

## Kategorie 4 — Theme · `themes/nicesima/` · 94 Dateien

Layouts, Partials, SCSS/CSS, JavaScript, Icon-Fonts, PhotoSwipe-Galerie.
Wird per `.github/workflows/sync_theme.yml` synchronisiert.

## Kategorie 5 — Konfiguration · 8 Dateien

`config.yaml` (Hugo-Hauptkonfiguration) · `archetypes/` (Vorlagen für neue
Beiträge) · `i18n/` (Übersetzungen) · `static/CNAME` (Domain) ·
`.gitignore` · `.sops.yaml` (Secret-Verschlüsselung) · `README.md`

## Kategorie 6 — Automatisierung · `.github/workflows/` · 2 Dateien

- `gh-pages.yml` — baut bei Push auf `main` mit Hugo 0.135.0 und
  veröffentlicht `./public` nach `gh-pages`
- `sync_theme.yml` — hält das Theme aktuell

---

## Duplikate

Geprüft wurde **bit-identischer Inhalt** (MD5 über alle 347 Dateien).
Ergebnis: 7 Gruppen, alle identisch aufgebaut.

### Verschoben nach `Duplikate/` — 7 Dateien

Bilder, die zweifach vorliegen. Die Kopien unter `static/uploads/2022/08/12/`
werden von **keiner** Datei referenziert — geprüft über `content/` (inklusive
der unveröffentlichten Entwürfe), `themes/`, `i18n/` und `config.yaml`. Die
tatsächlich eingebundenen Varianten liegen unter
`static/gears/xiaoxin-pad-pro-2021/` und bleiben unangetastet.

| Verschoben (verwaist) | Aktiv genutzt bleibt |
|---|---|
| `uploads/2022/08/12/xiaoxin-pad-pro-2021.jpg` | `gears/xiaoxin-pad-pro-2021/xiaoxin-pad-pro-2021.jpg` |
| `uploads/2022/08/12/xiaoxin-video-encoder.jpg` | `gears/xiaoxin-pad-pro-2021/video-encoder.jpg` |
| `uploads/2022/08/12/xiaoxin-pad-filesystem-role.jpg` | `gears/xiaoxin-pad-pro-2021/filesystem-role.jpg` |
| `uploads/2022/08/12/xiaoxin-pads-compare.jpg` | `gears/xiaoxin-pad-pro-2021/version-compares.jpg` |
| `uploads/2022/08/12/tachiyomi-on-xiaoxin-pad-pro-2021.jpg` | `gears/xiaoxin-pad-pro-2021/tachiyomi.jpg` |
| `uploads/2022/08/12/xiaoxin-pad-copy-tf-photo.jpg` | `gears/xiaoxin-pad-pro-2021/copy-tf-photo.jpg` |
| `uploads/2022/08/12/xiaoxin-pad-dual-screens.jpg` | `gears/xiaoxin-pad-pro-2021/dual-screens.jpg` |

`Duplikate/` liegt im Repository-Wurzelverzeichnis und **nicht** in `static/`.
Hugo kopiert nur `static/` in den Build — der Ordner landet also bewusst nicht
auf der Website, bleibt aber im Repository erhalten.

### Hinweis zum Branch `gh-pages`

Im generierten Output existiert eine achte Duplikat-Gruppe: drei identische
HTML-Dateien unter `2022/02/`. Sie entstehen aus den `aliases` im Frontmatter
von `content/posts/2022-02-12-how-to-homelab-part-0.md` und sind aktive
Weiterleitungen auf `/2022/02/how-to-homelab-part-0/`. Sie sind gleich, weil
sie dasselbe Ziel haben — nicht, weil eine überflüssig wäre, und dürfen nicht
entfernt werden.

---

## Zusätzlicher Befund: verwaiste Dateien ohne Duplikat

Diese Dateien werden von keinem Inhalt referenziert, sind aber **keine**
Duplikate und wurden deshalb **nicht** verschoben:

- `static/images/cover.jpg` — ohne erkennbare Verwendung
- `static/tutorials/how-to-homelab/proxmox/*` (8 Dateien) und
  `static/tutorials/how-to-homelab/storages/nas-server.jpeg` — gehören
  vermutlich zum unveröffentlichten Entwurf `content/draft/how-to-homelab-proxmox.md`
  und werden gebraucht, sobald dieser erscheint
- `static/tutorials/how-to-homelab/part-0/network-virtual-devices.png`

Ob diese gelöscht oder eingebunden werden, ist eine inhaltliche Entscheidung.

Die Website-Icons (Kategorie 3) erscheinen in keiner Inhaltsdatei, weil das
Theme sie über feste Pfade einbindet. Sie sind in Benutzung.
