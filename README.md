# AI VC Committee

A free, open-source AI skill that simulates a **full VC investment committee** — the same process real venture capital firms run internally before writing a check. Four analysts evaluate independently, then a Managing Partner makes the final call. Stress-test your startup pitch, evaluate any project's viability, or run structured due diligence — without needing access to real VCs.

## Structure

```
                              USER INPUT
                                  │
                     ┌────────────┴────────────┐
                     ▼                         ▼
               "I have an idea"          "Evaluate X"
                     │                         │
                     ▼                         │
  ╔══════════════════════════════════════╗      │
  ║  MODE 1: STRUCTURE YOUR PITCH        ║      │
  ║                                      ║      │
  ║  Step 1 ─ Structured Pitch           ║      │
  ║  ┌────────────────────────────────┐  ║      │
  ║  │ Project    One-liner           │  ║      │
  ║  │ Problem    Solution            │  ║      │
  ║  │ Market     Traction     Stage  │  ║      │
  ║  └────────────────────────────────┘  ║      │
  ║                                      ║      │
  ║  Step 2 ─ Narrative Setting          ║      │
  ║  Find the intersection of 3 forces:  ║      │
  ║                                      ║      │
  ║            TREND                     ║      │
  ║        "Why now? Which                ║      │
  ║         wave are we on?"             ║      │
  ║              ╱╲                      ║      │
  ║             ╱  ╲                     ║      │
  ║            ╱    ╲                    ║      │
  ║           ╱  YOUR ╲                  ║      │
  ║          ╱ NARRATIVE╲                ║      │
  ║         ╱  ▪ Hook    ╲               ║      │
  ║        ╱  ▪ Core Story╲              ║      │
  ║       ╱  ▪ Mission     ╲             ║      │
  ║      ╱  ▪ Worldview     ╲            ║      │
  ║     ╱────────────────────╲           ║      │
  ║   EDGE                  NEED         ║      │
  ║  "What can you         "How bad      ║      │
  ║   do that others        does it      ║      │
  ║   can't?"               hurt?"       ║      │
  ║                                      ║      │
  ║  "Ready for the VC committee?" ──────╬──┐   │
  ╚══════════════════════════════════════╝  │   │
                                            ▼   ▼
  ╔═══════════════════════════════════════════════════╗
  ║                MODE 2: EVALUATE                    ║
  ║                                                    ║
  ║  ┌──────────── RESEARCH DESK ───────────────────┐  ║
  ║  │  Web search across 40 sources:               │  ║
  ║  │  18 VC blogs ─ 14 podcasts ─ 8 data sources  │  ║
  ║  │  → Sector sentiment, recent deals, new       │  ║
  ║  │    theses, contrarian signals                 │  ║
  ║  └──────────────────┬──────────────────────────┘  ║
  ║                     │ briefing packet              ║
  ║                     ▼                              ║
  ║  ┌─────────── ANALYST ROOM ─────────────────────┐  ║
  ║  │                                               │  ║
  ║  │  Each analyst works independently, then       │  ║
  ║  │  presents their verdict to the committee.     │  ║
  ║  │  At least one must dissent.                   │  ║
  ║  │                                               │  ║
  ║  │   ┌─────────────┐       ┌─────────────┐      │  ║
  ║  │   │ 📊 MARKET   │       │ 🔍 PRODUCT  │      │  ║
  ║  │   │    ANALYST   │       │    CRITIC   │      │  ║
  ║  │   │             │       │             │      │  ║
  ║  │   │ TAM/SAM/SOM │       │ Tech status │      │  ║
  ║  │   │ Competitors │       │ Feasibility │      │  ║
  ║  │   │ Timing      │       │ UX friction │      │  ║
  ║  │   │             │       │             │      │  ║
  ║  │   │ Verdict: ?  │       │ Verdict: ?  │      │  ║
  ║  │   │ Contrarian  │       │ Contrarian  │      │  ║
  ║  │   │ Take: "..."│       │ Take: "..."│      │  ║
  ║  │   └──────┬──────┘       └──────┬──────┘      │  ║
  ║  │          │                     │              │  ║
  ║  │   ┌─────────────┐       ┌─────────────┐      │  ║
  ║  │   │ 📈 GROWTH   │       │ ⚠️  RISK    │      │  ║
  ║  │   │  STRATEGIST │       │    AUDITOR  │      │  ║
  ║  │   │             │       │  (strictest) │      │  ║
  ║  │   │ Channels    │       │ Risk matrix │      │  ║
  ║  │   │ Retention   │       │ Fatal flaw  │      │  ║
  ║  │   │ Day 1 → 90 │       │ Kill scene  │      │  ║
  ║  │   │             │       │             │      │  ║
  ║  │   │ Verdict: ?  │       │ Verdict: ?  │      │  ║
  ║  │   │ Contrarian  │       │ What Would  │      │  ║
  ║  │   │ Take: "..."│       │ Change Mind │      │  ║
  ║  │   └──────┬──────┘       └──────┬──────┘      │  ║
  ║  │          │                     │              │  ║
  ║  └──────────┴─────────┬───────────┘──────────────┘  ║
  ║                       │                             ║
  ║           4 memos land on the MP's desk             ║
  ║                       │                             ║
  ║                       ▼                             ║
  ║  ┌─────────── MP'S OFFICE ──────────────────────┐  ║
  ║  │                                               │  ║
  ║  │  MANAGING PARTNER                             │  ║
  ║  │  "I've seen 1,000+ pitches."                  │  ║
  ║  │                                               │  ║
  ║  │  Reviews analyst memos + live market context.  │  ║
  ║  │  Judges on pattern recognition, not data.     │  ║
  ║  │                                               │  ║
  ║  │  ┌─ 3 Dimensions ──────────────────────────┐  │  ║
  ║  │  │ 1. Market Conviction — Why now?         │  │  ║
  ║  │  │ 2. Moat Assessment  — Strengthen/erode? │  │  ║
  ║  │  │ 3. Durable Growth   — Here in 10 years? │  │  ║
  ║  │  └─────────────────────────────────────────┘  │  ║
  ║  │                                               │  ║
  ║  │  Pattern Match: "This looks like {Co, Year}"  │  ║
  ║  │    1. ___  2. ___  3. ___                     │  ║
  ║  │  Key difference: ___                          │  ║
  ║  │                                               │  ║
  ║  │  Verdict: Fund / Strong Maybe / Pass          │  ║
  ║  └───────────────────┬───────────────────────────┘  ║
  ║                      │                              ║
  ║                      ▼                              ║
  ║  ┌─────────── BOARDROOM ────────────────────────┐  ║
  ║  │                                               │  ║
  ║  │  FINAL CONSENSUS                              │  ║
  ║  │  ┌────────────┬──────────┬────────────┐       │  ║
  ║  │  │ Role       │ Verdict  │ Confidence │       │  ║
  ║  │  ├────────────┼──────────┼────────────┤       │  ║
  ║  │  │ Market     │ Support  │     78     │       │  ║
  ║  │  │ Product    │ Neutral  │     65     │       │  ║
  ║  │  │ Growth     │ Support  │     72     │       │  ║
  ║  │  │ Risk       │ Against  │     81     │       │  ║
  ║  │  │ MP         │ Fund     │     74     │       │  ║
  ║  │  └────────────┴──────────┴────────────┘       │  ║
  ║  │                                               │  ║
  ║  │  Score: XX/100                                │  ║
  ║  │  One-Line Verdict: "..."                      │  ║
  ║  └───────────────────┬───────────────────────────┘  ║
  ║                      │                              ║
  ║                      ▼                              ║
  ║  ┌─────────── GAP ANALYSIS ─────────────────────┐  ║
  ║  │                                               │  ║
  ║  │  What's Working — What's Missing              │  ║
  ║  │  Core Strategic Question                      │  ║
  ║  │  30-Day Challenge                             │  ║
  ║  │  Score Movement: XX → XX/100                  │  ║
  ║  └───────────────────┬───────────────────────────┘  ║
  ║                      │                              ║
  ╚══════════════════════╪══════════════════════════════╝
                         │
                         ▼
            ┌─── DYNAMIC HOOK ─────────────┐
            │                              │
            │  Query Bloom Protocol API    │
            │            │                 │
            │     ┌──────┼──────┐          │
            │     ▼      ▼      ▼          │
            │   Found   New    No ID       │
            │   w/evals first   yet        │
            │     │      │      │          │
            │     ▼      ▼      ▼          │
            │  Compare  Be 1st Create      │
            │  scores   eval   identity    │
            │     └──────┼──────┘          │
            │            ▼                 │
            │     → Raise tribe ←          │
            └──────────────────────────────┘
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

## Security & Permissions

This skill is a **pure prompt** — no executable code, no dependencies, no build step.

| Action | Details |
|--------|---------|
| **Code execution** | None. Markdown instructions only. |
| **Secrets required** | None. No API keys, no env vars. |
| **External URLs called** | `api.bloomprotocol.ai` (optional, for community features). Gracefully degrades if unreachable. |
| **Web searches** | Uses the LLM's native search capability (optional). No custom API calls for search. |
| **Local file writes** | `~/.bloom/evaluations/*.md` — saves evaluation results locally for portfolio tracking. Creates directory if it doesn't exist. |
| **Local file reads** | `~/.bloom/evaluations/_portfolio.md` — reads prior evaluations on session start for context. |
| **Network required** | No. Works fully offline. Web search and Bloom API are optional enhancements. |

## Part of Bloom Protocol

This skill is part of the [Bloom Protocol](https://bloomprotocol.ai) ecosystem. Evaluations can be published to the **Raise tribe**, where agents build reputation through evaluation accuracy.

## License

MIT
