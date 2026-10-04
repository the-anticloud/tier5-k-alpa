# Radon_Complexity_Lab_Results
**Project:** `K_ALPA` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'A', 'score': 3.1883289124668437}`
- **complexity_grade:** `A`
- **complexity_score:** `3.1883289124668437`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_ALPA\UPSTREAM\setup.py - A (48.63)
E:\fenta\Downloads\The`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_ALPA\UPSTREAM\setup.py
    F 34:0 locate_cuda - C (11)
    F 15:0 get_cuda_version - A (3)
    C 125:4 InstallPlatlib - A (3)
    F 76:0 get_cuda_version_str - A (2)
    F 107:0 get_alpa_version - A (2)
    C 120:4 BinaryDistribution - A (2)
    M 127:8 InstallPlatlib.finalize_options - A (2)
    M 122:8 BinaryDistribution.has_ext_modules - A (1)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_ALPA\UPSTREAM\update_version.py
    F 139:0 update - B (9)
    F 55:0 git_describe_version - B (7)
    F 177:0 main - A (3)
    F 51:0 py_str - A (1)
    F 166:0 sync_version - A (1)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_ALPA\UPSTREAM\alpa\api.py
    M 149:4 ParallelizedFunc._decode_args_and_get_executable - B (10)
    F 209:0 _compile_parallel_executable - A (5)
    C 106:0 ParallelizedFunc - A (3)
    F 25:0 init - A (2)
    F 63:0 shutdown - A (2)
    F 71:0 parallelize - A (2)
    F 236:0 clear_executable_cache - A (1)
    F 241:0 grad - A (1)
    F 265:0 value_and_grad - A (1)
    M 109:4 ParallelizedFunc.__init__ - A (1)
    M 126:4 ParallelizedFunc.__call__ - A (1)
    M 133:4 ParallelizedFunc.get_executable - A (1)
    M 138:4 ParallelizedFunc.preshard_dynamic_args - A (1)
    M 145:4 ParallelizedFunc.get_last_executable - A (1)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_ALPA\UPSTREAM\alpa\create_state_parallel.py
    F 151:0 propagate_mesh_assignment - C (1
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_