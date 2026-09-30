# Kategorisierung des Ordners `icyleaf.com` (Branch `gh-pages`)

**Stand:** 2026-09-30 · **Dateien insgesamt:** 720 (ohne `.git`)

## Wichtiger Hinweis zur Natur des Ordners

Dieser Ordner enthält **keine Dokumentensammlung**, sondern den von Hugo
**generierten Build-Output** der Website icyleaf.com. Jede HTML-Datei
entspricht einer öffentlich erreichbaren URL (`2013/08/linux-101-chmod/index.html`
→ `https://icyleaf.com/2013/08/linux-101-chmod/`).

Daraus folgt:

1. **Dateien umsortieren = URLs zerstören.** Eine Umstrukturierung in
   Themenordner würde jeden Link, jedes Suchmaschinen-Ergebnis und jedes
   Lesezeichen brechen. Die Kategorisierung unten ist deshalb eine
   *Inventarisierung*, keine Verschiebung.
2. **Der Branch wird bei jedem Deploy neu erzeugt.** Änderungen hier werden
   vom nächsten Hugo-Build überschrieben. Dauerhafte Änderungen gehören in
   den Quell-Branch (Markdown-Quellen + Theme), nicht hierher.

---

## Kategorie 1 — Artikel (Inhalt) · 114 Dateien

Die eigentlichen Blogposts, abgelegt als `JAHR/MONAT/slug/index.html`.

| Jahr | Artikel | Jahr | Artikel |
|------|--------:|------|--------:|
| 2007 | 3  | 2016 | 5 |
| 2008 | 13 | 2017 | 4 |
| 2009 | 13 | 2018 | 5 |
| 2010 | 5  | 2019 | 4 |
| 2011 | 5  | 2021 | 1 |
| 2012 | 19 | 2022 | 8 |
| 2013 | 13 | 2023 | 7 |
| 2014 | 4  | 2024 | 1 |
| 2015 | 3  | 2025 | 1 |

**Inhaltliche Schwerpunkte** (aus 116 Tags, nach Artikelzahl):

- **Web-Entwicklung** — php (8), kohana (4), css (2), python (3), django, flask
- **Apple-Plattformen** — mac (7), ios (7), xcode (3), app (4)
- **DevOps & Infrastruktur** — git (4), shell (3), docker, gitlab, centos, linux (2), ci
- **Homelab & Hardware** — homelab-Serie, gen8, openwrt, nas, laptop, 4k
- **Reise & Persönliches** (chinesisch) — 游记/旅行 (Reiseberichte, 5), 年终总结 (Jahresrückblicke, 5), 美食, 养生
- **Android & Mobile** — android (3), 黑莓 (BlackBerry)

**Serien** (6): `homelab`, `cocoapods-collection`, `dockerdeployrails`,
`fastlane`, `hackintosh`, `brothers-legacy-lasers-are-modernizing`

## Kategorie 2 — Weiterleitungs-Stubs · 131 Dateien

Leere HTML-Dateien mit `<meta http-equiv=refresh>`, die alte URLs auf neue
umleiten (Hugo-Aliase). Enthalten keinen Inhalt, sind aber **funktional
notwendig** — sie halten historische Links am Leben.

## Kategorie 3 — Navigations- und Listenseiten · 258 Dateien

Automatisch erzeugte Übersichten ohne eigenen Inhalt:
`tags/` (116 Tag-Seiten), `series/`, `page/` (Paginierung), `posts/`,
`projects/`, `about/`, `aboutme/`, `gears/`, `tutorials/`, `draft/`

## Kategorie 4 — Feeds und Maschinen-Dateien · 130 Dateien

128 × `index.xml` (RSS je Sektion und Tag) · `sitemap.xml` · `robots.txt`

## Kategorie 5 — Bild-Assets · 79 Dateien (nach Bereinigung)

- `uploads/JAHR/…` — Artikelbilder nach Upload-Datum (52 nach Bereinigung)
- `gears/…`, `images/…` — Bilder für Hardware-Seiten und Seiten-Grafiken
- Root-Icons: Favicons, Apple-Touch-Icon, Android-Chrome-Icons, `safari-pinned-tab.svg`

## Kategorie 6 — Theme-Dateien (Design & Verhalten) · 12+ Dateien

`css/` (4) · `js/` (3) · `font/`, `font-ali/` (Icon-Fonts) ·
`photoswipe/` (Bild-Galerie-Bibliothek)

## Kategorie 7 — Konfiguration · 4 Dateien

`CNAME` (Custom Domain) · `.nojekyll` (deaktiviert GitHub-Jekyll) ·
`404.html` · `index.html` (Startseite)

---

## Duplikate

Geprüft wurde **bit-identischer Inhalt** (MD5 über alle 720 Dateien).
Ergebnis: 8 Gruppen.

### Verschoben nach `Duplikate/` — 7 Dateien

Bilder, die zweifach vorliegen und deren Kopie unter `uploads/2022/08/12/`
von **keiner** HTML-, XML- oder CSS-Datei referenziert wird. Die aktiv
genutzte Variante liegt unter `gears/xiaoxin-pad-pro-2021/` und bleibt
unangetastet.

| Verschoben (verwaist) | Aktiv genutzt bleibt |
|---|---|
| `uploads/2022/08/12/xiaoxin-pad-pro-2021.jpg` | `gears/xiaoxin-pad-pro-2021/xiaoxin-pad-pro-2021.jpg` |
| `uploads/2022/08/12/xiaoxin-video-encoder.jpg` | `gears/xiaoxin-pad-pro-2021/video-encoder.jpg` |
| `uploads/2022/08/12/xiaoxin-pad-filesystem-role.jpg` | `gears/xiaoxin-pad-pro-2021/filesystem-role.jpg` |
| `uploads/2022/08/12/xiaoxin-pads-compare.jpg` | `gears/xiaoxin-pad-pro-2021/version-compares.jpg` |
| `uploads/2022/08/12/tachiyomi-on-xiaoxin-pad-pro-2021.jpg` | `gears/xiaoxin-pad-pro-2021/tachiyomi.jpg` |
| `uploads/2022/08/12/xiaoxin-pad-copy-tf-photo.jpg` | `gears/xiaoxin-pad-pro-2021/copy-tf-photo.jpg` |
| `uploads/2022/08/12/xiaoxin-pad-dual-screens.jpg` | `gears/xiaoxin-pad-pro-2021/dual-screens.jpg` |

### Bewusst NICHT verschoben — 3 Dateien

Diese drei HTML-Dateien sind bit-identisch, aber es sind **aktive
Weiterleitungen** auf `/2022/02/how-to-homelab-part-0/`. Sie sind gleich,
weil sie dasselbe Ziel haben — nicht, weil eine überflüssig wäre. Ein
Verschieben würde drei funktionierende URLs zu 404 machen:

- `2022/02/homelab/index.html`
- `2022/02/how-to-homelab/index.html`
- `2022/02/how-to-homelab-part-0-intro/index.html`

---

## Zusätzlicher Befund: verwaiste Datei ohne Duplikat

`images/cover.jpg` wird von keiner Datei referenziert, hat aber auch keine
Zweitkopie. Da es kein Duplikat ist, wurde es **nicht** verschoben — es
gehört gelöscht oder eingebunden, das ist eine inhaltliche Entscheidung.
