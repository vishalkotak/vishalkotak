I build the plumbing that keeps GPUs fed: data paths, KV-cache tiers, and the control planes around them. [vishalkotak.github.io](https://vishalkotak.github.io)

| Project | |
|---|---|
| [nvme-kv-cache](https://github.com/vishalkotak/nvme-kv-cache) | Rust DRAM/NVMe page cache. When does spilling to disk beat recompute? |
| [inference-serving](https://github.com/vishalkotak/inference-serving) | vLLM internals from scratch, CUDA execution experiments, serving benchmarks. |
| [downstream-detector](https://github.com/vishalkotak/infrastructure/tree/main/downstream-detector) | Point it at a PR. It runs your consumers' tests and shows what broke. |
| [model-store](https://github.com/vishalkotak/infrastructure/tree/main/model-store) | Model registry and deploy control plane on Temporal, Postgres, MinIO, k8s. |
| [healthkit-sync](https://github.com/vishalkotak/healthkit-sync) | iPhone app syncing all 189 HealthKit types to my own Postgres. |
| [triage-agent](https://github.com/vishalkotak/triage-agent) | Incident-triage LLM agent with a schema-validated tool registry. |

Notes
- [Disaggregated prefill/decode on 2× T4](https://github.com/vishalkotak/inference-serving/blob/main/results/d2-disagg-prefill-decode.md): every misconfiguration returned a correct-looking answer.
- [Finding the batching knee](https://github.com/vishalkotak/inference-serving/blob/main/results/d1-load-test.md): past 4 concurrent requests, +8% throughput for 2× latency.
