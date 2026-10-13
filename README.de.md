[English](README.md) · [Русский](README.ru.md) · [中文](README.zh.md) · [हिन्दी](README.hi.md) · [Español](README.es.md) · [العربية](README.ar.md) · **Deutsch** · [日本語](README.ja.md) · [Italiano](README.it.md)

# Anton Sergeev
### ML/DL- und C++/Python-Engineer · Industrielle KI · Energietechnik und Automatisierung

**Ich verbinde industrielles Fachwissen mit Softwareentwicklung und maschinellem Lernen.** Mein beruflicher Hintergrund umfasst die Diagnose elektrischer Betriebsmittel, Prozessautomatisierung und technische Projektleitung. Heute entwickle ich ML/DL-Modelle, native Rechenmodule und Datendienste für Überwachung, Prognosen und technische Entscheidungsunterstützung.

Meine Stärke ist der Blick auf die gesamte Aufgabe: die Bedeutung eines Messwerts, Ausfallmechanismen der Anlage, den Datenweg zum Modell und das Verhalten der Software beim Ausfall einer Verbindung oder Komponente.

## Beruflicher Hintergrund

- **2001–2023 · Ingenieur- und Führungsaufgaben:** Diagnose elektrischer Betriebsmittel im Bereich **0,4–750 kV**, einschließlich Teilentladungs- und Verlustfaktormessungen; Leitung von Automatisierungsarbeiten in großen Industrieprojekten.
- **Industrieprojekte:** Prozessautomatisierung für das Polypropylenwerk von SIBUR in Tobolsk und ein **120-MW-Kraftwerksprojekt** für Gazprom; Elektro-, Steuerungs- und Kommunikationsarbeiten in Projekten wie Leningrad NPP-2 und dem Hafen Lavna.
- **Seit September 2024 · Apollonian:** ML-Engineering und Projektleitung; LSTM- und Gradient-Boosting-Modelle für Schwingungs-, Druck- und Temperaturdaten; Datenpufferung, S3-Archive und REST/WebSocket-Integration.
- **Ausbildung:** Master in elektrischer Energietechnik, Peter-der-Große-Polytechnische Universität Sankt Petersburg, **2021**. Weiterbildungen in ML/DL, Computer Vision, RAG, C++, Python und DevOps.

Diese Industrieerfahrung prägt meine Softwarearbeit. Die öffentlichen Repositories zeigen nachvollziehbare Implementierungen und Evaluationsverfahren.

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

Ich übersetze betriebliche Anforderungen in testbare Softwareverträge, bewerte Modelle anhand von Daten und Baselines und messe Leistung vor Leistungsversprechen. **Industrieberufserfahrung und die Validierung öffentlicher Projekte sind getrennt:** synthetische ML-Experimente und Protokolltests im Labor belegen ihren dokumentierten Umfang, keine Feldgenauigkeit, Inbetriebnahme oder Zertifizierung. Jedes Repository beschreibt seine Grenzen.

## Arbeit und Zusammenarbeit

Interesse an **ML/DL-Engineering, C++/Python-Entwicklung und industrieller KI**: Diagnose, Prognosen, Suchsysteme, Telemetrie und zuverlässige Datendienste. Offen für einen Umzug und internationale Teams.

**Kontakt:** [kavery@mail.ru](mailto:kavery@mail.ru) · [Apollonian](https://apollonian.ru/) · [alle Repositories](https://github.com/Anton-Sergeev-EA?tab=repositories).
