[English](README.md) · [Русский](README.ru.md) · [中文](README.zh.md) · [हिन्दी](README.hi.md) · [Español](README.es.md) · [العربية](README.ar.md) · [Français](README.fr.md) · **Português** · [Deutsch](README.de.md) · [日本語](README.ja.md) · [Italiano](README.it.md) · [Ελληνικά](README.el.md) · [Čeština](README.cs.md)

# Anton Sergeev
### Engenheiro de ML/DL e C++/Python · IA industrial · Energia e automação

**Desenvolvo sistemas na interseção entre aprendizado de máquina, C++ moderno e engenharia industrial.** Meus projetos combinam modelos ML/DL, computação nativa, telemetria e sistemas de busca—do significado de um sinal ao comportamento do software que o processa.

Meu foco está nos desafios técnicos: dados ruidosos, recuperação de falhas, concorrência, avaliação de modelos e compromissos de desempenho mensuráveis.

## Projetos de engenharia

### [ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO) — aprendizado de máquina para diagnóstico de equipamentos
Características de sinais em C++20 via pybind11, detecção clássica de anomalias, modelos PyTorch LSTM/GRU e inferência ONNX. São documentadas as divisões de dados, baselines, procedência e abstenção: o sistema pode recusar uma estimativa sem evidências suficientes.

**Para verificar:** [contrato de confiabilidade](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/main/docs/RELIABILITY.md) · [artefatos de experimentos](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/tree/main/experiments) · [CI](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/actions).

### [Ironpulse](https://github.com/Anton-Sergeev-EA/Ironpulse) — telemetria industrial resiliente em C++20
Coleta assíncrona Modbus TCP, limites de tempo e reconexão, armazenamento WAL, detecção estatística de anomalias e interfaces REST/WebSocket. O foco é o comportamento durante falhas de comunicação e armazenamento.

**Para verificar:** [testes](https://github.com/Anton-Sergeev-EA/Ironpulse/tree/main/tests) · [compilação, sanitizers e integração](https://github.com/Anton-Sergeev-EA/Ironpulse/actions).

### [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore) — busca local de documentos e RAG
Índices vetoriais exatos/aproximados em C++ integrados ao Python, embeddings, BM25 e APIs. Testes de índices e benchmarks com cargas específicas permitem inspecionar a busca e os compromissos de desempenho.

**Para verificar:** [implementação nativa](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/native) · [benchmarks](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/benchmarks) · [CI](https://github.com/Anton-Sergeev-EA/Cognivore/actions).

### Outros sistemas

- **[GridGuard](https://github.com/Anton-Sergeev-EA/GridGuard):** Laboratório IEC 61850 MMS/URCB, qualidade da telemetria, WAL protegido por CRC e reaplicação no banco de dados.
- **[SCADA_Generator](https://github.com/Anton-Sergeev-EA/SCADA_Generator):** HMI gerada por configuração, adaptadores de protocolos industriais, ciclo de vida de alarmes e análise C++/Python.
- **[adaptive_capacity_allocator](https://github.com/Anton-Sergeev-EA/adaptive_capacity_allocator):** Políticas de crescimento de contêineres C++17/20 com medições reproduzíveis de memória e tempo.

## Ferramentas técnicas

| Área | Tecnologias e métodos |
|---|---|
| Machine Learning e Deep Learning | PyTorch, scikit-learn, LightGBM/XGBoost, LSTM/GRU, anomalias, séries temporais, PCA, ONNX |
| Software e dados | C++17/20, Python, CMake, pybind11, FastAPI, REST/WebSocket, PostgreSQL, SQLite |
| Busca e entrega | RAG, embeddings, BM25, busca vetorial, Linux, Docker, GitHub Actions, pytest, CTest, Ruff, sanitizers |

## Abordagem de engenharia

Transformo requisitos operacionais em contratos de software testáveis, avalio modelos em relação aos dados e baselines e meço antes de afirmar ganhos de desempenho. Experimentos ML sintéticos e testes de protocolos em laboratório demonstram seu escopo documentado, não precisão em campo, implantação ou certificação. Cada repositório descreve seus limites.

**Contato:** [avsergeev1981@gmail.com](mailto:avsergeev1981@gmail.com) · [Apollonian](https://apollonian.ru/) · [todos os repositórios](https://github.com/Anton-Sergeev-EA/?tab=repositories).
