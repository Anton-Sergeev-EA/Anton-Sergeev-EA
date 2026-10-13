[English](README.md) · [Русский](README.ru.md) · [中文](README.zh.md) · [हिन्दी](README.hi.md) · [Español](README.es.md) · [العربية](README.ar.md) · [Français](README.fr.md) · [Português](README.pt.md) · **Deutsch** · [日本語](README.ja.md) · [Italiano](README.it.md) · [Ελληνικά](README.el.md) · [Čeština](README.cs.md)

# Anton Sergeev
### ML/DL- und C++/Python-Engineer · Industrielle KI · Energietechnik und Automatisierung

**Ich entwickle Systeme an der Schnittstelle von maschinellem Lernen, modernem C++ und industrieller Technik.** Meine Projekte verbinden ML/DL-Modelle, native Rechenmodule, Telemetrie und Suchsysteme—von der Bedeutung eines Signals bis zum Verhalten der verarbeitenden Software.

Mein Fokus liegt auf anspruchsvollen Aufgaben: verrauschten Daten, Fehlerbehebung, Nebenläufigkeit, Modellevaluation und messbaren Leistungskompromissen.

## Ausgewählte Projekte

### [ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO) — maschinelles Lernen für die Anlagendiagnose
Signalmerkmale aus C++20 über pybind11, klassische Anomalieerkennung, PyTorch-LSTM/GRU und ONNX-Inferenz. Dokumentiert sind Datenaufteilungen, Baselines, Datenherkunft und das Zurückhalten nicht ausreichend belegter Schätzungen.

**Einsehen:** [Zuverlässigkeitsvertrag](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/main/docs/RELIABILITY.md) · [Experimentartefakte](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/tree/main/experiments) · [CI](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/actions).

### [Ironpulse](https://github.com/Anton-Sergeev-EA/Ironpulse) — robuste industrielle Telemetrie in C++20
Asynchrone Modbus-TCP-Erfassung, Timeouts und Wiederverbindung, WAL-Speicherung, statistische Anomalieerkennung und REST/WebSocket-Schnittstellen. Im Mittelpunkt steht sinnvolles Systemverhalten bei Kommunikations- und Speicherfehlern.

**Einsehen:** [Tests](https://github.com/Anton-Sergeev-EA/Ironpulse/tree/main/tests) · [Build-, Sanitizer- und Integrations-CI](https://github.com/Anton-Sergeev-EA/Ironpulse/actions).

### [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore) — lokale Dokumentensuche und RAG
Native C++-Indizes für exakte/approximative Vektorsuche mit Python-Anbindung, Embeddings, BM25 und APIs. Indextests und Benchmarks für konkrete Lastprofile machen Suchverhalten und Leistungskompromisse nachvollziehbar.

**Einsehen:** [native Implementierung](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/native) · [Benchmarks](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/benchmarks) · [CI](https://github.com/Anton-Sergeev-EA/Cognivore/actions).

### Weitere Systemprojekte

- **[GridGuard](https://github.com/Anton-Sergeev-EA/GridGuard):** IEC-61850-MMS/URCB-Labor, Telemetriequalität, CRC-geschütztes WAL und Datenbank-Replay.
- **[SCADA Generator](https://github.com/Anton-Sergeev-EA/SCADA_Generator):** HMI aus Konfiguration, industrielle Protokolladapter, Alarmlebenszyklus und C++/Python-Analytik.
- **[Adaptive capacity allocator](https://github.com/Anton-Sergeev-EA/adaptive_capacity_allocator):** C++17/20-Container-Wachstumsstrategien mit reproduzierbaren Speicher-/Zeitmessungen.

## Technische Werkzeuge

| Bereich | Technologien und Methoden |
|---|---|
| Machine Learning und Deep Learning | PyTorch, scikit-learn, LightGBM/XGBoost, LSTM/GRU, Anomalien, Zeitreihen, PCA, ONNX |
| Software und Daten | C++17/20, Python, CMake, pybind11, FastAPI, REST/WebSocket, PostgreSQL, SQLite |
| Suche und Bereitstellung | RAG, Embeddings, BM25, Vektorsuche, Linux, Docker, GitHub Actions, pytest, CTest, Ruff, Sanitizer |

## Arbeitsweise

Ich übersetze betriebliche Anforderungen in testbare Softwareverträge, bewerte Modelle anhand von Daten und Baselines und messe Leistung vor Leistungsversprechen.  synthetische ML-Experimente und Protokolltests im Labor belegen ihren dokumentierten Umfang, keine Feldgenauigkeit, Inbetriebnahme oder Zertifizierung. Jedes Repository beschreibt seine Grenzen.

**Kontakt:** [avsergeev1981@gmail.com](mailto:avsergeev1981@gmail.com) · [Apollonian](https://apollonian.ru/) · [alle Repositories](https://github.com/Anton-Sergeev-EA?tab=repositories).
