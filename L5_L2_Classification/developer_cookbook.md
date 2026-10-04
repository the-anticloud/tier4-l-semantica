# Developer Cookbook — L_SEMANTICA
**Stack:** Python 3.11, spaCy 3.7+, PAX 27B, SQLite (intent DB), AIOSS_FORMAT
**Domain:** Semantica: semantic parsing and intent classification for PAX 27B query understanding

## Parse query intent
```python
from l_semantica import SemanticParser

parser = SemanticParser(
    pax_model="./pax-27b-q4.gguf",
    intent_db="./semantica_intents.db",
    aioss_chain="./semantica.aioss"
)

result = parser.parse("Analyze this EEG signal for seizure activity in a HIPAA-compliant way")
print(f"Intent: {result.intent}")        # clinical_analysis
print(f"Domain: {result.domain}")        # TIER_7_BIOSIGNALS_NEURO
print(f"Entities: {result.entities}")    # [EEG, seizure, HIPAA]
print(f"Compliance: {result.compliance_flags}")  # [HIPAA]
print(f"Route to: {result.routing_target}")  # PAX_INFERENCE_CORE + K_BRAINFLOW
print(f"Chain: {result.chain_hash}")
```

## Train intent classifier on new domain
```python
parser.train_intent(
    examples=[
        ("analyze RF signal for jamming", "rf_security", "TIER_8"),
        ("detect GPS spoofing in GNSS data", "rf_security", "TIER_8"),
    ]
)
```

## Batch classification
```python
results = parser.batch_parse(queries)
domain_dist = {r.domain: sum(1 for x in results if x.domain == r.domain) for r in results}
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
