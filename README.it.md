[English](README.md) · [Русский](README.ru.md) · [中文](README.zh.md) · [हिन्दी](README.hi.md) · [Español](README.es.md) · [العربية](README.ar.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · **Italiano**

# Anton Sergeev
### Ingegnere ML/DL e C++/Python · IA industriale · Sistemi elettrici e automazione

**Unisco la conoscenza del settore industriale all'ingegneria del software e al machine learning.** Il mio percorso comprende diagnostica delle apparecchiature elettriche, automazione di processo e gestione di progetti tecnici. Oggi sviluppo modelli ML/DL, moduli di calcolo nativi e servizi dati per monitoraggio, previsione e supporto alle decisioni ingegneristiche.

Il mio punto di forza è comprendere il problema nella sua interezza: il significato di una misura, le modalità di guasto, il percorso dei dati verso il modello e il comportamento del software quando una connessione o un componente non funziona.

## Esperienza professionale

- **2001–2023 · Ruoli tecnici e di responsabilità:** diagnostica di apparecchiature elettriche da **0,4 a 750 kV**, comprese misure di scariche parziali e perdite dielettriche; direzione di lavori di automazione in grandi progetti industriali.
- **Progetti industriali:** automazione dello stabilimento di polipropilene SIBUR a Tobolsk e di un progetto di centrale da **120 MW** per Gazprom; lavori elettrici, di controllo e comunicazione in progetti tra cui Leningrad NPP-2 e il porto di Lavna.
- **Da settembre 2024 · Apollonian:** ingegneria ML e gestione di progetto; modelli LSTM e gradient boosting per telemetria di vibrazioni, pressione e temperatura; buffering dei dati, archivi S3 e integrazione REST/WebSocket.
- **Formazione:** laurea magistrale in Ingegneria dell'energia elettrica, Università Politecnica Pietro il Grande di San Pietroburgo, **2021**. Ulteriore formazione in ML/DL, computer vision, RAG, C++, Python e DevOps.

L'esperienza industriale orienta il mio lavoro software; i repository pubblici mostrano implementazioni e metodi di valutazione verificabili.

## Progetti selezionati

### [ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO) — machine learning per la diagnostica
Caratteristiche dei segnali in C++20 tramite pybind11, rilevamento classico delle anomalie, modelli PyTorch LSTM/GRU e inferenza ONNX. Sono documentati suddivisioni dei dati, baseline, provenienza e astensione: il sistema può rifiutare una stima non sufficientemente supportata.

**Da esaminare:** [contratto di affidabilità](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/main/docs/RELIABILITY.md) · [artefatti degli esperimenti](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/tree/main/experiments) · [CI](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/actions).

### [Ironpulse](https://github.com/Anton-Sergeev-EA/Ironpulse) — telemetria industriale resiliente in C++20
Acquisizione asincrona Modbus TCP, timeout e riconnessione, archiviazione WAL, rilevamento statistico delle anomalie e interfacce REST/WebSocket. Il progetto pone l'accento sul comportamento durante guasti di comunicazione e archiviazione.

**Da esaminare:** [test](https://github.com/Anton-Sergeev-EA/Ironpulse/tree/main/tests) · [build, sanitizer e integrazione CI](https://github.com/Anton-Sergeev-EA/Ironpulse/actions).

### [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore) — ricerca documentale locale e RAG
Indici vettoriali esatti/approssimati in C++ integrati con Python, embeddings, BM25 e API. Test degli indici e benchmark su carichi specifici rendono verificabili comportamento della ricerca e compromessi prestazionali.

**Da esaminare:** [implementazione nativa](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/native) · [benchmark](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/benchmarks) · [CI](https://github.com/Anton-Sergeev-EA/Cognivore/actions).

### Altri sistemi

- **[GridGuard](https://github.com/Anton-Sergeev-EA/GridGuard):** laboratorio IEC 61850 MMS/URCB, qualità della telemetria, WAL protetto da CRC e replay nel database.
- **[SCADA Generator](https://github.com/Anton-Sergeev-EA/SCADA_Generator):** HMI generata dalla configurazione, adattatori di protocolli industriali, ciclo degli allarmi e analisi C++/Python.
- **[Adaptive capacity allocator](https://github.com/Anton-Sergeev-EA/adaptive_capacity_allocator):** politiche di crescita dei contenitori C++17/20 con misure riproducibili di memoria e tempo.

## Strumenti tecnici

| Area | Tecnologie e metodi |
|---|---|
| Machine Learning e Deep Learning | PyTorch, scikit-learn, LightGBM/XGBoost, LSTM/GRU, anomalie, serie temporali, PCA, ONNX |
| Software e dati | C++17/20, Python, CMake, pybind11, FastAPI, REST/WebSocket, PostgreSQL, SQLite |
| Ricerca e distribuzione | RAG, embeddings, BM25, ricerca vettoriale, Linux, Docker, GitHub Actions, pytest, CTest, Ruff, sanitizer |

## Metodo di lavoro

Traduco requisiti operativi in contratti software verificabili, valuto i modelli rispetto a dati e baseline e misuro le prestazioni prima di formulare affermazioni. **Esperienza lavorativa industriale e validazione dei progetti pubblici sono distinte:** esperimenti ML sintetici e test di laboratorio dimostrano il loro ambito dichiarato, non accuratezza sul campo, deployment o certificazione. Ogni repository documenta i propri limiti.

## Lavoro e collaborazione

Interessato a **ingegneria ML/DL, sviluppo C++/Python e IA industriale**: diagnostica, previsioni, sistemi di ricerca, telemetria e servizi dati affidabili. Disponibile al trasferimento e al lavoro in team internazionali.

**Contatti:** [kavery@mail.ru](mailto:kavery@mail.ru) · [Apollonian](https://apollonian.ru/) · [tutti i repository](https://github.com/Anton-Sergeev-EA?tab=repositories).
