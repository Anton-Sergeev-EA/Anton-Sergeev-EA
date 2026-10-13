[English](README.md) · [Русский](README.ru.md) · [中文](README.zh.md) · [हिन्दी](README.hi.md) · [Español](README.es.md) · [العربية](README.ar.md) · **Français** · [Português](README.pt.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [Italiano](README.it.md) · [Ελληνικά](README.el.md) · [Čeština](README.cs.md)

# Anton Sergeev
### Ingénieur ML/DL et C++/Python · IA industrielle · Énergie et automatisation

**Je développe des systèmes à la croisée du machine learning, du C++ moderne et de l’ingénierie industrielle.** Mes projets associent modèles ML/DL, calcul natif, télémétrie et recherche documentaire, du sens d’un signal au comportement du logiciel qui le traite.

Je me concentre sur les difficultés techniques : données bruitées, reprise après incident, concurrence, évaluation des modèles et compromis de performance mesurables.

## Projets d’ingénierie

### [ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO) — machine learning pour le diagnostic des équipements
Caractéristiques de signaux en C++20 via pybind11, détection classique d’anomalies, modèles PyTorch LSTM/GRU et inférence ONNX. Les partitions de données, baselines, provenance et mécanismes d’abstention sont documentés : le système peut refuser une estimation insuffisamment étayée.

**À examiner:** [contrat de fiabilité](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/main/docs/RELIABILITY.md) · [artefacts expérimentaux](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/tree/main/experiments) · [CI](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/actions).

### [Ironpulse](https://github.com/Anton-Sergeev-EA/Ironpulse) — télémétrie industrielle robuste en C++20
Acquisition asynchrone Modbus TCP, délais d’attente et reconnexion, stockage WAL, détection statistique d’anomalies et interfaces REST/WebSocket. Le projet met l’accent sur le comportement en cas de panne des communications ou du stockage.

**À examiner:** [tests](https://github.com/Anton-Sergeev-EA/Ironpulse/tree/main/tests) · [compilation, sanitizers et intégration](https://github.com/Anton-Sergeev-EA/Ironpulse/actions).

### [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore) — recherche documentaire locale et RAG
Index vectoriels exacts/approximatifs en C++ intégrés à Python, embeddings, BM25 et API. Les tests d’index et benchmarks sur des charges précises rendent vérifiables le comportement de la recherche et les compromis de performance.

**À examiner:** [implémentation native](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/native) · [benchmarks](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/benchmarks) · [CI](https://github.com/Anton-Sergeev-EA/Cognivore/actions).

### Autres systèmes

- **[GridGuard](https://github.com/Anton-Sergeev-EA/GridGuard):** Laboratoire IEC 61850 MMS/URCB, qualité de télémétrie, WAL protégé par CRC et rejeu en base de données.
- **[SCADA_Generator](https://github.com/Anton-Sergeev-EA/SCADA_Generator):** HMI générée par configuration, adaptateurs de protocoles industriels, cycle de vie des alarmes et analyse C++/Python.
- **[adaptive_capacity_allocator](https://github.com/Anton-Sergeev-EA/adaptive_capacity_allocator):** Politiques de croissance de conteneurs C++17/20 avec mesures reproductibles de mémoire et de temps.

## Outils techniques

| Domaine | Technologies et méthodes |
|---|---|
| Machine Learning et Deep Learning | PyTorch, scikit-learn, LightGBM/XGBoost, LSTM/GRU, anomalies, séries temporelles, PCA, ONNX |
| Logiciels et données | C++17/20, Python, CMake, pybind11, FastAPI, REST/WebSocket, PostgreSQL, SQLite |
| Recherche et livraison | RAG, embeddings, BM25, recherche vectorielle, Linux, Docker, GitHub Actions, pytest, CTest, Ruff, sanitizers |

## Approche d’ingénierie

Je transforme les exigences opérationnelles en contrats logiciels testables, évalue les modèles par rapport aux données et aux baselines, et mesure avant d’annoncer un gain de performance. Les expériences ML synthétiques et les tests de protocoles en laboratoire démontrent leur périmètre documenté, pas la précision sur le terrain, un déploiement ou une certification. Chaque dépôt décrit ses limites.

**Contact:** [avsergeev1981@gmail.com](mailto:avsergeev1981@gmail.com) · [Apollonian](https://apollonian.ru/) · [tous les dépôts](https://github.com/Anton-Sergeev-EA/?tab=repositories).
