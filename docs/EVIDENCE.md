# Evidence behind the profile

The profile distinguishes recorded repository measurements from a new local verification. Measurements describe their stated workload, not field performance, certification or a customer deployment.

## ARGUS-NEURO — recorded synthetic experiment

Source snapshot: [`289671868e36cd1dee7a9ca55410851482e61e44`](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/tree/289671868e36cd1dee7a9ca55410851482e61e44).

The figure is rendered from the `revised` entries in [`metrics.json`](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/289671868e36cd1dee7a9ca55410851482e61e44/experiments/2026-09-30_reliability/metrics.json). It is a visualization of recorded results, not a new training run or live inference demo.

- Autoencoder: seed 3, 12 epochs, 2,030 held-out synthetic windows; TP 282, FP 79, FN 200, TN 1,469; precision 0.7812, recall 0.5851, F1 0.6690. Trajectories are split across training, validation and test. The separate spectral baseline uses 230 waveform examples and must not be compared as if it used the same test set.
- RUL: seed 5, 15 epochs; normalized test MAE 0.187539 versus 0.288046 for the training-target median predictor on the same held-out test set. The target is a synthetic countdown with a 3,000-second horizon, not measured equipment lifetime.
- [`config.json`](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/289671868e36cd1dee7a9ca55410851482e61e44/experiments/2026-09-30_reliability/config.json) records the original experiment date as 2026-09-30, starting commit `fd64b9d355e62f97986a8e90bd7e1f59c89fabe9` and `uncommitted_changes: true`. The saved [`diff.patch`](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/289671868e36cd1dee7a9ca55410851482e61e44/experiments/2026-09-30_reliability/diff.patch) is part of the provenance. This is a protocol repair experiment, not a controlled single-parameter comparison.

Inspect the [reliability contract](https://github.com/Anton-Sergeev-EA/ARGUS-NEURO/blob/289671868e36cd1dee7a9ca55410851482e61e44/docs/RELIABILITY.md), configuration, metrics and saved diff before reproducing `bash scripts/train_all.sh` in the documented project environment.

## Ironpulse — local build, tests and real simulator

Source snapshot: [`ff989c50f1e67ea7a65405904ab7dc73f6be6303`](https://github.com/Anton-Sergeev-EA/Ironpulse/tree/ff989c50f1e67ea7a65405904ab7dc73f6be6303).

Verified on 2026-10-13 with GCC 13, Debug configuration and warnings treated as errors:

```bash
cmake --preset debug -DIRONPULSE_WARNINGS_AS_ERRORS=ON
cmake --build --preset debug -j2
ctest --preset debug --output-on-failure
```

Result: **140 / 140 tests passed**. This includes API, WebSocket authentication and the pipeline test that marks a stopped device offline and recovers when it responds again. The initial restricted environment prevented socket creation; the full suite passed after local network access was enabled.

The dashboard screenshot is from the actual C++ executable receiving synthetic Modbus readings from the repository's Python simulator, using `pymodbus==3.6.9`. Two devices and four sensors were configured from [`config.example.json`](https://github.com/Anton-Sergeev-EA/Ironpulse/blob/ff989c50f1e67ea7a65405904ab7dc73f6be6303/deploy/config/config.example.json). For the local capture, HTTP/WebSocket ports were changed to 18080/18081, the data directory was isolated and notification channels were empty. No device hardware or external notification service was involved.

During the manual check, `/api/v1/devices` reported both devices online, both offline after stopping the simulator, and both online after restarting it. This verifies that scenario without claiming a recovery-time benchmark. `/healthz` and `/api/v1/sensors` were also checked. Persistence was enabled; the capture is not a crash-durability benchmark. Batched WAL writes have documented loss limits in [ADR 0002](https://github.com/Anton-Sergeev-EA/Ironpulse/blob/ff989c50f1e67ea7a65405904ab7dc73f6be6303/docs/adr/0002-storage-format.md).

Reproduction: follow the repository setup, run the simulator and executable with a local configuration, observe live readings, then stop and restart the simulator. Keep an unauthenticated demonstration local; configure API authentication for shared deployments.

## Cognivore — published interface and benchmark

Source snapshot: [`8ca2aaad23280cf283731191be442c398f0f6ed1`](https://github.com/Anton-Sergeev-EA/Cognivore/tree/8ca2aaad23280cf283731191be442c398f0f6ed1).

The image is the repository's [`web-ui-en.png`](https://github.com/Anton-Sergeev-EA/Cognivore/blob/8ca2aaad23280cf283731191be442c398f0f6ed1/docs/screenshots/web-ui-en.png), not a newly executed session. The benchmark numbers come from the [recorded table](https://github.com/Anton-Sergeev-EA/Cognivore/blob/8ca2aaad23280cf283731191be442c398f0f6ed1/README.md#benchmarks) and [`bench_index.py`](https://github.com/Anton-Sergeev-EA/Cognivore/blob/8ca2aaad23280cf283731191be442c398f0f6ed1/benchmarks/bench_index.py); they were not rerun for this profile update.

- Workload: uniform random, 384-dimensional vectors on a reported 2-core CI-class machine. Exact CPU model, distribution of timings and uncertainty are not specified in that table.
- Index construction for 3,000 vectors: C++ 0.027 seconds versus NumPy 0.615 seconds with `.add()` in a loop. This comparison does not measure full application speed or all possible NumPy implementations.
- NSW at 3,000 vectors and `ef=150`: Recall@10 0.93, 0.46 ms/query. At `ef=50`: 0.64 and 0.24 ms; at `ef=400`: 1.00 and 0.78 ms.
- Exact search is faster in the reported 1,000- and 10,000-vector workloads. The graph index becomes faster in the reported 50,000-vector workload. Choose against the actual workload rather than extrapolating a universal speedup.

To reproduce: use the repository's documented environment, run `python benchmarks/bench_index.py`, and record the CPU, thread count, versions, random seed and repeated timings alongside recall. See the [architecture decisions](https://github.com/Anton-Sergeev-EA/Cognivore/blob/8ca2aaad23280cf283731191be442c398f0f6ed1/docs/architecture.md) and native/fallback parity tests.

## Reading path

Start with the three visuals, inspect the metric sources and engineering decisions, then run the chosen project's documented tests. The architecture diagram presents independent pipelines; it does not claim that all three products form one deployed system. External adoption, customer results and independent reviews should only be added with verifiable public evidence.

## Cognivore agent harness

The [CLI](https://github.com/Anton-Sergeev-EA/Cognivore/blob/01689074017726ebe3191c222d07f53350232512/src/cognivore/cli.py) exposes `run-task`, `resume-task` and `publish-task`. The [recovery test](https://github.com/Anton-Sergeev-EA/Cognivore/blob/01689074017726ebe3191c222d07f53350232512/tests/test_resumable_task.py) interrupts the agent after a tool call, reopens the SQLite database, checks that the tool call is not replayed, and verifies that repeated approval returns the same published report. Run `pytest tests/test_resumable_task.py tests/test_comparison_workflow.py` in Cognivore.

## Cognivore browser specification review

The profile screenshot shows the English telemetry gateway demo running locally in Chrome. The [earlier revision](https://github.com/Anton-Sergeev-EA/Cognivore/blob/bc037323eb646cc82bb230969743d9b6a11d3dfa/src/cognivore/web/static/demo-before.md) and [later revision](https://github.com/Anton-Sergeev-EA/Cognivore/blob/bc037323eb646cc82bb230969743d9b6a11d3dfa/src/cognivore/web/static/demo-after.md) produce five annotated findings with the offline hashing embedder. This is a demonstration case.

The [matching tests](https://github.com/Anton-Sergeev-EA/Cognivore/blob/f1ee363dbd937f4e17cb86b9fbe5c455dd0cec24/tests/test_review.py) cover the annotated changes, ambiguous matches, and signal detection in German and Russian. The [web test](https://github.com/Anton-Sergeev-EA/Cognivore/blob/f1ee363dbd937f4e17cb86b9fbe5c455dd0cec24/tests/test_review_web.py) covers recovery after reopening the app, approval and export. Run `pytest tests/test_review.py tests/test_review_web.py` in Cognivore.

The [specification review benchmark](https://github.com/Anton-Sergeev-EA/Cognivore/blob/f1ee363dbd937f4e17cb86b9fbe5c455dd0cec24/benchmarks/REVIEW.md) compares Cognivore with line diff and greedy cosine matching. On ten synthetic pairs, Cognivore returned 13 correct findings, zero extra and zero missed. The line and cosine baselines returned 3 and 8 correct findings, respectively. The offline hashing configuration missed the intended NIST alignment. The benchmark records the corpus, evaluation rules and CPU timing procedure.

On two published examples from NIST and WCAG, MiniLM returned one exact finding using line text alone and two with section context. Line diff also found both changes. The NIST case was known during development and the two-case sample is a regression check. [Published-case results](https://github.com/Anton-Sergeev-EA/Cognivore/blob/f1ee363dbd937f4e17cb86b9fbe5c455dd0cec24/benchmarks/REVIEW.md#section-context-on-published-cases)
