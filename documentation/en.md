<!-- ELUCENIA technical documentation · escore-de-mayo-parcial · en · no clinical/professional/rights approval -->

# Partial Mayo score (ulcerative colitis)

[conditions, sources and permissions](https://elucenia.org/en/tools/escore-de-mayo-parcial)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Stool frequency

`freq`

- `0` — Normal for the patient
- `1` — 1 to 2 more than normal
- `2` — 3 to 4 more
- `3` — 5 or more additional

### Rectal bleeding

`sang`

- `0` — None
- `1` — Blood in fewer than half of bowel movements
- `2` — Blood in half or more
- `3` — Blood only (no stool)

### Physician global assessment

`global`

- `0` — Normal
- `1` — Mild disease
- `2` — Moderate
- `3` — Severe

## Method edition

Partial Mayo/Lewis 2008: 3 items 0–3, total 0–9, without endoscopic component

## Documented formula

Stool frequency (0 to 3) + rectal bleeding (0 to 3) + physician global assessment (0 to 3). Total 0 to 9.

Full Mayo (0 to 12) adds endoscopic appearance (0 to 3).

## Limits and population

Partial Mayo is a measure of activity and response in ulcerative colitis, with three components and no endoscopy; it is not equivalent to full Mayo and does not assess endoscopic healing. Lewis 2008 analyzed 105 patients with mild to moderate disease in a 12-week trial and compared change with patient-perceived improvement. That design does not establish universal performance in severe disease, children or other colitides. Record the symptom period and physician’s assessment; the total does not determine treatment alone.

## References

- [Schroeder KW, Tremaine WJ, Ilstrup DM. Coated oral 5-aminosalicylic acid therapy for mildly to moderately active ulcerative colitis: a randomized study. N Engl J Med, 1987.](https://doi.org/10.1056/NEJM198712243172603)

- [Lewis JD et al. Use of the noninvasive components of the Mayo score to assess clinical response in ulcerative colitis. Inflamm Bowel Dis, 2008.](https://doi.org/10.1002/ibd.20520)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Score ≤ 2: compatible with clinical remission

Cutoff of 2.5 with better sensitivity and specificity for patient-perceived remission (Lewis 2008).


### 2

Score ≥ 3: clinically active disease

A decrease of 3 points or more from baseline indicates clinical response (Lewis 2008).


### 3

Score ≥ 3: clinically active disease

A decrease of 3 points or more from baseline indicates clinical response (Lewis 2008).

