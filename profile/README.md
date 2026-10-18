# Delta Observatory

A research application for astronomical observations. People and AI agents do the same work through one API: they select observations, run analyses, compare runs, record judgments, and export evidence.
The first workflow searches TESS light curves for transit signals with box least squares.

![The SKY workspace with WASP-18 b selected](https://raw.githubusercontent.com/delta-observatory/delta-observatory/main/docs/screenshots/sky-wasp-18b.png)

**Start with the [entry repository](https://github.com/delta-observatory/delta-observatory).** It describes the architecture, the access model, and an example investigation, and it restores every component at a tested commit.

| Repository | Content |
|---|---|
| [database](https://github.com/delta-observatory/database) | Schema, migrations, and the cross-component contracts. |
| [workers](https://github.com/delta-observatory/workers) | Ingestion and scientific methods. |
| [backend](https://github.com/delta-observatory/backend) | Stateless FastAPI service: permissions, records, comparisons, and evidence exports. |
| [frontend](https://github.com/delta-observatory/frontend) | React, Three.js, and TypeScript interface. |
| [kubernetes](https://github.com/delta-observatory/kubernetes) | k3s manifests and in-cluster image builds. |
| [agents](https://github.com/delta-observatory/agents) | MCP adapter and agent operating manual. |

The scientific results are development-stage. The application records candidates for review. It does not confirm planets.
