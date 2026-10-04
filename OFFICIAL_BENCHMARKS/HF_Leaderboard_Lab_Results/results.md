# HF_Leaderboard_Lab_Results

**Project:** `K_ALPA`  
**Tier:** `TIER_5_WORLD_NEURO_EMBODIED`  
**Slug:** `alpa-projects/alpa`  
**Commit:** `b8078a9f75cb`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **49.65 ms** |
| Min latency | 41.64 ms |
| Max latency | 56.0 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **41** |
| Tokenization latency | 1.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5863 |
| Classification latency | 229.01 ms |
| Status | **PASS** |

**Input text tokenized:**
```
K_ALPA (alpa-projects/alpa) — 388 files, 70798 source lines, licence Apache-2.0, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'k', '_', 'al', '##pa', '(', 'al', '##pa', '-', 'projects', '/', 'al', '##pa', ')', '—', '38', '##8', 'files', ',', '70']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_