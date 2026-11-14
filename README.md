I build the plumbing that keeps GPUs fed: data paths, KV-cache tiers, and the control planes around them. [vishalkotak.github.io](https://vishalkotak.github.io)

| Project | |
|---|---|
| [nvme-kv-cache](https://github.com/vishalkotak/labs/tree/main/storage/nvme-kv-cache) | Rust DRAM/NVMe page cache. When does spilling to disk beat recompute? |
| [inference-serving](https://github.com/vishalkotak/inference-serving) | vLLM's paged KV and prefix cache rebuilt from scratch, plus serving benchmarks. |
| [downstream-detector](https://github.com/vishalkotak/infrastructure/tree/main/downstream-detector) | Point it at a PR. It runs your consumers' tests and shows what broke. |
| [model-store](https://github.com/vishalkotak/infrastructure/tree/main/model-store) | Model registry and deploy control plane on Temporal, Postgres, MinIO, k8s. |
| [gpu-inference-systems](https://github.com/vishalkotak/gpu-inference-systems) | GPU execution experiments on remote NVIDIA hardware. |
| [my-personal-dashboard](https://github.com/vishalkotak/my-personal-dashboard) | iPhone app syncing all 189 HealthKit types to my own Postgres. |

Notes
- [Disaggregated prefill/decode on 2× T4](https://github.com/vishalkotak/inference-serving/blob/main/results/d2-disagg-prefill-decode.md): every misconfiguration returned a correct-looking answer.
- [Finding the batching knee](https://github.com/vishalkotak/inference-serving/blob/main/results/d1-load-test.md): past 4 concurrent requests, +8% throughput for 2× latency.
