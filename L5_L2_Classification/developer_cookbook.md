# Developer Cookbook — K_ALPA
**Stack:** Python 3.11, JAX 0.4+, Alpa 0.x, CUDA 12.x, multi-GPU, AIOSS_FORMAT
**Domain:** Distributed model parallelism for large-scale PAX training across multi-GPU nodes

## Distributed training setup
```python
from k_alpa import AlpaTrainer

trainer = AlpaTrainer(
    model_config="./pax_27b_config.json",
    parallelism="auto",  # Alpa auto-selects optimal strategy
    aioss_chain="./alpa_training.aioss"
)

trainer.train(
    dataset="./anticloud_training_data/",
    n_steps=10000,
    checkpoint_every=500
)
```

## Manual parallelism strategy
```python
from k_alpa import PipelineMesh
mesh = PipelineMesh(pipeline_stages=4, tensor_parallel=2)
trainer = AlpaTrainer(model_config="./pax_27b_config.json", mesh=mesh)
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
