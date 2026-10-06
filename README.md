# Anton Sergeev

## Industrial AI · Power Systems · SCADA / OT · Predictive Maintenance

Power and automation engineer with 20+ years around mission-critical energy and industrial infrastructure, now building the software and AI layer on top of operational technology.

My strongest engineering intersection is **power systems + industrial automation + C++/Python + applied ML**: telemetry acquisition, SCADA/OT integration, anomaly detection, predictive maintenance, edge-oriented analytics, APIs and production engineering.

> This portfolio focuses on industrial systems where domain engineering, reliability, software architecture, and applied AI come together.

### What I build

- **Industrial telemetry & OT software:** Modbus, SCADA-oriented acquisition, protocol adapters, alarms, time-series pipelines and edge services.
- **Industrial AI:** anomaly detection, condition monitoring, predictive-maintenance prototypes, signal processing and RUL research.
- **Systems software:** modern C++, asynchronous I/O, concurrency, native Python extensions, testing and performance measurement.
- **ML/backend:** Python, PyTorch/scikit-learn, FastAPI, PostgreSQL, ONNX and reproducible model artifacts.
- **Delivery:** Linux, Docker, CI/CD, sanitizers, observability and documented engineering trade-offs.

## Flagship engineering portfolio

| Project | Engineering signal | What to inspect |
|---|---|---|
| [GridGuard](https://github.com/Anton-Sergeev-EA/GridGuard) | **Digital-substation laboratory / C++20 + Python** | Real libIEC61850 MMS reports, explicit synthetic/quality provenance, synced CRC WAL, SQLite/PostgreSQL replay, read-only OT adapters and fault-recovery tests; inspect implementation, test contracts and documented limits |
| [Ironpulse](https://github.com/Anton-Sergeev-EA/Ironpulse) | **C++20 industrial telemetry / edge monitoring** | Asio Modbus TCP, strands/timeouts/recovery, WAL/export, EWMA/CUSUM, REST/WebSocket/Prometheus, sanitizers + Docker smoke CI |
| [ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO) | **Predictive health / power-electronics ML** | C++20 signal core + pybind11, Isolation Forest/LSTM/GRU, ONNX, evidence/provenance, abstention and synthetic-RUL reliability contract |
| [SCADA Generator](https://github.com/Anton-Sergeev-EA/SCADA_Generator) | **SCADA / OT digitalization** | Config-generated HMI, Modbus/OPC UA/MQTT/IEC-104 adapters, alarm lifecycle, C++ streaming analytics, PCA/MSPC and pre-alarms |
| [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore) | **Systems AI / local RAG** | Hand-written C++ vector search, SIMD/OpenMP-oriented CPU path, retrieval architecture, evidence mapping and local-first orchestration |
| [Adaptive capacity allocator](https://github.com/Anton-Sergeev-EA/adaptive_capacity_allocator) | **Focused C++ systems algorithms** | Inspectable allocation policies, native test contracts and a small reproducible build |

### How the projects fit together

```text
Field equipment / PLCs / power assets
              │
              ▼
   OT acquisition & SCADA layer
   SCADA Generator · Ironpulse
              │
              ▼
 telemetry / events / history
              │
              ▼
 condition monitoring & diagnostics
          ARGUS-NEURO
              │
              ▼
 engineering knowledge / AI assistance
            Cognivore
```

This is the portfolio story: **acquire industrial data reliably → detect abnormal behaviour → support maintenance and engineering decisions**.

## Evidence and validation boundaries

The industrial projects include simulation-based validation. Synthetic telemetry,
synthetic RUL experiments and loopback protocol tests do not establish field
accuracy, independent IEC conformance or a production deployment. Review source,
limitations, test contracts and CI at a specific revision before relying on a claim.

GridGuard currently has a tested laboratory scope: real IEC 61850 MMS/URCB,
read-only protocol adapters, deterministic fault scenarios and durable replay.
Its supported profile and limitations are documented. No buffered-report recovery, GOOSE/SV,
IEC certification, field deployment or calibrated predictive performance is claimed.

## Supporting projects

The remaining repositories demonstrate breadth rather than define my primary positioning: backend/service reliability, computer vision, forecasting/data products, simulation/graphics and experimental AI applications. I keep them public, but hiring reviewers for Industrial AI / Grid Automation / Digitalization roles should start with the six projects above.

## Engineering principles

I prefer explicit failure modes over optimistic demos, reproducible measurements over unsupported performance claims, and documented limitations over “production-ready” labels that the evidence cannot support. Several portfolio projects intentionally distinguish synthetic/test validation from field validation.

## Target work

Industrial AI · Grid/Power Digitalization · SCADA/OT Software · Condition Monitoring · Predictive Maintenance · Edge Analytics · Industrial Data Platforms

Open to international engineering teams and relocation.
