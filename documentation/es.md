<!-- ELUCENIA technical documentation · escore-de-mayo-parcial · es · no clinical/professional/rights approval -->

# Puntuación parcial de Mayo (colitis ulcerosa)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/escore-de-mayo-parcial)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Frecuencia de deposiciones

`freq`

- `0` — Normal para el paciente
- `1` — De 1 a 2 más de lo normal
- `2` — De 3 a 4 más
- `3` — 5 o más adicionales

### Sangrado rectal

`sang`

- `0` — Ninguno
- `1` — Sangre en menos de la mitad de las deposiciones
- `2` — Sangre en la mitad o más
- `3` — Solo sangre (sin heces)

### Evaluación médica global

`global`

- `0` — Normal
- `1` — Enfermedad leve
- `2` — Moderada
- `3` — Grave

## Edición del método

Mayo parcial/Lewis 2008: 3 ítems 0–3, total 0–9, sin componente endoscópico

## Fórmula documentada

Frecuencia deposiciones (0 a 3) + sangrado rectal (0 a 3) + evaluación médica global (0 a 3). Total 0 a 9.

Mayo completo (0 a 12) añade aspecto endoscópico (0 a 3).

## Límites y población

El Mayo parcial mide actividad y respuesta en colitis ulcerosa, con tres componentes y sin endoscopia; no equivale al Mayo completo ni evalúa cicatrización endoscópica. Lewis 2008 analizó 105 pacientes con enfermedad leve a moderada en un ensayo de 12 semanas y comparó el cambio con la mejoría percibida por el paciente. Ese diseño no demuestra desempeño universal en enfermedad grave, niños u otras colitis. Registre el período de síntomas y la evaluación médica; el total no determina por sí solo el tratamiento.

## Referencias

- [Schroeder KW, Tremaine WJ, Ilstrup DM. Coated oral 5-aminosalicylic acid therapy for mildly to moderately active ulcerative colitis: a randomized study. N Engl J Med, 1987.](https://doi.org/10.1056/NEJM198712243172603)

- [Lewis JD et al. Use of the noninvasive components of the Mayo score to assess clinical response in ulcerative colitis. Inflamm Bowel Dis, 2008.](https://doi.org/10.1002/ibd.20520)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
