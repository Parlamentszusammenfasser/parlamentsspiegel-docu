# Parlamentsspiegel

Auf der Seite https://www.parlamentsspiegel.de veröffentlichen mehrere Landtage verschiedene Dokumente.

Es gibt eine Dokumentation, wie man auf der Seite suchen kann: https://www.parlamentsspiegel.de/suche?type=Tipp-Einstieg

So ist es möglich, den Stern `*` als Platzhalter für mehrere Zeichen oder das Fragezeichen ` ?` für ein einzelnes Zeichen zu verwenden.


## URL Query Parameter


### fqHerk

Der Parameter `fqHerk` gibt das Herkunfsbundesland an.


Mögliche Werte sind:

| Wert   | Land                   |
|--------|------------------------|
| `BAY`  | Bayern                 |
| `BLN`  | Berlin                 |
| `SAC`  | Sachsen                |
| `BW`   | Baden-Würtemberg       |
| `BRA`  | Brandenburg            |
| `NW`   | Nordrhein-Westfalen    |
| `NDS`  | Niedersachsen          |
| `SACA` | Sachsen-Anhalt         |
| `THUE` | Thüringen              |
| `RPF`  | Rheinland-Pfalz        |
| `HES`  | Hessen                 |
| `MEVO` | Mecklenburg-Vorpommern |
| `SH`   | Schleswig-Holstein     |
| `HB`   | Bremen                 |
| `HH`   | Hamburg                |
| `SAL`  | Saarland               |


### fqVSys

#### Beschaffen der Werte

Um alle Werte für den Parameter `fqVSys` zu erhalten, bietet es sich an, die Such-Seite des Parlamentsspiegels zu parsen.

Dazu lädt man sich zunächste die Seite im HTML-Format herunter:

```
curl -so ps-suche.html https://www.parlamentsspiegel.de/suche
```

(:warning: Letztes update: 15. 2. 2026)

Anschließend wird die Datei mit dem Skript ... geparst. :rotating_light: TODO: Skript verlinken


#### Liste der Werte

Mit dem Parameter `fqVSys` kann man ein Sachgebiet angeben.

Möglische Werte sind (ohne Gewähr der Vollständigkeit):

| Wert  | Bedeutung                     |
|-------|-------------------------------|
| 6110  | Natur                         |
| 6120  | Tier, Tierschutz, Tierhaltung |
| 6100  | Umwelt                        |
| 2130  | Erneuerbare Energien          |
| 6500  | Landwirtschaft                |
| 9999  | ohne Angaabe                  |
| 6700  | Jagd, Fischerei               |
| 6600  | Wald, Forsten                 |
| 6140  | Wasser                        |
| 2810  | Verkehrswegebau               |
| 4400  | Wissenschaft, Forschung       |
| 8300  | Öffentlischer Haushalt        |
| 1600  | Europäische Union             |
| 2820  | Städtebau                     |
| 6510  | Landwirtschaftliche Betriebe  |
| 2840  | Wasserbau                     |


### qyVTyp

Mit `qyVTyp` gibt man den Vorgangstyp an.


Mögliche Werte sind:

* `Anfrage`
* `Antrag`
* `Debatte`
* `Gesetz`
* `ohne@-VTyp`
* `Sonstiges`
* `Bericht`
* `Beschlussempfehlung`
* `Vorschrift`
* `Wahl`



