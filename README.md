Software engineer working on distributed systems and infrastructure. [vishalkotak.github.io](https://vishalkotak.github.io)

**Projects**
- **[nvme-kv-cache](https://github.com/vishalkotak/nvme-kv-cache)**: tiered DRAM/NVMe page cache in Rust. The io_uring backend does 3.2× the throughput of blocking I/O at queue depth 32. [Benchmarks](https://github.com/vishalkotak/nvme-kv-cache/blob/main/BENCHMARKS.md)
- **[inference-serving](https://github.com/vishalkotak/inference-serving)**: vLLM and SGLang serving internals rebuilt and compared. Jump-forward decoding cuts a JSON object from 33 forward passes to 4. [Disaggregated prefill/decode](https://github.com/vishalkotak/inference-serving/blob/main/results/d2-disagg-prefill-decode.md)
- **[healthkit-sync](https://github.com/vishalkotak/healthkit-sync)**: Qwen3.5-0.8B fine-tuned with LoRA on a Mac as a private health coach. Quality-check pass rate went from 46% to 93%. [Write-up](https://github.com/vishalkotak/healthkit-sync/blob/main/health-llm/docs/WRITEUP.md)

**Open source**

Data infra I used in past roles:
- **delta-rs**: [added deterministic simulation testing](https://github.com/delta-io/delta-rs/pull/5067) for concurrent commits. Any writer interleaving replays from a seed, it catches three known commit bugs, and it runs in CI in about a second.
- **Vortex**: [added GPU decoding for ALP-RD floats](https://github.com/vortex-data/vortex/pull/11707), so full-precision floats no longer fall back to the CPU on the CUDA path.

RL, alongside my own projects:
- **TorchRL**: [fixed safety costs being undercounted](https://github.com/pytorch/rl/pull/4744) with frame skipping, which kept only the last frame's cost.

Robotics and drones, out of interest in physical AI:
- **MuJoCo Warp**: [fixed GJK dropping contacts](https://github.com/google-deepmind/mujoco_warp/pull/1994) when geoms share a center, matching MuJoCo C.
- **PX4**: [stopped rovers arming with the drive stick pushed](https://github.com/PX4/PX4-Autopilot/pull/29899) when sticks are remapped.
- **Gazebo**: [fixed a use-after-free](https://github.com/gazebosim/gz-sim/pull/4238) behind a recurring CI crash.
