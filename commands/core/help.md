---
name: help
description: Show all CORE Method commands and the recommended execution flow.
---

# CORE Method Commands

| Command | Description |
|---------|-------------|
| `/core:assess` | Run a CORE Assessment — orchestrate skills across all 4 rings to produce a scored Calibration Document |
| `/core:arc` | Convert any skill output into ARC-formatted knowledge entries (COM, SVC, BEN, VOI, TMP, PRC) |
| `/core:aer` | Map skill outputs and agent recipes to AER pillars (Acquire, Engage, Retain) |
| `/core:grow` | Define Grow dashboard metrics and KPIs from startup metrics output |
| `/core:help` | This command reference |

## Recommended Flow

```
1. /core:assess  → Run the full CORE Assessment
2. /core:arc     → Convert outputs into ARC entries
3. /core:aer     → Map automations to AER pillars
4. /core:grow    → Define dashboard metrics
```

Each stage builds on the previous. The assessment identifies what you have and what's missing. ARC captures it as structured knowledge. AER maps it to automation. Grow measures the results.

## Prerequisites

This skill orchestrates commands from 8 other ORBWEVA skill repos. Install them first:

```
npx skills add ORBWEVA/founder-discovery
npx skills add ORBWEVA/dt-skill
npx skills add ORBWEVA/gtm-skills
npx skills add ORBWEVA/founder-metrics
npx skills add ORBWEVA/founder-pitch
npx skills add ORBWEVA/founder-ops
npx skills add ORBWEVA/solo-skills
npx skills add ORBWEVA/solo-agents
```
