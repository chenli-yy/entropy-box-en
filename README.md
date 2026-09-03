# Entropy Box — Embodied-AI Panorama & Knowledge Compiler

> An agent-native knowledge compiler and capability substrate for robotics and embodied-AI development. Turns bounded technical requirements into candidate implementation methods and grounded engineering workflows.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Language](https://img.shields.io/badge/lang-en-green.svg)](SKILL.md)
[![Skill](https://img.shields.io/badge/WorkBuddy-ClawHub-orange.svg)](https://clawhub.ai/)

## What this Skill does

Entropy Box compiles fragmented embodied-AI knowledge — papers, repositories, ROS packages, models, datasets, simulators, benchmarks, standards, and engineering docs — into a persistent, typed, deduplicated, machine-consumable artifact, and serves it through four runtime capabilities:

- **Consult (solution consultation):** decomposes "how should this embodied-AI task be done" into candidate methods, the capabilities, dependencies, assets, constraints, and gaps involved, assembled into a grounded development path.
- **Search (targeted retrieval):** runs RAG retrieval for a concrete question or to understand a selected technology more deeply.
- **Lookup (entity anchoring):** resolves a known ID, name, or alias to a structured topic / capability / asset record.
- **Evidence (verification):** retrieves source-linked comparisons, limitations, engineering notes, and benchmark context.

The public Panorama Graph spans **15 top-level domains, 2,511 vertical topic libraries, 7,000+ task chains, and 60k+ dependency edges**, supporting panorama navigation, capability/dependency analysis, asset selection, and knowledge-gap analysis.

## Install

### Option 1: ClawHub (recommended)

1. Open https://clawhub.ai/ and sign in with your GitHub account.
2. Click "Publish / Import skill", choose this repository `chenli-yy/entropy-box-en`, or search `entropy-box-en` to install in one click.

### Option 2: Manual install

```bash
git clone https://github.com/chenli-yy/entropy-box-en ~/.workbuddy/skills/entropy-box
```

After restarting WorkBuddy or running `/reload-skills`, WorkBuddy loads this skill automatically based on the trigger words in SKILL.md.

## Directory structure

```
entropy-box/
├── SKILL.md                      # skill definition and runtime workflow (core)
├── README.md                     # this file
└── references/
    ├── api.md                    # /api/consult and related endpoint docs
    ├── knowledge-compiler.md     # knowledge-compiler principles
    └── panorama.md               # the 15 top-level domains panorama
```

## When to use

- You need to answer "how should this embodied-AI task be done" and get candidate methods, capabilities, dependencies, assets, constraints, and gaps.
- You are mapping a field, analyzing a capability landscape, decomposing task chains, or assembling a development workflow.
- You already have a technical selection and want to dig deeper with Search / Lookup / Evidence to anchor entities or verify claims.

## Safety & boundaries

- Entropy Box does not itself authorize code deployment, procurement, or physical robot control; physical systems require qualified human review and controlled staged testing.
- Before sending any project context to the public API, strip credentials and sensitive details; proprietary or personal information requires explicit user consent.

## Related links

- Project site: https://xiangshang.ngrok.app/
- Public documentation: https://chenli-yy.github.io/entropy-box-public/
- Integration guide: https://chenli-yy.github.io/entropy-box-public/integrate/
- Live API schema: https://xiangshang.ngrok.app/openapi.json
- Archive & citation: https://doi.org/10.5281/zenodo.21712178

## License

MIT © Yuqi Wang
