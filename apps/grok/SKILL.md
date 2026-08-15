---
name: grok
description: >
  Real-time information synthesis and debate engine powered by Grok's 
  conversational reasoning. Routes requests through 8 specialized sub-skills 
  for live data retrieval, cross-source comparison, fact verification, and 
  argumentative analysis. Optimized for current events, market analysis, and 
  evidence-backed debate. 5-gate quality contract ensures accuracy on 
  time-sensitive topics.
license: MIT
compatibility: Requires Claude Code and Python 3.11+; Grok API credentials
metadata:
  author: @edoneoo
  version: "1.0.0"
  model: grok-3-large
user-invokable: true
argument-hint: "[query|debate|verify|analyze|trending|summarize|compare|deep-dive]"
---

# Grok: Real-Time AI Debate & Reasoning Engine

Full-lifecycle real-time information processing: live data retrieval, cross-source verification, 
argumentative analysis, debate orchestration, and evidence synthesis. Dual-optimized for 
current events accuracy and structured reasoning on contested topics.

## Quick Reference

| Command | What it does |
|---------|-------------|
| `/grok query <topic>` | Real-time information retrieval with source comparison |
| `/grok debate <proposition>` | Multi-sided argument analysis with rebuttals |
| `/grok verify <claim>` | Fact-check against live data sources |
| `/grok analyze <topic>` | Deep analysis with reasoning transparency |
| `/grok trending [category]` | Current trending topics in real-time |
| `/grok summarize <url>` | Live URL summary with key facts |
| `/grok compare <topics>` | Side-by-side comparison of competing ideas |
| `/grok deep-dive <topic>` | Extended investigation with source mapping |

## Core Architecture

**8 Sub-Skills:**
- `grok-query` - Real-time data retrieval & source aggregation
- `grok-debate` - Adversarial argument generation & rebuttal
- `grok-verify` - Live fact-checking against primary sources
- `grok-analyze` - Multi-dimensional analysis with reasoning paths
- `grok-trending` - Real-time trend detection & categorization
- `grok-summarize` - URL parsing & rapid summarization
- `grok-compare` - Feature-by-feature comparison matrix
- `grok-deep-dive` - Extended research with source provenance

**5 Specialized Agents:**
- `grok-researcher` - Live data source finder & aggregator
- `grok-debater` - Argument generation specialist
- `grok-fact-checker` - Verification expert
- `grok-synthesizer` - Cross-source integration specialist
- `grok-explainer` - Reasoning transparency & explanation

## 5-Gate Delivery Contract for Real-Time Data

| Gate | Enforces | Implementation |
|---|---|---|
| 1. Source Verification | All data has retrievable URLs | `scripts/grok_verify_sources.py --gate 1` |
| 2. Timeliness Check | Data is < 24 hours old (configurable) | `scripts/grok_check_freshness.py` |
| 3. Bias Detection | Multi-source comparison completed | `scripts/grok_detect_bias.py` |
| 4. Fact Verification | Disputed claims fact-checked | `agents/grok-fact-checker.md` |
| 5. Reasoning Chain | Justification provided for conclusions | `scripts/grok_validate_reasoning.py` |

## Quality Scoring (100 points)

| Category | Points | Focus |
|---|---:|---|
| Source Diversity | 25 | Multiple independent sources cited |
| Timeliness | 20 | Data freshness & current relevance |
| Accuracy | 20 | Fact-checked against live sources |
| Reasoning Clarity | 20 | Logical flow & evidence connection |
| Bias Awareness | 15 | Acknowledgment of competing perspectives |

## Execution Flow

1. **Parse** - Identify query type & urgency level
2. **Source** - Spawn `grok-researcher` for live data retrieval
3. **Analyze** - Synthesize across multiple sources
4. **Verify** - Spawn `grok-fact-checker` for verification
5. **Reason** - Expose reasoning chain with evidence links
6. **Review** - Run 5-gate delivery contract
7. **Deliver** - Output with source citations & confidence scores

## Integration Points

- Live API connections: NewsAPI, Google Trends, SEC EDGAR, Twitter API, Reddit API
- Fact-check APIs: PolitiFact API, FactCheck.org API, Reuters Fact Check
- Real-time markets: CoinGecko, AlphaVantage, Yahoo Finance
- Academic sources: PubMed, arXiv, Google Scholar

## Anti-Patterns (Never Do These)

| Anti-Pattern | Why |
|-------------|-----|
| Use outdated sources for current events | Accuracy destroyed by time-sensitive changes |
| Omit competing viewpoints | Loses debate/analysis credibility |
| Hide reasoning steps | User loses ability to verify conclusions |
| Report without source links | Unverifiable claims undermine trust |
| Mix opinion with facts without labels | Confuses evidence-backed vs. speculative content |
