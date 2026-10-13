# Anton Sergeev

### Industrial AI · Machine Learning & Deep Learning · Power Systems · C++ / Python

I am a power systems and industrial automation engineer with more than 20 years of experience in energy and industrial infrastructure. I now develop C++/Python software and ML/DL models for industrial telemetry, condition monitoring and engineering analytics.

**Interested in:** Machine Learning / Deep Learning Engineering, Industrial AI, Industrial Software and SCADA/OT Software roles, and collaboration on diagnostics, time-series modelling and telemetry.

## Machine Learning & Deep Learning

- **Classical ML and signal analysis:** anomaly detection, Isolation Forest, PCA/MSPC and condition monitoring.
- **Deep Learning:** PyTorch, LSTM/GRU sequence models, time-series forecasting and remaining-useful-life research in [ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO); synthetic CNN/LSTM experiments in [Smart_Guard_AI](https://github.com/Anton-Sergeev-EA/Smart_Guard_AI).
- **ML engineering:** documented data splits and baselines, experiment artifacts, native C++/Python integration and ONNX inference.
- **Retrieval systems:** local RAG workflows, vector search and evidence mapping in [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore).

Model results are tied to the datasets and evaluation conditions documented in each repository. Synthetic experiments demonstrate laboratory behaviour; they do not establish field accuracy.

## Start here

- **[GridGuard](https://github.com/Anton-Sergeev-EA/GridGuard):** IEC 61850 MMS/URCB laboratory, telemetry quality and durable replay. [Measurement boundaries](https://github.com/Anton-Sergeev-EA/GridGuard/blob/main/docs/BENCHMARKS.md) · [CI](https://github.com/Anton-Sergeev-EA/GridGuard/actions).
- **[Ironpulse](https://github.com/Anton-Sergeev-EA/Ironpulse):** C++20 Modbus TCP acquisition, reconnects, WAL storage and monitoring APIs. [Tests](https://github.com/Anton-Sergeev-EA/Ironpulse/tree/main/tests) · [CI](https://github.com/Anton-Sergeev-EA/Ironpulse/actions).
- **[ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO):** C++/Python signal processing, classical ML and PyTorch LSTM/GRU models for anomaly detection and synthetic RUL experiments. [Reliability contract](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/main/docs/RELIABILITY.md) · [Experiments](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/tree/main/experiments) · [CI](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/actions).

## More engineering work

- [SCADA Generator](https://github.com/Anton-Sergeev-EA/SCADA_Generator): configuration-driven HMI, protocol adapters, alarm lifecycle and C++/Python analytics.
- [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore): local retrieval workflows, a native C++ vector index, evidence mapping and workload-specific benchmarks.
- [Adaptive capacity allocator](https://github.com/Anton-Sergeev-EA/adaptive_capacity_allocator): C++17/20 container growth policies with measured memory/time trade-offs.

Supporting repositories cover service reliability, forecasting, computer vision, graphics and concurrency. Their READMEs identify status and evaluation limits.

## Validation and engineering approach

My industrial employment experience and the validation of these public software projects are separate. Laboratory protocol tests, synthetic telemetry and synthetic RUL experiments do not establish field accuracy, industrial deployment or independent IEC certification.

GridGuard covers a documented MMS/URCB laboratory profile and read-only adapters. Buffered-report recovery, GOOSE/SV, certification and field deployment are outside its demonstrated scope. ML results should be read with their dataset, split, baseline and experiment revision.

I focus on explicit failure modes, useful tests, reproducible measurements and documented trade-offs. Review each project's source, tests, limitations and CI at the revision relevant to your use case.

## Technical focus

C++17/20 · Python · CMake · pybind11 · asynchronous I/O · industrial protocols · PyTorch / scikit-learn · ONNX · FastAPI · PostgreSQL / SQLite · Linux · Docker · CI and sanitizers

## Work and collaboration

Open to international engineering teams and relocation. For project discussions, use the relevant repository's issue tracker. Please keep sensitive operational data out of public issues.

