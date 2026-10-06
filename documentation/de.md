<!-- ELUCENIA technical documentation · escore-de-mayo-parcial · de · no clinical/professional/rights approval -->

# Partieller Mayo-Score (Colitis ulcerosa)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/escore-de-mayo-parcial)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Stuhlfrequenz

`freq`

- `0` — Für den Patienten normal
- `1` — 1 bis 2 mehr als normal
- `2` — 3 bis 4 mehr
- `3` — 5 oder mehr zusätzlich

### Rektale Blutung

`sang`

- `0` — Keiner
- `1` — Blut bei weniger als der Hälfte der Stuhlgänge
- `2` — Blut bei der Hälfte oder mehr
- `3` — Nur Blut (kein Stuhl)

### Globale ärztliche Beurteilung

`global`

- `0` — Normal
- `1` — Leichte Erkrankung
- `2` — Mäßig
- `3` — Schwer

## Fassung der Methode

Partieller Mayo/Lewis 2008: 3 Items 0–3, Gesamt 0–9, ohne Endoskopie

## Dokumentierte Formel

Stuhlfrequenz (0 bis 3) + rektale Blutung (0 bis 3) + globale ärztliche Einschätzung (0 bis 3). Gesamt 0 bis 9.

Vollständiger Mayo (0 bis 12) ergänzt Endoskopie (0 bis 3).

## Grenzen und Population

Der partielle Mayo misst Aktivität und Ansprechen bei Colitis ulcerosa mit drei Komponenten ohne Endoskopie; er entspricht nicht dem vollständigen Mayo und beurteilt keine endoskopische Heilung. Lewis 2008 analysierte 105 Patienten mit leichter bis mittelschwerer Erkrankung in einer 12-wöchigen Studie und verglich die Veränderung mit der vom Patienten empfundenen Besserung. Dieses Design belegt keine universelle Leistung bei schwerer Erkrankung, Kindern oder anderen Kolitiden. Dokumentieren Sie den Symptomzeitraum und die ärztliche Beurteilung; die Gesamtsumme allein legt die Behandlung nicht fest.

## Referenzen

- [Schroeder KW, Tremaine WJ, Ilstrup DM. Coated oral 5-aminosalicylic acid therapy for mildly to moderately active ulcerative colitis: a randomized study. N Engl J Med, 1987.](https://doi.org/10.1056/NEJM198712243172603)

- [Lewis JD et al. Use of the noninvasive components of the Mayo score to assess clinical response in ulcerative colitis. Inflamm Bowel Dis, 2008.](https://doi.org/10.1002/ibd.20520)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Punktzahl ≤ 2: vereinbar mit klinischer Remission

Cutoff von 2,5 mit besserer Sensitivität und Spezifität für die vom Patienten wahrgenommene Remission (Lewis 2008).


### 2

Punktzahl ≥ 3: klinisch aktive Erkrankung

Ein Rückgang um 3 Punkte oder mehr gegenüber dem Ausgangswert weist auf ein klinisches Ansprechen hin (Lewis 2008).


### 3

Punktzahl ≥ 3: klinisch aktive Erkrankung

Ein Rückgang um 3 Punkte oder mehr gegenüber dem Ausgangswert weist auf ein klinisches Ansprechen hin (Lewis 2008).

