<p align="center">
  <img src="figure/banner.png" alt="Mi-Memory Banner" width="100%">
</p>

<h1 align="center">Mi-Memory</h1>

<p align="center">
  <strong>A Lifecycle Memory Framework for Personal AI</strong>
</p>

<p align="center">
  <a href="https://darwin-agent.github.io/Mi-Memory/"><img src="https://img.shields.io/badge/Homepage-Visit-ff6900?style=flat" alt="Homepage"></a>
  <a href="paper.pdf"><img src="https://img.shields.io/badge/Paper-PDF-red?style=flat" alt="Paper PDF"></a>
  <img src="https://img.shields.io/badge/Pages-53-blue?style=flat" alt="Pages">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-22c55e?style=flat" alt="License: MIT"></a>
  <img src="https://img.shields.io/badge/Status-Technical_Report-a855f7?style=flat" alt="Status">
</p>

<p align="center">
  <a href="https://darwin-agent.github.io/Mi-Memory/">Homepage</a> •
  <a href="#-overview">Overview</a> •
  <a href="#-architecture">Architecture</a> •
  <a href="#-highlights">Highlights</a> •
  <a href="#-results">Results</a> •
  <a href="#-citation">Citation</a>
</p>

---

## 📢 News

- **2026-07** — Technical report released: [**Mi-Memory: A Lifecycle Memory Framework for Personal AI**](paper.pdf).
- **2026-07** — Repository is live as a project introduction page with the report PDF and overview figures.

## 🧭 Overview

Project homepage: **https://darwin-agent.github.io/Mi-Memory/**

Personal AI is moving beyond chat-only interaction toward continuous services across phones, cars, homes, wearables, cameras, and tools. In this setting, memory cannot remain a cache of prior conversations: it must preserve durable user state, connect answers to multimodal and device evidence, support correction and forgetting, bound policy evolution, and remain deployable across edge/cloud constraints.

**Mi-Memory** is a lifecycle memory framework organized around four roles:

- **Structure** — memory runtime, storage hierarchy, retrieval, filtering, and context assembly.
- **Expansion** — multimodal and cross-device evidence acquisition.
- **Evolution** — diagnostic iteration, governed strategy updates, and rollback.
- **Deployment** — substrate-independent memory variants for constrained environments.

## 📐 Architecture

<p align="center">
  <img src="figure/mimemory.png" alt="Mi-Memory lifecycle overview" width="85%">
</p>

Mi-Memory links the lifecycle through a shared audit contract: typed evidence payloads preserve source identity and provenance, diagnostic traces localize evidence loss, strategy artifacts make memory-policy changes explicit, and gate/rollback records bound accepted evolution.

## ✨ Highlights

| | |
|---|---|
| 🧱 **Composable memory structure** | Multi-granularity storage with stage-level diagnostic traces. |
| 🌐 **Multi-source evidence** | Dialogue, multimodal perception, cross-device events, and causal fusion. |
| 🔄 **Governed evolution** | D²ACCI human-in-the-loop iteration and EMEND/AEGIS-style bounded strategy evolution. |
| 📦 **Deployment flexibility** | Full-stack cloud reference and repository-native lightweight memory variant. |
| 📊 **Comprehensive evaluation** | Structure benchmarks plus module-level, transfer-feasibility, and design-level evidence. |

## 📊 Results

| Benchmark | Track | Metric | Score |
|:----------|:------|:-------|------:|
| **LoCoMo** | Structure | Judge Accuracy | **93.59%** |
| **PersonaMem-V2** | Structure | Preference Accuracy | **57.24%** |
| **LongMemEval** | Structure | Judge Accuracy | **87.47%** |
| **Mem-Gallery** | Expansion | Judge Accuracy (3-vote) | **89.15%** |
| **MemFuseBench** | Expansion | Checklist Score | **33.1%** |
| **Light-Memory / LoCoMo** | Deployment | Capability Retention | **97.0%** |

See [`paper.pdf`](paper.pdf) for the full technical report, evaluation protocol, evidence boundaries, and detailed analysis.

## 📁 Repository Contents

```text
.
├── index.html             # GitHub Pages project homepage
├── paper.pdf              # Released technical report
├── figure/                # README-facing visual assets
├── LICENSE
└── README.md
```

> This repository is an introduction page for the Mi-Memory technical report. It does not include implementation source code.

## 📖 Citation

If you find this work useful, please cite:

```bibtex
@techreport{mimemory2026,
  title       = {Mi-Memory: A Lifecycle Memory Framework for Personal AI},
  author      = {Darwin Agent Team},
  institution = {Xiaomi},
  year        = {2026},
  url         = {https://github.com/Darwin-Agent/Mi-Memory}
}
```

## License

This project is licensed under the [MIT License](LICENSE).
