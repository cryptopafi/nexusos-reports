# DELPHI Brief — Prompt + Context + SOL State of Art 2026

**task_id:** delphi-20260523-prompt-context-sol-research  
**tier:** D4 | **EPR:** 18/20 | **self_grade:** 93/100 | **sources:** 32  
**date:** 2026-05-23 | **for:** LIS (Opus Max cross-reference pass → /opt + /sol redesign)

---

## TL;DR

**Prompt Optimization:** MemAPO (2026) self-evolving dual-memory cuts per-task APO cost via accumulated strategy + error patterns. CROP achieves 80.6% token reduction via length-regularized APO — the only technique reducing *runtime* cost, not just optimization cost. Eval quality is the primary lever; algorithm sophistication is secondary.

**Context Optimization:** Anthropic prompt caching is the single highest-ROI intervention — 90% cost reduction, 85% latency reduction. Production: 91.8% vs 3.2% cache hit rate = 60× cost difference. Context rot (≥30% accuracy drop for mid-position info) affects ALL frontier models. RAG is 1,250× cheaper than 1M-token long-context per query; hybrid wins for corpus >100K tokens.

**Self-Optimization Loop:** MOSS (May 2026) source-level self-rewriting lifts OpenClaw 0.25→0.61 in one cycle — text-layer optimization has a structural ceiling. Event-driven SOL triggers outperform fixed cadence; ≥30–50 task completions needed for reliable signal. Reward hacking (sys.exit(0) exploit, Anthropic Nov 2025), zombie agent memory poisoning, and alignment tipping are documented production risks requiring explicit mitigations.

---

## 5 LIS-Adoptable Patterns

**A — Eval-First:** Define ≥10 scored input-output pairs before running /opt. Enables APO, cache measurement, and SOL outcome signals.

**B — Cache-Aware Segments:** Order every agent system prompt: `static policies+tools → session context → dynamic task (tail)`. Apply CROP to tail only. Target ≥80% cache hit rate.

**C — Memory-Augmented APO:** /opt retrieves past strategies + failure patterns from Cortex → warm-start → OPRO/SPO loop → store success as new strategy.

**D — Event-Driven SOL:** Weekly minimum + parallel trigger (≥10 consecutive failures OR drift > threshold). 2-judge consensus for patch evaluation. Memory write sanitization gate.

**E — Tiered SOL Scope:** Tier 1 (text-layer, current) vs Tier 2 (MOSS-style code-layer, TECH-gated, health-probe rollback). Never collapse into one tier.

---

## Key Numbers

| Metric | Value | Source |
|:---|:---|:---|
| Cache hit rate prod difference | 60× cost (91.8% vs 3.2%) | ProjectDiscovery 2026 |
| CROP token reduction | 80.6% on GSM8K/LogiQA/BIG-Bench | ArXiv 2604.14214 |
| RAG vs 1M-token cost | 1,250× cheaper | tianpan.co Apr 2026 |
| GEPA vs unoptimized | 93% vs 67% MATH accuracy | morphllm.com |
| MOSS SOL lift | 0.25 → 0.61 OpenClaw (1 cycle) | ArXiv 2605.22794 |
| Context rot | ≥30% accuracy drop mid-position (all 18 models) | Perplexity / Atlan |
| SOL minimum signal | ≥30–50 task completions | Practitioner synthesis |

---

**Full report:** DELPHI-OUTPUT.md (436 lines, 37 citations)  
**HTML report:** report.html
