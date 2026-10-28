# Evoluzione dei basecaller per nanopori

| Basecaller | Architettura | Note |
|---|---|---|
| Nanocall | HMM su eventi | Prima generazione, sensibile a rumore e omopolimeri |
| DeepNano | RNN | Primo basecaller a reti ricorrenti |
| BasecRAWller | 2 RNN (segmentazione + k-mer) | Lavora sul segnale grezzo |
| Chiron | CNN + RNN/LSTM + decoder CTC | End-to-end |
| RODAN | CNN | Per RNA diretto |
| Guppy (ONT, 2017) | RNN | Standard per anni, modification-unaware |
| Bonito (ONT) | CNN | Facilmente addestrabile su dati specifici |
| Dorado (ONT) | Deep learning, multi-modal | Stato dell'arte, rileva m6A, m5C, Ψ durante il basecalling |

## Rilevamento di modifiche

| Strumento | Approccio |
|---|---|
| Tombo | Confronto del segnale con riferimento (resquiggling) |
| NanoCompore | Confronto WT vs knock-out/controllo |
| EpiNano | Differenze "error-like" tra campioni |
| m6ABasecaller | Basecaller modification-aware per m6A |
| IL-AD | Apprendimento incrementale + anomaly detection |
