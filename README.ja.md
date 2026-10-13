[English](README.md) · [Русский](README.ru.md) · [中文](README.zh.md) · [हिन्दी](README.hi.md) · [Español](README.es.md) · [العربية](README.ar.md) · [Deutsch](README.de.md) · **日本語** · [Italiano](README.it.md)

# アントン・セルゲーエフ
### ML/DL・C++/Python エンジニア · 産業 AI · 電力システムと自動化

**産業分野の知識を、ソフトウェア工学と機械学習につなげています。** 電気設備の診断、プロセス自動化、技術プロジェクトのマネジメントを経験してきました。現在は監視、予測、技術的意思決定の支援に向けて、ML/DL モデル、ネイティブ計算モジュール、データサービスを開発しています。

私の強みは問題を全体として捉えることです。測定値の意味、設備の故障の仕組み、モデルまでのデータの流れ、通信やコンポーネントが停止した際のソフトウェアの動作を考慮します。

## 職務経験

- **2001–2023 · エンジニアリングと管理業務：** **0.4–750 kV** の電気設備を診断。部分放電や誘電損失の測定、大規模産業プロジェクトの自動化業務の指揮を担当。
- **産業プロジェクト：** トボリスクの SIBUR ポリプロピレン工場、および Gazprom の **120 MW 発電所プロジェクト**のプロセス自動化。Leningrad NPP-2 や Lavna 港などのプロジェクトで電気・制御・通信業務に従事。
- **2024 年 9 月から · Apollonian：** ML エンジニアリングとプロジェクト管理。振動・圧力・温度のテレメトリを扱う LSTM と勾配ブースティング、データのバッファリング、S3 アーカイブ、REST/WebSocket による統合。
- **学歴：** ピョートル大帝サンクトペテルブルク工科大学、電力工学修士、**2021 年**。ML/DL、コンピュータビジョン、RAG、C++、Python、DevOps の追加研修。

産業での経験をソフトウェア開発に生かしています。以下の公開リポジトリでは、実装と評価方法を確認できます。

## 主な開発プロジェクト

### [ARGUS-NEURO](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO) — 設備診断の機械学習
pybind11 で公開する C++20 信号特徴量、従来型の異常検知、PyTorch LSTM/GRU、ONNX 推論。データ分割、ベースライン、データ由来、根拠が不十分な推定を出力しない仕組みを文書化しています。

**確認：** [信頼性に関する契約](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/main/docs/RELIABILITY.md) · [実験成果物](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/tree/main/experiments) · [CI](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/actions)。

### [Ironpulse](https://github.com/Anton-Sergeev-EA/Ironpulse) — C++20 による障害に強い産業テレメトリ
非同期 Modbus TCP 収集、タイムアウトと再接続、WAL 保存、統計的異常検知、REST/WebSocket インターフェース。通信や保存に障害が起きた際の動作を重視しています。

**確認：** [テスト](https://github.com/Anton-Sergeev-EA/Ironpulse/tree/main/tests) · [ビルド・sanitizer・統合 CI](https://github.com/Anton-Sergeev-EA/Ironpulse/actions)。

### [Cognivore](https://github.com/Anton-Sergeev-EA/Cognivore) — ローカル文書検索と RAG
Python と連携する C++ の厳密・近似ベクトル索引、埋め込み、BM25 検索、API。索引テストと特定の負荷に対するベンチマークにより、検索動作と性能上のトレードオフを検証できます。

**確認：** [ネイティブ実装](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/native) · [ベンチマーク](https://github.com/Anton-Sergeev-EA/Cognivore/tree/main/benchmarks) · [CI](https://github.com/Anton-Sergeev-EA/Cognivore/actions)。

### その他のシステム開発

- **[GridGuard](https://github.com/Anton-Sergeev-EA/GridGuard)：** IEC 61850 MMS/URCB の実験環境、テレメトリ品質、CRC 保護 WAL、データベースへのリプレイ。
- **[SCADA Generator](https://github.com/Anton-Sergeev-EA/SCADA_Generator)：** 設定から生成する HMI、産業プロトコルアダプター、アラームのライフサイクル、C++/Python 分析。
- **[Adaptive capacity allocator](https://github.com/Anton-Sergeev-EA/adaptive_capacity_allocator)：** C++17/20 コンテナの拡張方針と、再現可能なメモリ・時間測定。

## 技術と手法

| 分野 | 技術・手法 |
|---|---|
| 機械学習・深層学習 | PyTorch、scikit-learn、LightGBM/XGBoost、LSTM/GRU、異常検知、時系列、PCA、ONNX |
| ソフトウェア・データ | C++17/20、Python、CMake、pybind11、FastAPI、REST/WebSocket、PostgreSQL、SQLite |
| 検索・デリバリー | RAG、埋め込み、BM25、ベクトル検索、Linux、Docker、GitHub Actions、pytest、CTest、Ruff、sanitizer |

## 開発方針

運用上の要件をテスト可能なソフトウェア契約に変換し、データとベースラインに基づいてモデルを評価し、性能を主張する前に測定します。**産業での職務経験と公開プロジェクトの検証は別のものです。** 合成データによる ML 実験や実験室のプロトコル試験は、文書化された範囲を示すものであり、現場での精度、導入、認証を証明するものではありません。制約は各リポジトリに記載しています。

## 仕事と協業

**ML/DL エンジニアリング、C++/Python 開発、産業 AI**に関心があります。対象は診断、予測、検索システム、テレメトリ、信頼性の高いデータサービスです。転居と国際チームでの勤務に対応できます。

**連絡先：** [kavery@mail.ru](mailto:kavery@mail.ru) · [Apollonian](https://apollonian.ru/) · [全リポジトリ](https://github.com/Anton-Sergeev-EA?tab=repositories)。
