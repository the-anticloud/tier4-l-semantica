# 3-Seed Simulation — L_SEMANTICA

**Seeds:** `56924` · `88261` · `22460`

**Seed method:** `sha256("L_SEMANTICA")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `L_SEMANTICA`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 7.132 | 0.1737 | ±0.3405 |
| throughput_tokens_per_sec | 1026.0 | 33.3336 | ±65.3339 |
| p50_latency_ms | 45.89 | 4.4566 | ±8.7349 |
| p99_latency_ms | 107.49 | 6.4058 | ±12.5554 |
| ttft_ms | 29.9567 | 1.2422 | ±2.4347 |
| mmlu_proxy | 0.7155 | 0.0262 | ±0.0514 |
| hellaswag_proxy | 0.7694 | 0.0302 | ±0.0592 |
| truthfulqa_proxy | 0.5817 | 0.0476 | ±0.0933 |
| arc_proxy | 0.688 | 0.0388 | ±0.076 |
| complexity_cyclomatic | 4.7167 | 0.2894 | ±0.5672 |
| maintainability_index | 71.81 | 4.3629 | ±8.5513 |
| security_issues_high | 0.3333 | 0.4714 | ±0.9239 |
| dependency_freshness_pct | 79.8333 | 2.2647 | ±4.4388 |
| test_coverage_pct | 62.1667 | 3.7748 | ±7.3986 |
| doc_coverage_pct | 62.0333 | 5.9421 | ±11.6465 |
| memory_mb | 186.6667 | 11.0708 | ±21.6988 |
| gpu_util_pct | 71.0333 | 5.8437 | ±11.4537 |
| openssf_score | 6.2467 | 0.4781 | ±0.9371 |
| eu_ai_act_compliance_pct | 77.3667 | 0.7134 | ±1.3983 |
| slsa_level | 1.6667 | 0.4714 | ±0.9239 |

## Per-Seed Raw Results

| Metric | Seed 56924 | Seed 88261 | Seed 22460 |
|--------|------------|------------|------------|
| trl_score | 7.239 | 7.27 | 6.887 |
| throughput_tokens_per_sec | 979.2 | 1044.5 | 1054.3 |
| p50_latency_ms | 52.18 | 42.4 | 43.09 |
| p99_latency_ms | 101.46 | 104.65 | 116.36 |
| ttft_ms | 28.58 | 31.59 | 29.7 |
| mmlu_proxy | 0.697 | 0.697 | 0.7525 |
| hellaswag_proxy | 0.806 | 0.7702 | 0.7321 |
| truthfulqa_proxy | 0.5152 | 0.6243 | 0.6056 |
| arc_proxy | 0.6333 | 0.7195 | 0.7111 |
| complexity_cyclomatic | 4.96 | 4.88 | 4.31 |
| maintainability_index | 74.86 | 65.64 | 74.93 |
| security_issues_high | 1 | 0 | 0 |
| dependency_freshness_pct | 77.5 | 82.9 | 79.1 |
| test_coverage_pct | 59.7 | 59.3 | 67.5 |
| doc_coverage_pct | 63.6 | 68.4 | 54.1 |
| memory_mb | 186.1 | 173.4 | 200.5 |
| gpu_util_pct | 63.7 | 78.0 | 71.4 |
| openssf_score | 6.34 | 5.62 | 6.78 |
| eu_ai_act_compliance_pct | 76.4 | 77.6 | 78.1 |
| slsa_level | 2 | 2 | 1 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._