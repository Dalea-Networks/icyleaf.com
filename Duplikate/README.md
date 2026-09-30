# Duplikate

Ausgelagerte Dateien, die im Repository nicht mehr gebraucht werden. Der
Ordner liegt im Wurzelverzeichnis und **nicht** in `static/`: Hugo kopiert nur
`static/` in den Build, der Inhalt hier erscheint also nicht auf der Website,
bleibt aber im Repository erhalten.

Die Ordnerstruktur unterhalb entspricht der ursprünglichen, damit jede Datei
bei Bedarf zurückgelegt werden kann:

    Duplikate/static/…  →  static/…

Der Ordner enthält zwei verschiedene Arten von Dateien.

## 1. Echte Duplikate — 7 Dateien

`static/uploads/2022/08/12/` (7 Bilder)

Bit-identisch (gleiche MD5-Summe) zu einer zweiten Datei im Repository und an
dieser Stelle von keinem Inhalt referenziert. Die aktiv eingebundenen
Varianten liegen unter `static/gears/xiaoxin-pad-pro-2021/` und sind
unangetastet. Vollständige Gegenüberstellung in `../KATEGORISIERUNG.md`.

## 2. Verwaiste Dateien ohne Zweitkopie — 2 Dateien

`static/images/cover.jpg` · `static/tutorials/how-to-homelab/part-0/network-virtual-devices.png`

Diese beiden sind **keine** Duplikate — es gibt keine zweite Kopie von ihnen.
Sie werden lediglich von keiner Datei mehr referenziert und wurden auf
ausdrücklichen Wunsch mit hierher ausgelagert. Da keine Zweitkopie existiert,
sind sie **nur noch hier** vorhanden: wer sie wieder braucht, muss sie von
hier zurückholen.

Geprüft wurde jeweils `content/` einschließlich der unveröffentlichten
Entwürfe, `themes/`, `i18n/` und `config.yaml`. Für `cover.jpg` zusätzlich
alle `image:`- und `cover:`-Angaben im Frontmatter: die verwendeten Cover
verweisen auf `/aboutme/`, `/uploads/` und `/gears/`, nie auf `/images/`.

## Nicht hier ausgelagert

Die acht Bilder unter `static/tutorials/how-to-homelab/proxmox/` und
`storages/nas-server.jpeg` sind ebenfalls unreferenziert, gehören aber zum
unveröffentlichten Entwurf `content/draft/how-to-homelab-proxmox.md` und
werden gebraucht, sobald dieser erscheint.
