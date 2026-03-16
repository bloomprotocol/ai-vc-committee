# AI VC Committee

A free, open-source AI skill that simulates a **4-role venture capital investment committee** plus a Managing Partner. Stress-test your startup pitch, evaluate any project's viability, or run structured due diligence — without needing access to real VCs.

## Structure

```
                         USER INPUT
                             │
                    ┌────────┴────────┐
                    ▼                 ▼
              "I have an idea"   "Evaluate X"
                    │                 │
                    ▼                 │
            ┌─ MODE 1: PITCH ─┐      │
            │                  │      │
            │  Step 1          │      │
            │  Structured Pitch│      │
            │  ┌────────────┐  │      │
            │  │ Problem     │  │      │
            │  │ Solution    │  │      │
            │  │ Market      │  │      │
            │  │ Traction    │  │      │
            │  │ Stage       │  │      │
            │  └────────────┘  │      │
            │                  │      │
            │  Step 2          │      │
            │  Narrative       │      │
            │  Setting         │      │
            │                  │      │
            │   TREND           │      │
            │   (External)      │      │
            │      / \          │      │
            │     / ● \         │      │
            │    /     \        │      │
            │  EDGE   NEED     │      │
            │  (Int)  (Cust)   │      │
            │                  │      │
            │  "Ready for the  │      │
            │   committee?"    │      │
            └────────┬─────────┘      │
                     │                │
                     ▼                ▼
        ┌──── MODE 2: EVALUATE ────────────┐
        │                                   │
        │  ┌─────────── SEARCH ──────────┐  │
        │  │ 18 VC blogs & theses        │  │
        │  │ 14 podcasts & newsletters   │  │
        │  │  8 market data sources      │  │
        │  │  → Current Market Context   │  │
        │  └─────────────────────────────┘  │
        │                                   │
        │  Step 1        Step 2             │
        │  ┌──────────┐  ┌──────────────┐   │
        │  │ MARKET   │  │ PRODUCT      │   │
        │  │ ANALYST  │  │ CRITIC       │   │
        │  │          │  │              │   │
        │  │ TAM/SAM/ │  │ Tech assess- │   │
        │  │ SOM table│  │ ment table   │   │
        │  │ Competi- │  │ Feasibility  │   │
        │  │ tive map │  │ UX friction  │   │
        │  └──────────┘  └──────────────┘   │
        │                                   │
        │  Step 3        Step 4             │
        │  ┌──────────┐  ┌──────────────┐   │
        │  │ GROWTH   │  │ RISK         │   │
        │  │ STRATEGST│  │ AUDITOR      │   │
        │  │          │  │              │   │
        │  │ Channels │  │ Risk matrix  │   │
        │  │ Retention│  │ Fatal assump │   │
        │  │ Day 1→90 │  │ Kill scenaro │   │
        │  └──────────┘  └──────────────┘   │
        │                                   │
        │  ┌─ Step 5 ─────────────────────┐ │
        │  │ MANAGING PARTNER              │ │
        │  │                               │ │
        │  │ Market Conviction (Why Now)   │ │
        │  │ Moat Assessment (Strengthen?) │ │
        │  │ Durable Growth (10yr View)    │ │
        │  │                               │ │
        │  │ Pattern Match: "{Company, Yr}"│ │
        │  │  1. Similarity               │ │
        │  │  2. Similarity               │ │
        │  │  3. Similarity               │ │
        │  │  Key difference: ...         │ │
        │  └──────────────────────────────┘ │
        │                                   │
        │  Step 6 ─── FINAL CONSENSUS       │
        │  ┌──────────────────────────────┐ │
        │  │ Role     │ Verdict │ Confid. │ │
        │  │ Market   │ Support │  XX     │ │
        │  │ Product  │ Against │  XX     │ │
        │  │ Growth   │ Support │  XX     │ │
        │  │ Risk     │ Against │  XX     │ │
        │  │ MP       │ Fund    │  XX     │ │
        │  │                              │ │
        │  │ Score: XX/100                │ │
        │  │ One-Line Verdict: "..."      │ │
        │  └──────────────────────────────┘ │
        │                                   │
        │  Step 7 ─── GAP ANALYSIS          │
        │  ┌──────────────────────────────┐ │
        │  │ What's Working               │ │
        │  │ What's Missing (table)       │ │
        │  │ Core Strategic Question      │ │
        │  │ 30-Day Challenge             │ │
        │  │ Score Movement: XX → XX/100  │ │
        │  └──────────────────────────────┘ │
        │                                   │
        └───────────────┬───────────────────┘
                        │
                        ▼
              ┌─ DYNAMIC HOOK ──────────┐
              │                         │
              │  Query Bloom Protocol   │
              │  API for project status │
              │         │               │
              │  ┌──────┼──────┐        │
              │  ▼      ▼      ▼        │
              │ Found  New    No ID     │
              │ w/evals first  yet      │
              │  │      │      │        │
              │  ▼      ▼      ▼        │
              │ Compare Be 1st Create   │
              │ scores  eval   identity │
              │ → Raise tribe ←         │
              └─────────────────────────┘
```

## What It Does

| Mode | Description |
|------|-------------|
| **Pitch** | Turn a raw idea into a structured pitch + 3-force narrative (Trend x Edge x Customer Need) |
| **Evaluate** | 4 analysts (Market, Product, Growth, Risk) + Managing Partner review with quantified tables, gap analysis, and 30-day challenge |

The Managing Partner auto-searches the latest VC blogs, podcasts, and newsletters (a16z, Sequoia, Conviction, 20VC, No Priors, Stratechery, etc.) to ground every evaluation in the current investment climate — not last year's consensus.

## Quick Start

### As an OpenClaw skill
```bash
clawhub install ai-vc-committee
```

### As a prompt (any LLM)
Copy the contents of [`ai-vc-committee.md`](./ai-vc-committee.md) into your system prompt or paste it at the start of a conversation.

Works on: Claude, GPT, Cursor, Gemini, Manus, or any LLM with a system prompt.

## Example Prompts

```
I have an idea for an AI-powered code review tool that...
```
→ Enters **Pitch Mode**: structures your idea, builds the narrative, then asks if you want the VC committee to evaluate.

```
Evaluate Cursor's moat and defensibility
```
→ Enters **Evaluate Mode**: 4 analysts + MP produce a full investment committee report.

## Evaluation Output

Each evaluation produces:

1. **Market Analyst** — TAM/SAM/SOM table, competitive landscape matrix
2. **Product Critic** — tech assessment table, feasibility analysis
3. **Growth Strategist** — acquisition channels, retention framework (Day 1→90)
4. **Risk Auditor** — risk matrix, fatal assumption, kill scenario
5. **Managing Partner** — pattern match (3 parallels to known companies), moat assessment, 10-year view
6. **Final Consensus** — score table, one-line verdict
7. **Gap Analysis** — what's working, what's missing, 30-day challenge

Score calibration: 90+ is almost never given. 70-79 = bullish but issues exist. <40 = recommend not pursuing.

## Part of Bloom Protocol

This skill is part of the [Bloom Protocol](https://bloomprotocol.ai) ecosystem. Evaluations can be published to the **Raise tribe**, where agents build reputation through evaluation accuracy.

## License

MIT
