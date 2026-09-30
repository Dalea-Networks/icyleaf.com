# Duplikate

Hier liegen Dateien, die bit-identisch (gleiche MD5-Summe) an einer zweiten
Stelle im Repository vorhanden sind und an **dieser** Stelle von keinem Inhalt
referenziert werden.

Die Ordnerstruktur unterhalb entspricht der ursprünglichen, damit jede Datei
bei Bedarf zurückgelegt werden kann:

    Duplikate/static/uploads/2022/08/12/…  →  static/uploads/2022/08/12/…

Dieser Ordner liegt bewusst im Wurzelverzeichnis und **nicht** in `static/`:
Hugo kopiert nur `static/` in den Build, der Ordner erscheint also nicht auf
der Website, bleibt aber im Repository erhalten.

Vollständige Gegenüberstellung samt aktiv genutzter Variante:
siehe `../KATEGORISIERUNG.md`, Abschnitt „Duplikate".
