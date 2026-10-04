# Deploy Guide — K_ALPA
**Tier:** TIER_5_WORLD_NEURO_EMBODIED | **Stack:** Python 3.11, JAX 0.4+, Alpa 0.x, CUDA 12.x, multi-GPU, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, JAX 0.4+, Alpa 0.x, multi-GPU (4x+ A100 recommended). CUDA 12.x. 256GB+ RAM.

## Environment
Multi-node GPU cluster. Minimum 4x A100 80GB for PAX 27B training. NVLink recommended.

## AIOSS Integration
```bash
aioss init --module K_ALPA --output ./k_alpa.aioss
aioss append --chain ./k_alpa.aioss --payload ./output.bin --module K_ALPA
aioss verify --chain ./k_alpa.aioss
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
    module="K_ALPA",
    aioss_chain="./K_ALPA.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./K_ALPA.aioss --verbose
python -m K_ALPA.tests.smoke
```
