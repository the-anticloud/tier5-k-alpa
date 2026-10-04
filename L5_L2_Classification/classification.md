# L5 Narrow / L2 General Classification — K_ALPA
**Platform:** Anticloud | **Tier:** TIER_5_WORLD_NEURO_EMBODIED | **PAX:** 27B
**IP:** USPTO pending 2026, Anticloud FZ LLE, 0-1.gg | **License:** Apache-2.0

## L5 Narrow
K_ALPA specializes in automated pipeline and tensor parallelism for training PAX 27B and larger models. Narrow scope: Anticloud model training infrastructure. Does not attempt general distributed training for arbitrary frameworks.

## L2 General
L2 General: K_ALPA's distributed training capabilities benefit all tiers by enabling more capable base models to be trained on Anticloud hardware clusters.

## PAX 27B Integration
PAX 27B training uses K_ALPA for distributed execution. K_ALPA compiles JAX model code into optimized multi-GPU execution plans, reducing PAX training time.

## AIOSS Audit Chain
Every training checkpoint (step ID + loss hash + model weight hash + GPU topology hash) is chained: H_n = SHA3-256(H_{n-1} || entry_hash_n || timestamp_n).
Offline-verifiable, tamper-evident, zero cloud dependency.

## Regulatory / Compliance
No external regulatory. ISO/IEC 42001 (AI system capability documentation).
