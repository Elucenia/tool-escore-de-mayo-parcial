<!-- ELUCENIA technical documentation · escore-de-mayo-parcial · fr · no clinical/professional/rights approval -->

# Score de Mayo partiel (rectocolite hémorragique)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/escore-de-mayo-parcial)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Fréquence des selles

`freq`

- `0` — Normale pour le patient
- `1` — 1 à 2 de plus que la normale
- `2` — 3 à 4 de plus
- `3` — 5 ou plus supplémentaires

### Saignement rectal

`sang`

- `0` — Aucun
- `1` — Sang dans moins de la moitié des selles
- `2` — Sang dans la moitié ou plus
- `3` — Sang seul (sans selles)

### Évaluation médicale globale

`global`

- `0` — Normal
- `1` — Maladie légère
- `2` — Modérée
- `3` — Sévère

## Édition de la méthode

Mayo partiel/Lewis 2008 : 3 items 0–3, total 0–9, sans composante endoscopique

## Formule documentée

Fréquence selles (0 à 3) + saignement rectal (0 à 3) + évaluation globale médicale (0 à 3). Total 0 à 9.

Mayo complet (0 à 12) ajoute aspect endoscopique (0 à 3).

## Limites et population

Le Mayo partiel mesure l’activité et la réponse dans la rectocolite hémorragique, avec trois composantes et sans endoscopie ; il n’équivaut pas au Mayo complet et n’évalue pas la cicatrisation endoscopique. Lewis 2008 a analysé 105 patients ayant une maladie légère à modérée dans un essai de 12 semaines et comparé la variation à l’amélioration perçue par le patient. Ce plan ne démontre pas une performance universelle dans les formes sévères, chez les enfants ou dans d’autres colites. Consignez la période des symptômes et l’évaluation médicale ; le total ne détermine pas seul le traitement.

## Références

- [Schroeder KW, Tremaine WJ, Ilstrup DM. Coated oral 5-aminosalicylic acid therapy for mildly to moderately active ulcerative colitis: a randomized study. N Engl J Med, 1987.](https://doi.org/10.1056/NEJM198712243172603)

- [Lewis JD et al. Use of the noninvasive components of the Mayo score to assess clinical response in ulcerative colitis. Inflamm Bowel Dis, 2008.](https://doi.org/10.1002/ibd.20520)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Score ≤ 2 : compatible avec une rémission clinique

Seuil de 2,5 avec une meilleure sensibilité et spécificité pour la rémission perçue par le patient (Lewis 2008).


### 2

Score ≥ 3 : maladie cliniquement active

Une diminution de 3 points ou plus par rapport à la valeur initiale indique une réponse clinique (Lewis 2008).


### 3

Score ≥ 3 : maladie cliniquement active

Une diminution de 3 points ou plus par rapport à la valeur initiale indique une réponse clinique (Lewis 2008).

