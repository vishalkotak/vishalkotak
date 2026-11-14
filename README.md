Software engineer working on distributed systems and infrastructure. [vishalkotak.github.io](https://vishalkotak.github.io)

| Project | Description |
|---|---|
| [nvme-kv-cache](https://github.com/vishalkotak/nvme-kv-cache) | Tiered DRAM/NVMe page cache in Rust with io_uring and blocking I/O backends. |
| [inference-serving](https://github.com/vishalkotak/inference-serving) | Reimplementation of vLLM's paged KV cache and PagedAttention, with serving benchmarks. |
| [downstream-detector](https://github.com/vishalkotak/infrastructure/tree/main/downstream-detector) | Runs downstream consumers' test suites against a library PR to catch compatibility breaks. |
| [model-store](https://github.com/vishalkotak/infrastructure/tree/main/model-store) | Model registry and Kubernetes operator for stable and canary rollouts. |
| [healthkit-sync](https://github.com/vishalkotak/healthkit-sync) | iOS app that syncs Apple Health data to Postgres, with a local dashboard. |

**Write-ups**
- [Cache benchmarks](https://github.com/vishalkotak/nvme-kv-cache/blob/main/BENCHMARKS.md): io_uring vs blocking I/O, LRU eviction cost
- [Disaggregated prefill/decode on 2× T4](https://github.com/vishalkotak/inference-serving/blob/main/results/d2-disagg-prefill-decode.md): why the KV handoff failed silently
- [Concurrency load test](https://github.com/vishalkotak/inference-serving/blob/main/results/d1-load-test.md): where batching stops paying off
