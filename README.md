# Anatomia dei Basecallers per Sequenziatori basati su Nanopori

Rassegna bioinformatica sul *basecalling* nel sequenziamento Oxford Nanopore (ONT) e sul rilevamento di modifiche epigenetiche ed epitrascrittomiche (m6A, m5C, Ψ, A-to-I).

Basata sulla mia tesi di laurea triennale in Biotecnologie Mediche e Farmaceutiche (Università di Bari "A. Moro", A.A. 2024-2025). Relatore: Prof. Adriano Fonzino.

## Di cosa parla

- **Epigenomica ed epitrascrittomica**: perché le modifiche chimiche di DNA e RNA contano e i limiti dei metodi Short-Reads (frammentazione, PCR, approcci indiretti come m6A-seq).
- **Sequenziamento a nanopori**: principio fisico, segnale di corrente ("squiggle"), k-mer, Long-Reads, pori R9.4.1 vs R10.4.1.
- **Evoluzione dei basecaller**: da HMM su eventi (Nanocall) a reti neurali (DeepNano, BasecRAWller, Chiron, RODAN), fino a Guppy, Bonito e Dorado.
- **Rilevamento delle modifiche**: confronto del segnale (Tombo, NanoCompore, EpiNano) vs basecaller *modification-aware* (m6ABasecaller, Dorado, IL-AD).

## Contenuti del repository

| File | Descrizione |
|---|---|
| [`docs/riassunto.md`](docs/riassunto.md) | Riassunto strutturato della tesi per capitolo |
| [`docs/evoluzione-basecaller.md`](docs/evoluzione-basecaller.md) | Tabella comparativa dei basecaller e delle architetture |
| [`docs/bibliografia.md`](docs/bibliografia.md) | Riferimenti principali con DOI |

## Competenze dimostrate

Sequenziamento di terza generazione · analisi del segnale nanopore · deep learning applicato alla genomica (CNN, RNN/LSTM) · epigenomica ed epitrascrittomica · lettura critica della letteratura scientifica · buona pratica di laboratorio · RT-qPCR e Western Blot (certificazioni Bio-Rad)

## Autrice

**Chiara Bruscella**: laureata in Biotecnologie Mediche e Farmaceutiche (UniBA), studentessa magistrale in Biotecnologie Mediche (UniMiB, LM-9).

- LinkedIn: _https://www.linkedin.com/in/chiara-bruscella22_
- Email: _chiara.bruscella@gmail.com_

## Licenza

Testi originali sotto [CC BY 4.0](LICENSE). Le figure della tesi appartengono agli autori citati e non sono incluse.
