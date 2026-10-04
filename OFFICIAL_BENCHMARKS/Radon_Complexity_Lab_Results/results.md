# Radon_Complexity_Lab_Results
**Project:** `L_SEMANTICA` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'A', 'score': 2.9204771371769382}`
- **complexity_grade:** `A`
- **complexity_score:** `2.9204771371769382`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_SEMANTICA\UPSTREAM\symai\components.py - B (16.07)
E:\fenta\D`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_SEMANTICA\UPSTREAM\symai\components.py
    M 354:4 MetadataTracker._accumulate_completion_token_details - C (18)
    M 568:4 DynamicEngine._create_engine_instance - C (11)
    M 720:4 ChonkieChunker._resolve_chunker - B (9)
    M 121:4 FileReader.forward - B (8)
    M 279:4 MetadataTracker.__str__ - B (7)
    M 313:4 MetadataTracker._trace_calls - B (7)
    M 253:4 PrimitiveDisabler._extract_primitives - B (6)
    M 486:4 MetadataTracker._track_parallel_usage_items - B (6)
    C 52:0 FileReader - A (5)
    M 66:4 FileReader.get_files - A (5)
    C 270:0 MetadataTracker - A (5)
    M 334:4 MetadataTracker._accumulate_usage_record - A (5)
    C 222:0 PrimitiveDisabler - A (4)
    M 241:4 PrimitiveDisabler._disable_primitives - A (4)
    C 508:0 DynamicEngine - A (4)
    C 688:0 ChonkieChunker - A (4)
    F 618:0 _lazy_import_chonkie - A (3)
    F 673:0 _get_chunker_mapping - A (3)
    F 680:0 _is_chonkie_available - A (3)
    C 28:0 Interface - A (3)
    M 54:4 FileReader.exists - A (3)
    M 105:4 FileReader.integrity_check - A (3)
    C 140:0 Function - A (3)
    M 175:4 Function.prompt - A (3)
    M 228:4 PrimitiveDisabler.__enter__ - A (3)
    M 248:4 PrimitiveDisabler._enable_primitives - A (3)
    M 554:4 DynamicEngine.__exit__ - A (3)
    M 701:4 ChonkieChunker.forward - A (3)
    M 710:4 ChonkieChunker._get_tokenizer - A (3)
    M 35:4 Interface.__new__ - A (2)
    M 44:4 Interface.load_module_class - A (2)
    
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_