# Ledger Status

**Project:** `L_SEMANTICA`  
**Tier:** TIER_4_INFERENCE_AGENTS  
**Identity:** Upstream `ExtensityAI/symbolicai` @ `44d13560e4f1` (BSD-3-Clause)

## Chain state

| Fact | Value |
| --- | --- |
| Upstream | `ExtensityAI/symbolicai` |
| Commit | `44d13560e4f13c19c10b00aac0613816fbe8d414` |
| Upstream licence | BSD-3-Clause |
| Licence class | permissive |
| Clone size | 22.69 MB |
| Ledger | 0 blocks, chain verified |
| Current TRL | NOT YET MEASURED |
| Post-optimisation TRL | NOT YET MEASURED |
| II budget cap | 1000.0 IIU |
| Verified upstream edits | 1 |

- Blocks: **0**
- Head digest: `None`
- Chain verification: **verified**

## Independent verification

The chain is verifiable without trusting this project's tooling:

```
anticloud ledger verify
anticloud ledger export > ledger.jsonl
```

Each block carries the previous block's digest, so removing or reordering an
entry invalidates every block after it. That property is the reason the
ledger can stand in for a claim of what happened.
