# esp-anker-releases

Fertige, digital signierte Firmware-Dateien (nur Binaerdateien, kein Quellcode) fuer den Anker-Controller auf ESP32.
Die Geraete holen `manifest.json` von hier und installieren Updates nur, wenn die Signatur stimmt (ECDSA P-256, Schluessel im Geraet).

- `manifest.json`: Version, Dateiname, Groesse, SHA-256, Signatur und Aenderungsprotokoll je Geraetetyp (esp32s3, esp32c3)
- `anker-<typ>-<version>.bin`: die Firmware

Dieses Repository wird automatisch aus dem privaten Projekt befuellt (`tools/release.py`). Nicht von Hand aendern: Eine veraenderte Datei wird vom Geraet abgelehnt.
Keine Zugangsdaten, Tokens oder Einstellungen sind in den Dateien enthalten; sie liegen nur im jeweiligen Geraet.

Nutzung auf eigene Verantwortung, ohne Gewaehr.
