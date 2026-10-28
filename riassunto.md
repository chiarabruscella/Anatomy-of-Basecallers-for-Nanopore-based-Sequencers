# Riassunto della tesi

## Introduzione
Le tecnologie NGS hanno trasformato genomica e trascrittomica, ma lo studio di epigenoma ed epitrascrittoma (modifiche chimiche che regolano l'espressione genica senza cambiare la sequenza) richiede approcci diretti. Il sequenziamento a nanopori di ONT (terza generazione) legge molecole native, non amplificate né frammentate.

## Capitolo 1: Epigenomica ed epitrascrittomica
- I metodi Short-Reads (50-300 bp) richiedono frammentazione e PCR; metodi come m6A-seq (immunoprecipitazione + NGS) danno informazioni indirette, senza risoluzione a singola base e singola molecola.
- Le Long-Reads (da ~10 kb a >1 Mb) permettono assemblaggi de novo, varianti strutturali, regioni ripetute e genomi T2T.
- Principio ONT: la molecola attraversa un nanoporo proteico, un enzima ne controlla la velocità, e ogni k-mer altera la corrente ionica ("squiggle"). Le modifiche lasciano una "firma" in ampiezza, intensità e tempo di permanenza (dwell time).
- Pori R10.4 (dual reader head) migliorano l'accuratezza rispetto a R9.4.1.

## Capitolo 2: Decodifica del dato grezzo
- Prima generazione: segmentazione in eventi + HMM (Nanocall), sensibile al rumore e agli omopolimeri.
- Poi reti neurali: DeepNano, BasecRAWller, Chiron (CNN + RNN/LSTM + decoder CTC), RODAN (CNN).
- Basecaller ONT: Guppy (RNN, modification-unaware), Bonito (CNN, addestrabile), Dorado (stato dell'arte, multi-modal, modification-aware).
- Esempi applicativi: ribonucleotidi incorporati nel DNA (Grasso et al., 2024) ed editing C-to-U dell'RNA da dRNA-Seq (Fonzino et al., 2023).

## Capitolo 3: Rilevamento delle modifiche
- Approccio 1: confronto del segnale con riferimento/controllo e resquiggling (Tombo, NanoCompore, EpiNano).
- Approccio 2: basecaller modification-aware addestrati su dati con e senza modifica (m6ABasecaller, Dorado, IL-AD).
- Sfide: dataset di training rappresentativi, cross-reattività tra modifiche adiacenti, falsi positivi.

## Conclusioni
ONT consente il rilevamento diretto delle modifiche a singola molecola; i basecaller modification-aware sono la frontiera attuale, ma accuratezza a singola read ed errori sistematici restano aree aperte.
