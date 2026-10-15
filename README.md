# Wordclock – Updates

Hier liegt die aktuelle Firmware für die Wordclock. Die iOS-App holt sie von hier
und spielt sie im WLAN auf die Uhr (Tab **Info** → „Software-Update“).

| Datei | Inhalt |
|---|---|
| `firmware.bin` | fertig übersetzte Firmware (aus der Arduino IDE exportiert) |
| `version.json` | Versionsnummer und kurzer Text, was neu ist |

## Neue Version veröffentlichen

1. In `Wordclock.ino` die Version erhöhen: `#define FW_VERSION "1.1.1"`
2. Arduino IDE → **Sketch → Kompilierte Binärdatei exportieren**
3. Die Datei `Wordclock.ino.bin` aus dem Ordner `build` in **`firmware.bin`** umbenennen und hier hochladen (ersetzt die alte)
4. `version.json` anpassen: gleiche Versionsnummer wie `FW_VERSION`

GitHub braucht danach bis zu 5 Minuten, bis die neue Datei überall ankommt.

Der Quellcode liegt in einem privaten Repository.

© Musikerli
