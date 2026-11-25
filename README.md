Software engineer working on distributed systems and infrastructure. [vishalkotak.github.io](https://vishalkotak.github.io)

**Projects**
- **[nvme-kv-cache](https://github.com/vishalkotak/nvme-kv-cache)**: tiered DRAM/NVMe page cache in Rust. The io_uring backend does 3.2× the throughput of blocking I/O at queue depth 32. [Benchmarks](https://github.com/vishalkotak/nvme-kv-cache/blob/main/BENCHMARKS.md)
- **[inference-serving](https://github.com/vishalkotak/inference-serving)**: vLLM and SGLang serving internals rebuilt and compared. Jump-forward decoding cuts a JSON object from 33 forward passes to 4. [Disaggregated prefill/decode](https://github.com/vishalkotak/inference-serving/blob/main/results/d2-disagg-prefill-decode.md)
- **[healthkit-sync](https://github.com/vishalkotak/healthkit-sync)**: Qwen3.5-0.8B fine-tuned with LoRA on a Mac as a private health coach. Quality-check pass rate went from 46% to 93%. [Write-up](https://github.com/vishalkotak/healthkit-sync/blob/main/health-llm/docs/WRITEUP.md)

**Open source**
- Data infra I used in past roles: [deterministic simulation testing](https://github.com/delta-io/delta-rs/pull/5067) for concurrent commits in delta-rs, [GPU decoding of ALP-RD floats](https://github.com/vortex-data/vortex/pull/11707) in Vortex
- RL, alongside my own projects: [safety-gymnasium cost fixes](https://github.com/pytorch/rl/pull/4744) in TorchRL
- Robotics and drones, out of interest in physical AI: [GJK contact fix](https://github.com/google-deepmind/mujoco_warp/pull/1994) in MuJoCo Warp, [rover arming check](https://github.com/PX4/PX4-Autopilot/pull/29899) in PX4, [use-after-free fix](https://github.com/gazebosim/gz-sim/pull/4238) in Gazebo
