**English** · [Русский](README.ru.md) · [中文](README.zh.md) · [हिन्दी](README.hi.md) · [Español](README.es.md) · [العربية](README.ar.md) · [Français](README.fr.md) · [Português](README.pt.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [Italiano](README.it.md) · [Ελληνικά](README.el.md) · [Čeština](README.cs.md)

# Anton Sergeev
### ML/DL & C++/Python Engineer · Industrial AI · Power Systems & Automation

**I build systems at the intersection of machine learning, modern C++ and industrial engineering.** My work spans ML/DL models, native computing modules, telemetry pipelines and retrieval systems—from the meaning of a signal to the behaviour of the software that processes it.

I focus on the hard parts: noisy data, failure recovery, concurrency, model evaluation and measurable performance trade-offs.

## Selected engineering work

### [ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO) — machine learning for equipment diagnostics
C++20 signal features exposed through pybind11, classical anomaly detection, PyTorch LSTM/GRU models and ONNX inference. The reliability work documents data splits, baselines, provenance and abstention: the system can decline to provide an unsupported estimate.

**Inspect:** [reliability contract](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/main/docs/RELIABILITY.md) · [experiment artifacts](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/tree/main/experiments) · [CI](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/actions).

### [Ironpulse](https://github.com/Anton-Sergeev-EA/Ironpulse) — resilient industrial telemetry in C++20
Asynchronous Modbus TCP acquisition, timeouts and reconnection, WAL storage, statistical anomaly detection and REST/WebSocket interfaces. The focus is preserving useful behaviour under communication and storage failures.

**Inspect:** [tests](https://github.com/Anton-Sergeev-EA/Ironpulse/tree/main/tests) · [build, sanitizers and integration CI](https://github.com/Anton-Sergeev-EA/Ironpulse/actions).

### [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore) — local document retrieval and RAG
Native C++ exact/approximate vector indexes integrated with Python, embeddings, BM25 retrieval and APIs. Index tests and workload-specific benchmarks make retrieval behaviour and performance trade-offs inspectable.

**Inspect:** [native implementation](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/native) · [benchmarks](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/benchmarks) · [CI](https://github.com/Anton-Sergeev-EA/Cognivore/actions).

### Additional systems work

- **[GridGuard](https://github.com/Anton-Sergeev-EA/GridGuard):** IEC 61850 MMS/URCB laboratory, telemetry quality, CRC-protected WAL and database replay.
- **[SCADA Generator](https://github.com/Anton-Sergeev-EA/SCADA_Generator):** configuration-generated HMI, industrial protocol adapters, alarm lifecycle and C++/Python analytics.
- **[Adaptive capacity allocator](https://github.com/Anton-Sergeev-EA/adaptive_capacity_allocator):** C++17/20 container growth policies with reproducible memory/time trade-offs.

## Technical toolkit

| Area | Technologies and methods |
|---|---|
| Machine Learning & Deep Learning | PyTorch, scikit-learn, LightGBM/XGBoost, LSTM/GRU, anomaly detection, time series, PCA, ONNX |
| Software and data | C++17/20, Python, CMake, pybind11, FastAPI, REST/WebSocket, PostgreSQL, SQLite |
| Retrieval and delivery | RAG, embeddings, BM25, vector search, Linux, Docker, GitHub Actions, pytest, CTest, Ruff, sanitizers |

## How I work

I translate operational requirements into testable software contracts, keep model evaluation tied to data and baselines, and measure performance before making claims. Synthetic ML experiments and laboratory protocol tests demonstrate their stated scope, not field accuracy, deployment or certification. Each repository documents its own limits.

**Contact:** [avsergeev1981@gmail.com](mailto:avsergeev1981@gmail.com) · [Apollonian](https://apollonian.ru/) · [all repositories](https://github.com/Anton-Sergeev-EA?tab=repositories).
