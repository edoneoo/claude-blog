---
name: gpt-5
description: >
  Advanced reasoning and creative synthesis platform powered by GPT-5.6's 
  enhanced context window and multi-modal reasoning. Routes through 8 specialized 
  sub-skills for complex problem solving, creative ideation, code generation, 
  and long-form reasoning. Optimized for 200K+ context window and structured 
  thinking tasks.
license: MIT
compatibility: Requires Claude Code and Python 3.11+; OpenAI GPT-5.6 API
metadata:
  author: @edoneoo
  version: "1.0.0"
  model: gpt-5-turbo-extended
user-invokable: true
argument-hint: "[reason|create|code|research|brainstorm|architect|optimize|solve]"
---

# GPT-5.6: Advanced Reasoning & Creative Synthesis

Full-lifecycle advanced reasoning platform: complex problem decomposition, creative solution generation, 
code architecture design, research synthesis, and strategic planning. Leverages 200K+ context window 
for deep analysis and multi-step reasoning chains.

## Quick Reference

| Command | What it does |
|---------|-------------|
| `/gpt5 reason <problem>` | Multi-step logical reasoning with full chain |
| `/gpt5 create <brief>` | Creative content generation with style control |
| `/gpt5 code <spec>` | Architecture-aware code generation |
| `/gpt5 research <query>` | Deep research synthesis with source integration |
| `/gpt5 brainstorm <topic>` | Ideation with structured idea ranking |
| `/gpt5 architect <system>` | System design with trade-off analysis |
| `/gpt5 optimize <problem>` | Performance optimization with benchmarks |
| `/gpt5 solve <challenge>` | Complex problem solving with multiple approaches |

## Core Architecture

**8 Sub-Skills:**
- `gpt5-reason` - Multi-step logical reasoning & chain-of-thought
- `gpt5-create` - Creative generation with style templates
- `gpt5-code` - Code architecture & implementation
- `gpt5-research` - Synthesis research with 200K context
- `gpt5-brainstorm` - Ideation & concept ranking
- `gpt5-architect` - System design & trade-off analysis
- `gpt5-optimize` - Performance & resource optimization
- `gpt5-solve` - Complex problem solving framework

**5 Specialized Agents:**
- `gpt5-reasoner` - Logical reasoning & validation
- `gpt5-creator` - Creative direction specialist
- `gpt5-engineer` - Code architecture expert
- `gpt5-researcher` - Long-form synthesis specialist
- `gpt5-strategist` - System thinking & planning expert

## 5-Gate Delivery Contract for Advanced Reasoning

| Gate | Enforces | Implementation |
|---|---|---|
| 1. Logic Validation | Reasoning chain is sound | `scripts/gpt5_validate_logic.py --gate 1` |
| 2. Completeness | All major considerations addressed | `scripts/gpt5_check_coverage.py` |
| 3. Code Quality | Generated code passes quality gates | `scripts/gpt5_lint_code.py` |
| 4. Reasoning Review | Multi-step reasoning verified | `agents/gpt5-reasoner.md` |
| 5. Integration Test | Outputs integrate with context | `scripts/gpt5_validate_integration.py` |

## Quality Scoring (100 points)

| Category | Points | Focus |
|---|---:|---|
| Reasoning Depth | 25 | Multi-step logic clarity |
| Creativity | 20 | Novel & useful ideas |
| Technical Soundness | 20 | Code quality & architecture |
| Completeness | 20 | Coverage of edge cases |
| Integration Clarity | 15 | How solution fits larger context |

## Execution Flow

1. **Parse** - Identify problem type & complexity level
2. **Decompose** - Spawn `gpt5-reasoner` for problem breakdown
3. **Explore** - Generate multiple solution approaches
4. **Evaluate** - Analyze trade-offs & constraints
5. **Synthesize** - Create integrated solution
6. **Review** - Run 5-gate delivery contract
7. **Deliver** - Output with reasoning transparency & alternatives

## Context Window Usage

- **Status Quo**: 8K-16K context (standard reasoning)
- **Extended**: 100K+ context (research synthesis, code review)
- **Maximum**: 200K context (book-length document processing)
- **Adaptive**: Auto-select based on query complexity

## Integration Points

- Code analysis: GitHub API, GitLab, static analyzers
- Research: arXiv, Google Scholar, academic databases
- Ideation: Trend databases, market research APIs
- Validation: Testing frameworks, CI/CD pipelines

## Anti-Patterns (Never Do These)

| Anti-Pattern | Why |
|-------------|-----|
| Ignore edge cases in reasoning | Creates flawed solutions |
| Over-complicate when simpler exists | Wastes context window |
| Hide trade-offs in recommendations | Decision-makers can't evaluate |
| Generate code without architecture | Results in technical debt |
| Rush reasoning without validation | Outputs may be logically unsound |
