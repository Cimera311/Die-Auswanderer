# Die Auswanderer 🌴

Inoffizieller, werbefreier Episodenguide für **Goodbye Deutschland! Die Auswanderer**.

## GitHub Pages aktivieren

1. Repository → **Settings** → **Pages**
2. Bei **Build and deployment**: **Deploy from a branch**
3. Branch **main**, Folder **/(root)**, dann **Save**

Seite: https://cimera311.github.io/Die-Auswanderer/

## Inhalte

- `index.html`: mobilfreundliche Episodenübersicht mit Suche, Filtern und Gesehen-Markierungen
- `episodes.json`: Episodendaten, derzeit bewusst **leer**, bis Originaltermine und Titel geprüft sind

## Schema einer Episode

```json
{
  "id": "eindeutige-id",
  "title": "Folgentitel",
  "firstAirDate": "2026-01-01",
  "season": null,
  "episode": null,
  "status": "uncertain",
  "description": "Kurzbeschreibung",
  "people": [],
  "location": "",
  "sourceUrl": "https://example.org"
}
```

Die Datei `episodes.json` enthält ein Array solcher Objekte. `status`: `new` = bestätigte Erstausstrahlung, `repeat` = Wiederholung, `uncertain` = Herkunft unklar. Niemals Staffelnummern erfinden oder Uploads als Erstausstrahlung werten.

## Zwei Geräte

Die Website ist auf beiden iPhones nutzbar. **Gesehen-Markierungen bleiben zunächst je Browser lokal**; gemeinsame Synchronisierung benötigt später eine separate Datenbank. Das ChatGPT-Monitoring aktualisiert die GitHub-Dateien nicht selbstständig.

Nicht mit RTL/VOX verbunden.
