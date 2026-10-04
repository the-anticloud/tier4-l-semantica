# HF_Leaderboard_Lab_Results

**Project:** `L_SEMANTICA`  
**Tier:** `TIER_4_INFERENCE_AGENTS`  
**Slug:** `ExtensityAI/symbolicai`  
**Commit:** `44d13560e4f1`  
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
| Avg latency | **46.22 ms** |
| Min latency | 39.54 ms |
| Max latency | 54.5 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **40** |
| Tokenization latency | 1.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5841 |
| Classification latency | 72.51 ms |
| Status | **PASS** |

**Input text tokenized:**
```
L_SEMANTICA (ExtensityAI/symbolicai) — 288 files, 49833 source lines, licence BSD-3-Clause, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'l', '_', 'semantic', '##a', '(', 'ex', '##tens', '##ity', '##ai', '/', 'symbolic', '##ai', ')', '—', '288', 'files', ',', '49', '##8']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_