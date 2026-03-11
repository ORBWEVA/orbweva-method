# orbweva-method

**The strategic glue. CORE -> ARC -> AER -> Grow.**

A Claude Code skill that connects ORBWEVA's open-source founder toolkit (8 repos, 87 commands) to the ORBWEVA CORE Method -- a structured framework for building, operating, and scaling a business.

## What is CORE?

CORE is a 4-ring strategic framework. Each ring builds on the previous:

| Ring | Name | What it defines |
|------|------|----------------|
| 1 | **Calibrate** | ICP, UVP, Messaging, Pricing |
| 2 | **Operate** | Sales, Marketing, Finance |
| 3 | **Reinforce** | Team, Ops, Product |
| 4 | **Evolve** | Environment, Competition, AI Visibility |

The rings feed three systems:
- **ARC** (Adaptive Resource Center) -- structured knowledge base powering all automation
- **AER** (Acquire, Engage, Retain) -- automation workflows across three pillars
- **Grow** -- client dashboard with business performance, AI decision logs, health scores

## Install

```bash
npx skills add ORBWEVA/orbweva-method
```

## Commands

| Command | Description |
|---------|-------------|
| `/core:assess` | Run a CORE Assessment -- orchestrate skills across all 4 rings to produce a scored Calibration Document |
| `/core:arc` | Convert any skill output into ARC-formatted knowledge entries (COM, SVC, BEN, VOI, TMP, PRC) |
| `/core:aer` | Map skill outputs and agent recipes to AER pillars (Acquire, Engage, Retain) |
| `/core:grow` | Define Grow dashboard metrics and KPIs from startup metrics output |
| `/core:help` | Command reference and recommended flow |

## The Flow

```
              ┌──────────────┐
              │  /core:assess │  ← Start here
              └──────┬───────┘
                     │
        ┌────────────┼────────────┐
        v            v            v
  ┌──────────┐ ┌──────────┐ ┌──────────┐
  │ Ring 1   │ │ Ring 2   │ │ Ring 3-4 │
  │ Calibrate│ │ Operate  │ │ Reinforce│
  │          │ │          │ │ + Evolve │
  └────┬─────┘ └────┬─────┘ └────┬─────┘
       │            │            │
       v            v            v
  ┌──────────┐ ┌──────────┐ ┌──────────┐
  │/core:arc │ │/core:aer │ │/core:grow│
  │ populate │ │ deploy   │ │ measure  │
  └──────────┘ └──────────┘ └──────────┘
```

1. **Assess** -- Run the full CORE Assessment across all 4 rings. Get a score out of 100.
2. **ARC** -- Convert skill outputs into structured knowledge entries. Knowledge before automation.
3. **AER** -- Map automations to Acquire/Engage/Retain pillars. Check deployment readiness.
4. **Grow** -- Define dashboard metrics across 5 layers. Set alert thresholds.

## How It Connects to the Toolkit

This skill orchestrates commands from 8 other ORBWEVA skill repos:

| Repo | Commands | Feeds Ring |
|------|----------|-----------|
| `founder-discovery` | `/discovery:*` (interview, survey, jobs, analyze) | 1 - Calibrate |
| `dt-skill` | `/dt:*` (empathize, define, ideate, prototype, test, audit) | 1 - Calibrate |
| `gtm-skills` | `/gtm:*` + `/geo:*` + `/seo:*` (positioning, channels, pricing, outreach, landing, launch, metrics, growth, score, optimize, audit, page, schema, hreflang) | 1-2 - Calibrate + Operate |
| `founder-metrics` | `/startup:*` (pmf, unit, churn, runway, funnel, growth, moat, ready, glossary) | 2-4 - Operate + Evolve |
| `founder-pitch` | `/pitch:*` (deck, financials, email, objections) | 2 - Operate |
| `founder-ops` | `/legal:*`, `/hire:*`, `/retain:*` | 3 - Reinforce |
| `solo-skills` | `/solo:*` (offer, revenue, audience, content, copy, leads, sales, onboard, clients, support, books, tax, time, stack) | 2-3 - Operate + Reinforce |
| `solo-agents` | `/agent:*` (audit, design, build, leads, support, content, inbox, social, onboard, invoice, research) | 4 - Evolve |

Install them all:

```bash
npx skills add ORBWEVA/founder-discovery
npx skills add ORBWEVA/dt-skill
npx skills add ORBWEVA/gtm-skills
npx skills add ORBWEVA/founder-metrics
npx skills add ORBWEVA/founder-pitch
npx skills add ORBWEVA/founder-ops
npx skills add ORBWEVA/solo-skills
npx skills add ORBWEVA/solo-agents
```

## Part of the ORBWEVA Founder Toolkit

9 repos. 92 commands. One method.

This skill doesn't replace any other skill -- it sequences them and converts their outputs into the CORE framework. Skills are the building blocks. CORE is the blueprint.

## License

MIT
