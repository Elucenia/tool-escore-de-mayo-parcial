<!-- ELUCENIA technical documentation · escore-de-mayo-parcial · it · no clinical/professional/rights approval -->

# Punteggio di Mayo parziale (rettocolite ulcerosa)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/escore-de-mayo-parcial)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Frequenza delle evacuazioni

`freq`

- `0` — Normale per il paziente
- `1` — Da 1 a 2 più del normale
- `2` — Da 3 a 4 in più
- `3` — 5 o più in aggiunta

### Sanguinamento rettale

`sang`

- `0` — Nessuno
- `1` — Sangue in meno della metà delle evacuazioni
- `2` — Sangue nella metà o più
- `3` — Solo sangue (senza feci)

### Valutazione medica globale

`global`

- `0` — Normale
- `1` — Malattia lieve
- `2` — Moderata
- `3` — Grave

## Edizione del metodo

Mayo parziale/Lewis 2008: 3 item 0–3, totale 0–9, senza componente endoscopico

## Formula documentata

Frequenza evacuazioni (0 a 3) + sanguinamento rettale (0 a 3) + valutazione medica globale (0 a 3). Totale 0 a 9.

Mayo completo (0 a 12) aggiunge aspetto endoscopico (0 a 3).

## Limiti e popolazione

Il Mayo parziale misura attività e risposta nella colite ulcerosa, con tre componenti e senza endoscopia; non equivale al Mayo completo né valuta la guarigione endoscopica. Lewis 2008 ha analizzato 105 pazienti con malattia lieve o moderata in uno studio di 12 settimane, confrontando il cambiamento con il miglioramento percepito dal paziente. Questo disegno non dimostra prestazioni universali nella malattia grave, nei bambini o in altre coliti. Registra il periodo dei sintomi e la valutazione medica; il totale da solo non determina il trattamento.

## Riferimenti

- [Schroeder KW, Tremaine WJ, Ilstrup DM. Coated oral 5-aminosalicylic acid therapy for mildly to moderately active ulcerative colitis: a randomized study. N Engl J Med, 1987.](https://doi.org/10.1056/NEJM198712243172603)

- [Lewis JD et al. Use of the noninvasive components of the Mayo score to assess clinical response in ulcerative colitis. Inflamm Bowel Dis, 2008.](https://doi.org/10.1002/ibd.20520)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
