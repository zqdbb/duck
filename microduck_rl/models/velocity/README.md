# MicroDuck flat-velocity backlash policy

Final artifacts from the September 30, 2026 continuation run of
`Mjlab-Velocity-Flat-Backlash-MicroDuck`.

## Files

- `microduck_velocity_flat_backlash_2026-09-30.onnx` — deployment policy,
  validated with input `obs [1, 61]` and output `actions [1, 14]`.
- `microduck_velocity_flat_backlash_2026-09-30.pt` — RSL-RL checkpoint for
  evaluation or further training.

## Training result

- Final iteration: `24999/25000`
- Total simulation steps in this continuation: `614,400,000`
- Mean reward: `114.37`
- Mean episode length: `955.90`
- Mean action standard deviation: `0.19`
- Linear velocity error: `0.3554`
- Yaw velocity error: `1.0846`
- Fell-over metric: `0.1250`
- NaN termination metric: `0.0000`

The run warm-started from the previous backlash-aware checkpoint
`model_24999.pt` produced on September 29, 2026. It used 1,024 parallel
environments and the project's standard PPO configuration. Intermediate
checkpoints and logs are not stored in Git.

## SHA-256

```text
6bab54836fb8522b5348b29b2c3938cb5eecaa5b5d94739c5ad37422e34c79bc  microduck_velocity_flat_backlash_2026-09-30.onnx
9a6bb02d884e67d379b8a2a4b827d13ba19a32ef1ac238eb633198fe93ede09e  microduck_velocity_flat_backlash_2026-09-30.pt
```

