# 3-Seed Simulation — K_ALPA

**Seeds:** `72874` · `4211` · `38410`

**Seed method:** `sha256("K_ALPA")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `K_ALPA`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 6.9603 | 0.1253 | ±0.2456 |
| throughput_tokens_per_sec | 1365.9333 | 31.7074 | ±62.1465 |
| p50_latency_ms | 42.51 | 4.0215 | ±7.8821 |
| p99_latency_ms | 112.6933 | 11.1548 | ±21.8634 |
| ttft_ms | 31.19 | 1.7439 | ±3.418 |
| mmlu_proxy | 0.7576 | 0.0262 | ±0.0514 |
| hellaswag_proxy | 0.7792 | 0.0328 | ±0.0643 |
| truthfulqa_proxy | 0.5696 | 0.0375 | ±0.0735 |
| arc_proxy | 0.6724 | 0.0318 | ±0.0623 |
| complexity_cyclomatic | 4.5267 | 0.6137 | ±1.2029 |
| maintainability_index | 76.06 | 4.3347 | ±8.496 |
| security_issues_high | 0.6667 | 0.9428 | ±1.8479 |
| dependency_freshness_pct | 80.9667 | 6.585 | ±12.9066 |
| test_coverage_pct | 49.5333 | 3.565 | ±6.9874 |
| doc_coverage_pct | 67.8 | 3.879 | ±7.6028 |
| memory_mb | 65.5333 | 2.1823 | ±4.2773 |
| gpu_util_pct | 71.7333 | 6.2941 | ±12.3364 |
| openssf_score | 6.7367 | 0.6791 | ±1.331 |
| eu_ai_act_compliance_pct | 84.2333 | 6.144 | ±12.0422 |
| slsa_level | 1.6667 | 0.4714 | ±0.9239 |

## Per-Seed Raw Results

| Metric | Seed 72874 | Seed 4211 | Seed 38410 |
|--------|------------|------------|------------|
| trl_score | 6.784 | 7.064 | 7.033 |
| throughput_tokens_per_sec | 1334.1 | 1354.5 | 1409.2 |
| p50_latency_ms | 41.83 | 37.96 | 47.74 |
| p99_latency_ms | 128.36 | 106.46 | 103.26 |
| ttft_ms | 29.44 | 33.57 | 30.56 |
| mmlu_proxy | 0.7206 | 0.7761 | 0.7761 |
| hellaswag_proxy | 0.8071 | 0.7974 | 0.7332 |
| truthfulqa_proxy | 0.5196 | 0.5792 | 0.61 |
| arc_proxy | 0.6318 | 0.6758 | 0.7095 |
| complexity_cyclomatic | 3.66 | 4.92 | 5.0 |
| maintainability_index | 79.09 | 69.93 | 79.16 |
| security_issues_high | 0 | 2 | 0 |
| dependency_freshness_pct | 84.8 | 71.7 | 86.4 |
| test_coverage_pct | 44.5 | 51.8 | 52.3 |
| doc_coverage_pct | 72.5 | 67.9 | 63.0 |
| memory_mb | 63.7 | 64.3 | 68.6 |
| gpu_util_pct | 75.2 | 77.1 | 62.9 |
| openssf_score | 7.35 | 7.07 | 5.79 |
| eu_ai_act_compliance_pct | 87.7 | 75.6 | 89.4 |
| slsa_level | 1 | 2 | 2 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._