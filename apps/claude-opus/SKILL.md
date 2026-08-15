---
name: claude-opus
description: >
  Premium reasoning platform leveraging Claude 3 Opus's nuanced understanding 
  and extended reasoning capabilities. Routes through 9 specialized sub-skills 
  for philosophical analysis, ethical reasoning, complex writing, and ambiguous 
  problem solving. Optimized for tasks requiring deep contextual understanding 
  and nuanced judgment calls.
license: MIT
compatibility: Requires Claude Code and Python 3.11+; Anthropic Claude 3 API
metadata:
  author: @edoneoo
  version: "1.0.0"
  model: claude-3-opus-latest
user-invokable: true
argument-hint: "[analyze|interpret|write|reason|advise|review|refine|synthesize|advocate]"
---

# Claude Opus: Premium Reasoning & Nuanced Understanding

Full-lifecycle premium reasoning platform: philosophical analysis, ethical reasoning, complex writing 
with nuance, ambiguous problem-solving, and contextual judgment. Specialized for tasks requiring 
deep understanding of ambiguity, cultural context, and ethical dimensions.

## Quick Reference

| Command | What it does |
|---------|-------------|
| `/opus analyze <topic>` | Deep contextual analysis with multiple lenses |
| `/opus interpret <text>` | Nuanced interpretation with ambiguity handling |
| `/opus write <brief>` | Complex writing with stylistic control |
| `/opus reason <dilemma>` | Ethical reasoning with competing values |
| `/opus advise <scenario>` | Strategic advice considering full context |
| `/opus review <work>` | Critical review with constructive feedback |
| `/opus refine <draft>` | Refinement with sensitivity to nuance |
| `/opus synthesize <sources>` | Cross-cultural synthesis & integration |
| `/opus advocate <position>` | Strongest case for competing positions |

## Core Architecture

**9 Sub-Skills:**
- `opus-analyze` - Multi-dimensional contextual analysis
- `opus-interpret` - Nuanced interpretation & hermeneutics
- `opus-write` - Complex writing with stylistic control
- `opus-reason` - Ethical reasoning framework
- `opus-advise` - Strategic advice with context
- `opus-review` - Critical review & feedback
- `opus-refine` - Sensitivity-aware refinement
- `opus-synthesize` - Cross-cultural synthesis
- `opus-advocate` - Adversarial argumentation

**5 Specialized Agents:**
- `opus-analyst` - Multi-dimensional analysis expert
- `opus-philosopher` - Ethical reasoning specialist
- `opus-writer` - Literary & nuanced writing expert
- `opus-strategist` - Context-aware strategy specialist
- `opus-interpreter` - Hermeneutics & cultural understanding expert

## 5-Gate Delivery Contract for Nuanced Understanding

| Gate | Enforces | Implementation |
|---|---|---|
| 1. Context Mapping | Full contextual landscape identified | `scripts/opus_map_context.py --gate 1` |
| 2. Ambiguity Handling | Competing interpretations acknowledged | `scripts/opus_identify_ambiguity.py` |
| 3. Nuance Preservation | Subtleties not flattened | `scripts/opus_check_nuance.py` |
| 4. Reasoning Review | Ethical logic validated | `agents/opus-philosopher.md` |
| 5. Sensitivity Check | Cultural/ethical sensitivity verified | `scripts/opus_sensitivity_check.py` |

## Quality Scoring (100 points)

| Category | Points | Focus |
|---|---:|---|
| Contextual Depth | 25 | Understanding of full landscape |
| Nuance Handling | 20 | Preservation of complexity |
| Ethical Rigor | 20 | Sound ethical reasoning |
| Writing Quality | 20 | Clarity within complexity |
| Cultural Sensitivity | 15 | Respectful of diverse perspectives |

## Execution Flow

1. **Map** - Spawn `opus-analyst` for context mapping
2. **Explore** - Identify ambiguities & competing views
3. **Reason** - Apply ethical reasoning framework
4. **Synthesize** - Integrate perspectives with nuance
5. **Compose** - Create refined output
6. **Review** - Run 5-gate delivery contract
7. **Deliver** - Output with context notes & caveats

## Specialization Areas

- **Philosophical**: Ethics, metaphysics, epistemology
- **Writing**: Literary fiction, essays, complex proposals
- **Strategy**: Organizational change, diplomatic solutions
- **Cultural**: Cross-cultural communication, translation
- **Ethical**: Dilemmas, competing values, stakeholder interests

## Integration Points

- Philosophy databases: Stanford Encyclopedia of Philosophy, PhilPapers
- Literary analysis: Project Gutenberg, literary criticism databases
- Cultural studies: Anthropological journals, cultural research
- Strategic planning: Business case studies, diplomatic protocols
- Ethics frameworks: Applied ethics resources, case law

## Anti-Patterns (Never Do These)

| Anti-Pattern | Why |
|-------------|-----|
| Flatten ambiguity into false clarity | Loses essential nuance |
| Ignore cultural/ethical context | Results in insensitive outputs |
| Treat complex issues as simple | Oversimplification undermines credibility |
| Hide reasoning for controversial topics | Reduces transparency & trust |
| Force single perspective on multifaceted issues | Misses reality's complexity |
