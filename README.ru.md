[English](README.md) · **Русский** · [中文](README.zh.md) · [हिन्दी](README.hi.md) · [Español](README.es.md) · [العربية](README.ar.md) · [Français](README.fr.md) · [Português](README.pt.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [Italiano](README.it.md) · [Ελληνικά](README.el.md) · [Čeština](README.cs.md)

# Антон Сергеев
### Инженер ML/DL и разработчик C++/Python · Промышленный ИИ · Энергетика и автоматизация

**Разрабатываю системы на стыке машинного обучения, современного C++ и промышленной инженерии.** Мои проекты объединяют ML/DL-модели, нативные вычисления, телеметрию и поисковые системы — от понимания сигнала до поведения программного комплекса, который его обрабатывает.

Мой фокус — сложные инженерные задачи: шумные данные, восстановление после сбоев, многопоточность, оценка моделей и измеримые компромиссы производительности.

## Избранные инженерные проекты

### [ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO) — машинное обучение для диагностики оборудования
Извлечение признаков на C++20 через pybind11, классические детекторы аномалий, модели PyTorch LSTM/GRU и инференс ONNX. Документированы разбиения данных, базовые модели, происхождение данных и отказ от выдачи неподтверждённой оценки.

**Для проверки:** [контракт надёжности](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/main/docs/RELIABILITY.md) · [артефакты экспериментов](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/tree/main/experiments) · [CI](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/actions).

### [Ironpulse](https://github.com/Anton-Sergeev-EA/Ironpulse) — устойчивая промышленная телеметрия на C++20
Асинхронный сбор Modbus TCP, тайм-ауты и восстановление соединения, хранение WAL, статистические детекторы аномалий и REST/WebSocket. Основной акцент — поведение системы при сбоях связи и хранения.

**Для проверки:** [тесты](https://github.com/Anton-Sergeev-EA/Ironpulse/tree/main/tests) · [сборка, санитайзеры и интеграционные проверки](https://github.com/Anton-Sergeev-EA/Ironpulse/actions).

### [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore) — локальный поиск по документам и RAG
Индексы точного и приближённого векторного поиска на C++ с интеграцией в Python, embeddings, BM25 и API. Тесты индексов и измерения на конкретных нагрузках показывают поведение поиска и компромиссы производительности.

**Для проверки:** [нативная реализация](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/native) · [бенчмарки](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/benchmarks) · [CI](https://github.com/Anton-Sergeev-EA/Cognivore/actions).

### Другие системные проекты

- **[GridGuard](https://github.com/Anton-Sergeev-EA/GridGuard):** лаборатория IEC 61850 MMS/URCB, качество телеметрии, WAL с CRC и повторная запись в БД.
- **[SCADA Generator](https://github.com/Anton-Sergeev-EA/SCADA_Generator):** HMI из конфигурации, промышленные протоколы, жизненный цикл аварийных сообщений и аналитика C++/Python.
- **[Adaptive capacity allocator](https://github.com/Anton-Sergeev-EA/adaptive_capacity_allocator):** политики роста контейнеров C++17/20 с воспроизводимыми измерениями памяти и времени.

## Технический инструментарий

| Направление | Технологии и методы |
|---|---|
| Машинное и глубокое обучение | PyTorch, scikit-learn, LightGBM/XGBoost, LSTM/GRU, аномалии, временные ряды, PCA, ONNX |
| Разработка и данные | C++17/20, Python, CMake, pybind11, FastAPI, REST/WebSocket, PostgreSQL, SQLite |
| Поиск и поставка ПО | RAG, embeddings, BM25, векторный поиск, Linux, Docker, GitHub Actions, pytest, CTest, Ruff, санитайзеры |

## Подход к работе

Перевожу эксплуатационные требования в проверяемые программные контракты, оцениваю модели относительно данных и базовых решений, измеряю производительность до заявлений об ускорении.  синтетические ML-эксперименты и протокольные стенды показывают заявленный лабораторный результат, а не точность на реальном объекте, внедрение или сертификацию. Границы описаны в каждом репозитории.

**Связь:** [avsergeev1981@gmail.com](mailto:avsergeev1981@gmail.com) · [Apollonian](https://apollonian.ru/) · [все репозитории](https://github.com/Anton-Sergeev-EA?tab=repositories).
