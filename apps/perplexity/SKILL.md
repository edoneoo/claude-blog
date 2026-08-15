---
name: perplexity
description: >
  Deep research and fact verification platform powered by Perplexity's real-time 
  search capabilities and academic database access. Routes through 7 specialized 
  sub-skills for comprehensive research, citation management, fact-checking, and 
  academic sourcing. Optimized for evidence-backed research with full provenance.
license: MIT
compatibility: Requires Claude Code and Python 3.11+; Perplexity API credentials
metadata:
  author: @edoneoo
  version: "1.0.0"
  model: perplexity-sonar-pro
user-invokable: true
argument-hint: "[research|verify|source|academic|deep-search|cite|audit]"
---

# Perplexity: Deep Research & Academic Sourcing

Full-lifecycle research platform: comprehensive literature review, academic sourcing, fact verification, 
citation management, and evidence audit. Leverages real-time search and academic databases for 
authoritative research synthesis.

## Quick Reference

| Command | What it does |
|---------|-------------|
| `/perplexity research <topic>` | Comprehensive research with full citations |
| `/perplexity verify <claim>` | Academic fact-checking across databases |
| `/perplexity source <concept>` | Find authoritative academic sources |
| `/perplexity academic <field>` | Deep academic literature review |
| `/perplexity deep-search <query>` | Extended search across multiple databases |
| `/perplexity cite <claim>` | Generate citations for claims |
| `/perplexity audit <content>` | Verify claims with source mapping |

## Core Architecture

**7 Sub-Skills:**
- `perplexity-research` - Comprehensive research synthesis
- `perplexity-verify` - Academic fact-checking
- `perplexity-source` - Authority source finder
- `perplexity-academic` - Academic literature review
- `perplexity-search` - Deep multi-database search
- `perplexity-cite` - Citation & reference management
- `perplexity-audit` - Content verification audit

**5 Specialized Agents:**
- `perplexity-researcher` - Research synthesis specialist
- `perplexity-fact-checker` - Academic verification expert
- `perplexity-librarian` - Source curation specialist
- `perplexity-scholar` - Academic domain expert
- `perplexity-auditor` - Evidence verification specialist

## 5-Gate Delivery Contract for Research Integrity

| Gate | Enforces | Implementation |
|---|---|---|
| 1. Source Authority | Only Tier 1-2 sources used | `scripts/perplexity_verify_sources.py --gate 1` |
| 2. Citation Completeness | All claims cited | `scripts/perplexity_check_citations.py` |
| 3. Academic Rigor | Peer-review status verified | `scripts/perplexity_check_peer_review.py` |
| 4. Fact Verification | Claims verified against sources | `agents/perplexity-fact-checker.md` |
| 5. Bias Detection | Source diversity & balance checked | `scripts/perplexity_check_bias.py` |

## Quality Scoring (100 points)

| Category | Points | Focus |
|---|---:|---|
| Source Quality | 25 | Authority & peer-review status |
| Citation Completeness | 25 | All claims traceable to sources |
| Research Depth | 20 | Comprehensive coverage |
| Academic Rigor | 20 | Methodology & evidence standards |
| Neutrality | 10 | Balance across perspectives |

## Execution Flow

1. **Map** - Spawn `perplexity-librarian` for source discovery
2. **Research** - Conduct comprehensive literature review
3. **Extract** - Identify key claims & evidence
4. **Verify** - Spawn `perplexity-fact-checker` for verification
5. **Cite** - Generate complete citations
6. **Audit** - Run 5-gate delivery contract
7. **Deliver** - Output with full provenance & citations

## Database Access

- **Academic**: PubMed, arXiv, Google Scholar, JSTOR
- **Scientific**: Nature, Science, Cell, peer-reviewed journals
- **News**: Reuters, AP, BBC, major news archives
- **Legal**: SEC Edgar, court databases, regulatory filings
- **Financial**: Yahoo Finance, Bloomberg (where available)
- **Government**: Census data, CDC, NIST databases

## Citation Formats

- **APA** (Default)
- **MLA**
- **Chicago**
- **Harvard**
- **IEEE**
- **Custom formats**

## Integration Points

- Citation managers: Zotero, Mendeley, BibTeX
- Academic platforms: arXiv, ResearchGate, Academia.edu
- Publisher APIs: Springer, Wiley, Elsevier (where available)
- Fact-check services: PolitiFact, FactCheck.org
- News aggregators: NewsAPI, Google News API

## Anti-Patterns (Never Do These)

| Anti-Pattern | Why |
|-------------|-----|
| Mix primary & secondary sources without distinction | Loses methodological rigor |
| Ignore publication date on time-sensitive topics | Outdated information undermines findings |
| Use non-peer-reviewed sources as primary evidence | Reduces academic credibility |
| Omit contradictory sources | Biases research synthesis |
| Fail to cite extraordinary claims | Violates research integrity |
