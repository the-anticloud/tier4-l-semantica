# Deploy Guide — L_SEMANTICA
**Tier:** TIER_4_INFERENCE_AGENTS | **Stack:** Python 3.11, spaCy 3.7+, PAX 27B, SQLite (intent DB), AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, spaCy 3.7+, PAX 27B weights, SQLite intent database.

## Environment
4GB RAM. GPU for PAX semantic analysis. CPU for spaCy parsing.

## AIOSS Integration
```bash
aioss init --module L_SEMANTICA --output ./l_semantica.aioss
aioss append --chain ./l_semantica.aioss --payload ./output.bin --module L_SEMANTICA
aioss verify --chain ./l_semantica.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="L_SEMANTICA",
    aioss_chain="./L_SEMANTICA.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./L_SEMANTICA.aioss --verbose
python -m L_SEMANTICA.tests.smoke
```
