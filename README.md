# Duck Robot Stack

This repository groups the two official Pollen Robotics MicroDuck projects used for simulation training:

- [`microduck/`](microduck/) - MicroDuck runtime, robot control and deployment code.
- [`microduck_rl/`](microduck_rl/) - MuJoCo Warp / `mjlab` reinforcement-learning environments and policy export tools.

The main training task is `Mjlab-Velocity-Flat-MicroDuck`. It uses 61 actor observations, 14 joint-position actions, PPO, BAM actuator modeling, and domain randomization for sim-to-real transfer.

The training environment is intentionally not committed. Create it with the instructions in [`microduck_rl/README.md`](microduck_rl/README.md), then keep checkpoints and logs outside Git.
