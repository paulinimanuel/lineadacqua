# Linea d’Acqua — build PWA con 11 schermate

Questa versione ricostruisce l’interfaccia a partire dalla tavola di riferimento fornita: ingresso, Home, Il mio acquario, Valori dell’acqua, Guida, Piante, dettaglio pianta, Diario, Analisi, Aggiungi evento e Consigli.

## Prova in locale
1. Estrai tutto lo ZIP in una cartella nuova.
2. Per verificare l’interfaccia, apri `index.html` nel browser.
3. Per provare installazione PWA e modalità offline, pubblica i file su HTTPS oppure avvia un server locale. Il service worker non funziona pienamente aprendo il file direttamente.

## Funzioni incluse
- Configurazione generica dell’acquario, volume, tipo, fase e attrezzatura (nessun acquario precompilato).
- Inserimento dei test con valore, data/ora e note; gli stessi test alimentano diario, valori e grafici.
- Storico filtrabile e cancellazione delle voci, con aggiornamento delle analisi.
- Grafico con intervalli di 7 giorni, 30 giorni, 3 mesi e 1 anno, statistiche min/max/media e range ideali indicativi.
- Diario per test, cambio acqua, fertilizzazione, manutenzione, piante/fauna, prodotti, foto e note. Foto fino a 900 KB per voce.
- Catalogo botanico iniziale con ricerca, filtri, schede dettagliate e lista personale delle piante.
- Guida passo passo e consigli contestuali basati sui dati registrati.
- Esportazione JSON e dati locali del browser.

## Note importanti
- Non sono inseriti risultati di test dimostrativi: i valori appaiono dopo che li registri.
- Gli intervalli sono orientativi, non una diagnosi e non sono adatti automaticamente a tutte le specie.
- I dati restano nel browser/dispositivo e non si sincronizzano automaticamente tra dispositivi. Esporta regolarmente una copia.
- Questa è una build di test. Il design segue la foto come riferimento, ma la corrispondenza pixel per pixel e il collaudo su tutti i dispositivi richiedono verifica visiva e test reali prima di pubblicare online.


## Revisione grafica 16 ottobre 2026
La barra di navigazione segue il riferimento approvato: Home, Analisi, Diario, Piante, Guida. Il pulsante + flottante compare nel Diario per creare una nuova voce. Palette e dimensioni sono state rifinite per avvicinare l'interfaccia al collage approvato. Build preliminare: verificare tutte le funzioni prima della pubblicazione.


## Revisione visuale v4 — 16 ottobre 2026
- Home: aggiunta la checklist interattiva “Attività di oggi” con stato 0/3 e salvataggio locale delle spunte.
- Guida: aggiunta la card introduttiva “Guida passo passo” e disposizione delle categorie in due colonne su schermi abbastanza larghi, con layout adattivo su telefoni stretti.
- Rifinitura di spaziature, tonalità blu e card per avvicinarsi ulteriormente alla tavola approvata.
- Il riferimento grafico originale è incluso in `riferimenti/riferimento_design_approvato.png`.
- Build di prova: non sostituisce la versione online; verificare interazioni e resa sul proprio telefono prima della pubblicazione.


## Rifinitura Home e Guida
- Accessi rapidi Home riallineati al riferimento: Nuovo test, Nuova attività, Aggiungi foto.
- Le tre azioni aprono il modulo corretto e selezionano il tipo di evento pertinente.
- Aggiunta la scheda larga "Problemi comuni" sotto le Categorie principali nella Guida, prima delle Guide rapide; apre la guida su alghe, acqua torbida e valori fuori range.


## Catalogo piante ampliato
Il catalogo locale è stato ampliato con ulteriori specie d’acqua dolce, incluse piante a stelo, tappezzanti, epifite, muschi e galleggianti. Le schede sono orientative: verificare sempre la specie/cultivar e le condizioni dell’acquario. Non è un catalogo esaustivo di tutte le specie esistenti e non è collegato automaticamente a un catalogo online. Alcune specie galleggianti o a crescita rapida possono essere soggette a restrizioni locali: non rilasciarle mai in natura.


### Immagini del catalogo piante
Le schede aggiunte includono miniature botaniche illustrative incorporate nella PWA e disponibili anche offline. Sono immagini generate per orientare visivamente tra forme di crescita e gruppi di piante; non sostituiscono una fotografia botanica verificata della singola cultivar/specie. Prima dell'acquisto, confronta il nome scientifico con una fonte specialistica.


FOTO DELLE 59 SPECIE: Le schede cercano online una fotografia per il nome botanico esatto su Wikipedia e Wikimedia Commons. La foto e disponibile solo con Internet e solo quando una corrispondenza e presente; altrimenti rimane l’immagine illustrativa locale. La ricerca non garantisce identificazione botanica verificata ne la disponibilita per tutte le 59 specie. Nessuna foto online e incorporata nell’archivio.
