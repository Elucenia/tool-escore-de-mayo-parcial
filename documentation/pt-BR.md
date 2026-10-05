<!-- ELUCENIA technical documentation · escore-de-mayo-parcial · pt-BR · no clinical/professional/rights approval -->

# Escore de Mayo parcial (retocolite)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/escore-de-mayo-parcial)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Frequência evacuatória

`freq`

- `0` — Normal para o paciente
- `1` — 1 a 2 a mais que o normal
- `2` — 3 a 4 a mais
- `3` — 5 ou mais a mais

### Sangramento retal

`sang`

- `0` — Nenhum
- `1` — Sangue em menos da metade das evacuações
- `2` — Sangue em metade ou mais
- `3` — Só sangue (sem fezes)

### Avaliação médica global

`global`

- `0` — Normal
- `1` — Doença leve
- `2` — Moderada
- `3` — Grave

## Edição do método

Partial Mayo/Lewis 2008:3 itens 0–3, total 0–9, sem componenteendoscópico

## Fórmula documentada

Frequência evacuatória (0 a 3) + sangramento retal (0 a 3) + avaliação médica global (0 a 3). Total de 0 a 9.

O escore de Mayo completo (0 a 12) soma o aspecto endoscópico (0 a 3).

## Limites e população

O Mayo parcial é uma medida de atividade e resposta na retocolite ulcerativa, com três componentes e sem endoscopia; não equivale ao Mayo completo nem avalia cicatrização endoscópica. A análise de Lewis 2008 envolveu 105 pacientes com doença leve a moderada em um ensaio de 12 semanas e comparou a mudança com a melhora percebida pelo paciente. Esse desenho não demonstra desempenho universal em doença grave, crianças ou outras colites. Registre o período dos sintomas e a avaliação médica; o total não determina tratamento sozinho.

## Referências

- [Schroeder KW, Tremaine WJ, Ilstrup DM. Coated oral 5-aminosalicylic acid therapy for mildly to moderately active ulcerative colitis: a randomized study. N Engl J Med, 1987.](https://doi.org/10.1056/NEJM198712243172603)

- [Lewis JD et al. Use of the noninvasive components of the Mayo score to assess clinical response in ulcerative colitis. Inflamm Bowel Dis, 2008.](https://doi.org/10.1002/ibd.20520)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
