[English](README.md) · [Русский](README.ru.md) · **中文** · [हिन्दी](README.hi.md) · [Español](README.es.md) · [العربية](README.ar.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [Italiano](README.it.md)

# 安东·谢尔盖耶夫
### ML/DL 与 C++/Python 工程师 · 工业人工智能 · 电力系统与自动化

**我将工业领域知识与软件工程、机器学习结合起来。** 我的经历涵盖电气设备诊断、过程自动化和技术项目管理。目前，我开发用于监测、预测和工程决策支持的 ML/DL 模型、原生计算模块及数据服务。

我的优势是理解完整的问题：测量值代表什么、设备如何发生故障、数据如何进入模型，以及通信或组件失效时软件系统如何运行。

## 专业经历

- **2001–2023 · 工程与管理岗位：** 对 **0.4–750 kV** 电气设备进行诊断，包括局部放电和介质损耗测量；负责大型工业项目的自动化工作。
- **工业项目：** 西布尔集团托博尔斯克聚丙烯工厂的过程自动化，以及俄罗斯天然气工业股份公司 **120 MW 电站项目**；参与列宁格勒核电站二期和拉夫纳港等项目的电气、控制与通信工作。
- **自 2024 年 9 月起 · Apollonian：** 机器学习工程与项目管理；面向振动、压力和温度遥测数据开发 LSTM 与梯度提升模型；数据缓冲、S3 归档及 REST/WebSocket 集成。
- **教育：** 圣彼得堡彼得大帝理工大学电力工程硕士，**2021 年**。进一步学习 ML/DL、计算机视觉、RAG、C++、Python 与 DevOps。

工业经历帮助我定义软件需求；以下公开项目展示可供审阅的实现与评估方法。

## 精选工程项目

### [ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO) — 设备诊断机器学习
通过 pybind11 暴露 C++20 信号特征，结合传统异常检测、PyTorch LSTM/GRU 与 ONNX 推理。可靠性工作记录数据划分、基线、数据来源和拒绝输出机制：系统可以拒绝提供证据不足的估计。

**审阅：** [可靠性约定](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/main/docs/RELIABILITY.md) · [实验产物](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/tree/main/experiments) · [CI](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/actions)。

### [Ironpulse](https://github.com/Anton-Sergeev-EA/Ironpulse) — C++20 工业遥测与故障恢复
异步 Modbus TCP 采集、超时与重连、WAL 存储、统计异常检测及 REST/WebSocket 接口。重点是通信和存储发生故障时系统仍能保持有用的行为。

**审阅：** [测试](https://github.com/Anton-Sergeev-EA/Ironpulse/tree/main/tests) · [构建、sanitizer 与集成 CI](https://github.com/Anton-Sergeev-EA/Ironpulse/actions)。

### [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore) — 本地文档检索与 RAG
与 Python 集成的 C++ 精确/近似向量索引、嵌入、BM25 检索和 API。索引测试与特定负载基准展示检索行为及性能取舍。

**审阅：** [原生实现](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/native) · [基准测试](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/benchmarks) · [CI](https://github.com/Anton-Sergeev-EA/Cognivore/actions)。

### 其他系统项目

- **[GridGuard](https://github.com/Anton-Sergeev-EA/GridGuard)：** IEC 61850 MMS/URCB 实验平台、遥测质量、CRC 保护的 WAL 与数据库重放。
- **[SCADA Generator](https://github.com/Anton-Sergeev-EA/SCADA_Generator)：** 配置生成 HMI、工业协议适配器、报警生命周期与 C++/Python 分析。
- **[Adaptive capacity allocator](https://github.com/Anton-Sergeev-EA/adaptive_capacity_allocator)：** C++17/20 容器增长策略及可复现的内存/时间取舍测量。

## 技术工具

| 领域 | 技术与方法 |
|---|---|
| 机器学习与深度学习 | PyTorch、scikit-learn、LightGBM/XGBoost、LSTM/GRU、异常检测、时间序列、PCA、ONNX |
| 软件与数据 | C++17/20、Python、CMake、pybind11、FastAPI、REST/WebSocket、PostgreSQL、SQLite |
| 检索与交付 | RAG、嵌入、BM25、向量检索、Linux、Docker、GitHub Actions、pytest、CTest、Ruff、sanitizer |

## 工作方法

我将运行需求转化为可测试的软件约定，以数据和基线为依据评估模型，并在提出性能结论前进行测量。**工业任职经历与公开项目验证是两个不同层面：** 合成数据实验和实验室协议测试只证明其明确的测试范围，不代表现场准确性、部署或认证。各项目说明自身限制。

## 工作与合作

关注 **ML/DL 工程、C++/Python 开发及工业人工智能**：诊断、预测、检索系统、遥测和可靠的数据服务。愿意搬迁并加入国际团队。

**联系：** [kavery@mail.ru](mailto:kavery@mail.ru) · [Apollonian](https://apollonian.ru/) · [全部项目](https://github.com/Anton-Sergeev-EA?tab=repositories)。
