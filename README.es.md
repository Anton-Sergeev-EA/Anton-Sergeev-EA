[English](README.md) · [Русский](README.ru.md) · [中文](README.zh.md) · [हिन्दी](README.hi.md) · **Español** · [العربية](README.ar.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [Italiano](README.it.md)

# Anton Sergeev
### Ingeniero de ML/DL y C++/Python · IA industrial · Sistemas eléctricos y automatización

**Conecto el conocimiento industrial con la ingeniería de software y el aprendizaje automático.** Mi trayectoria abarca el diagnóstico de equipos eléctricos, la automatización de procesos y la dirección de proyectos técnicos. Actualmente desarrollo modelos ML/DL, módulos de cálculo nativos y servicios de datos para monitorización, predicción y apoyo a decisiones de ingeniería.

Mi fortaleza es comprender el problema completo: qué significa una medición, cómo falla un equipo, cómo llegan los datos al modelo y cómo se comporta el software cuando falla una conexión o un componente.

## Trayectoria profesional

- **2001–2023 · Ingeniería y dirección:** diagnóstico de equipos eléctricos de **0,4–750 kV**, incluidas mediciones de descargas parciales y pérdidas dieléctricas; dirección de trabajos de automatización en grandes proyectos industriales.
- **Proyectos industriales:** automatización de la planta de polipropileno de SIBUR en Tobolsk y de un proyecto de central de **120 MW** para Gazprom; trabajos eléctricos, de control y comunicaciones en proyectos como Leningrad NPP-2 y el puerto de Lavna.
- **Desde septiembre de 2024 · Apollonian:** ingeniería de ML y dirección de proyecto; modelos LSTM y gradient boosting para telemetría de vibración, presión y temperatura; almacenamiento temporal de datos, archivos S3 e integración REST/WebSocket.
- **Formación:** máster en Ingeniería Eléctrica, Universidad Politécnica Pedro el Grande de San Petersburgo, **2021**. Formación adicional en ML/DL, visión artificial, RAG, C++, Python y DevOps.

Esta experiencia industrial orienta mi trabajo de software; los repositorios públicos muestran implementaciones y métodos de evaluación que pueden revisarse.

## Proyectos destacados

### [ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO) — aprendizaje automático para diagnóstico de equipos
Características de señales en C++20 mediante pybind11, detección clásica de anomalías, modelos PyTorch LSTM/GRU e inferencia ONNX. Se documentan particiones de datos, baselines, procedencia y abstención: el sistema puede rechazar una estimación sin respaldo suficiente.

**Revisar:** [contrato de fiabilidad](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/main/docs/RELIABILITY.md) · [artefactos experimentales](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/tree/main/experiments) · [CI](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/actions).

### [Ironpulse](https://github.com/Anton-Sergeev-EA/Ironpulse) — telemetría industrial resiliente en C++20
Adquisición asíncrona Modbus TCP, tiempos de espera y reconexión, almacenamiento WAL, detección estadística de anomalías e interfaces REST/WebSocket. El objetivo es mantener un comportamiento útil ante fallos de comunicación o almacenamiento.

**Revisar:** [pruebas](https://github.com/Anton-Sergeev-EA/Ironpulse/tree/main/tests) · [compilación, sanitizers e integración CI](https://github.com/Anton-Sergeev-EA/Ironpulse/actions).

### [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore) — búsqueda documental local y RAG
Índices vectoriales exactos/aproximados en C++ integrados con Python, embeddings, BM25 y API. Las pruebas de índices y benchmarks con cargas específicas permiten revisar el comportamiento y los compromisos de rendimiento.

**Revisar:** [implementación nativa](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/native) · [benchmarks](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/benchmarks) · [CI](https://github.com/Anton-Sergeev-EA/Cognivore/actions).

### Otros sistemas

- **[GridGuard](https://github.com/Anton-Sergeev-EA/GridGuard):** laboratorio IEC 61850 MMS/URCB, calidad de telemetría, WAL protegido por CRC y reproducción en bases de datos.
- **[SCADA Generator](https://github.com/Anton-Sergeev-EA/SCADA_Generator):** HMI generado desde configuración, adaptadores industriales, ciclo de alarmas y analítica C++/Python.
- **[Adaptive capacity allocator](https://github.com/Anton-Sergeev-EA/adaptive_capacity_allocator):** políticas de crecimiento de contenedores C++17/20 con mediciones reproducibles de memoria y tiempo.

## Herramientas técnicas

| Área | Tecnologías y métodos |
|---|---|
| Machine Learning y Deep Learning | PyTorch, scikit-learn, LightGBM/XGBoost, LSTM/GRU, anomalías, series temporales, PCA, ONNX |
| Software y datos | C++17/20, Python, CMake, pybind11, FastAPI, REST/WebSocket, PostgreSQL, SQLite |
| Búsqueda y entrega | RAG, embeddings, BM25, búsqueda vectorial, Linux, Docker, GitHub Actions, pytest, CTest, Ruff, sanitizers |

## Forma de trabajar

Convierto requisitos operativos en contratos de software verificables, evalúo modelos respecto a datos y baselines y mido antes de afirmar mejoras de rendimiento. **La experiencia laboral industrial y la validación de proyectos públicos son distintas:** los experimentos sintéticos y las pruebas de laboratorio demuestran su alcance declarado, no precisión en campo, despliegue ni certificación. Cada repositorio documenta sus límites.

## Trabajo y colaboración

Interesado en **ingeniería ML/DL, desarrollo C++/Python e IA industrial**: diagnóstico, predicción, sistemas de búsqueda, telemetría y servicios de datos fiables. Disponible para reubicación y equipos internacionales.

**Contacto:** [kavery@mail.ru](mailto:kavery@mail.ru) · [Apollonian](https://apollonian.ru/) · [todos los repositorios](https://github.com/Anton-Sergeev-EA?tab=repositories).
