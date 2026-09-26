# GPU visualizers

Small interactive tools that explain how GPU infrastructure actually behaves. Companion to the **#ZeroToGPU** and **#GPUtoPlatform** series on LinkedIn.

**Live:** https://<your-username>.github.io/gpu-visualizers/

## Tools

| Tool | What it shows | Link |
|------|---------------|------|
| [Four ways to share one GPU](multi-tenancy/) | Whole card vs time-slicing vs MPS vs MIG: utilization, stranded capacity, queued tenants, and memory / performance / fault isolation | `/multi-tenancy/` |

More coming: utilization and own-vs-rent economics, topology-aware placement, tail latency, KV-cache memory pressure.

## Notes

Simplified teaching models, not benchmarks. MIG shapes follow NVIDIA's publicly documented profiles for an 80 GB-class GPU (1g.10gb to 7g.80gb). Time-slicing and MPS behaviour is approximated from public documentation.

Each tool is a single self-contained HTML file in its own folder. No build step.

## Adding a tool

1. Create a folder, e.g. `utilization-calculator/`
2. Put the tool in it as `index.html`
3. Add a card to the root `index.html` and a row to the table above

Built by Meet Andani.
