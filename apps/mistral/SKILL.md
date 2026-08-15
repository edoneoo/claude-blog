---
name: mistral
description: >
  Fast reasoning and technical analysis platform powered by Mistral Large's 
  efficient reasoning and multilingual capabilities. Routes through 7 specialized 
  sub-skills for code analysis, performance optimization, technical documentation, 
  and rapid problem-solving. Optimized for speed without sacrificing accuracy.
license: MIT
compatibility: Requires Claude Code and Python 3.11+; Mistral API credentials
metadata:
  author: @edoneoo
  version: "1.0.0"
  model: mistral-large-latest
user-invokable: true
argument-hint: "[analyze|optimize|document|debug|review|refactor|evaluate]"
---

# Mistral Large: Fast Reasoning & Technical Analysis

Full-lifecycle technical analysis platform: code analysis & optimization, technical documentation, 
performance debugging, rapid problem-solving, and system design review. Emphasizes speed and 
technical accuracy for professional development teams.

## Quick Reference

| Command | What it does |
|---------|-------------|
| `/mistral analyze <code>` | Comprehensive code analysis |
| `/mistral optimize <code>` | Performance optimization suggestions |
| `/mistral document <code>` | Auto-generate technical documentation |
| `/mistral debug <issue>` | Rapid debugging & root cause analysis |
| `/mistral review <code>` | Code review with actionable feedback |
| `/mistral refactor <code>` | Refactoring recommendations |
| `/mistral evaluate <solution>` | Solution evaluation against requirements |

## Core Architecture

**7 Sub-Skills:**
- `mistral-analyze` - Code analysis & pattern detection
- `mistral-optimize` - Performance optimization
- `mistral-document` - Auto-documentation generation
- `mistral-debug` - Debugging & diagnosis
- `mistral-review` - Code review process
- `mistral-refactor` - Refactoring guidance
- `mistral-evaluate` - Solution evaluation

**5 Specialized Agents:**
- `mistral-analyst` - Code analysis expert
- `mistral-optimizer` - Performance specialist
- `mistral-documentarian` - Technical writing expert
- `mistral-debugger` - Debugging specialist
- `mistral-architect` - System design expert

## 5-Gate Delivery Contract for Technical Accuracy

| Gate | Enforces | Implementation |
|---|---|---|
| 1. Code Parsing | Code parses without errors | `scripts/mistral_validate_syntax.py --gate 1` |
| 2. Analysis Completeness | All code aspects analyzed | `scripts/mistral_check_coverage.py` |
| 3. Performance Baseline | Current performance measured | `scripts/mistral_benchmark.py` |
| 4. Recommendation Validity | Suggestions are implementable | `agents/mistral-optimizer.md` |
| 5. Test Coverage | Solutions include test cases | `scripts/mistral_check_tests.py` |

## Quality Scoring (100 points)

| Category | Points | Focus |
|---|---:|---|
| Technical Accuracy | 30 | Correctness of analysis |
| Actionability | 20 | Implementability of suggestions |
| Performance Impact | 20 | Measured improvements |
| Code Quality | 20 | Standards & best practices |
| Documentation | 10 | Clarity of explanation |

## Execution Flow

1. **Parse** - Validate code syntax & structure
2. **Analyze** - Spawn `mistral-analyst` for deep analysis
3. **Benchmark** - Measure current performance
4. **Optimize** - Generate optimization suggestions
5. **Document** - Auto-generate documentation
6. **Review** - Run 5-gate delivery contract
7. **Deliver** - Output with benchmarks & test cases

## Language Support

- **Primary**: Python, JavaScript, Java, C++, Go, Rust
- **Secondary**: TypeScript, Ruby, PHP, Swift, Kotlin, C#
- **Scripting**: Bash, PowerShell, SQL, YAML
- **Markup**: HTML, CSS, XML, JSON, TOML
- **IaC**: Terraform, CloudFormation, Ansible

## Performance Analysis Metrics

- Time Complexity: Big O analysis
- Space Complexity: Memory usage patterns
- CPU Usage: Profiling & optimization
- Memory Leaks: Detection & remediation
- Cache Efficiency: Hit rates & optimization
- I/O Performance: Latency & throughput
- Database Queries: Optimization & indexing

## Integration Points

- Version Control: GitHub, GitLab, Bitbucket
- CI/CD: Jenkins, GitHub Actions, GitLab CI
- Profiling: Python cProfile, Node.js profiler, JProfiler
- Testing: pytest, Jest, JUnit, unittest
- Documentation: Sphinx, JSDoc, JavaDoc, Rustdoc
- Performance: Datadog, New Relic, Prometheus

## Anti-Patterns (Never Do These)

| Anti-Pattern | Why |
|-------------|-----|
| Optimize without profiling | Wastes effort on non-bottlenecks |
| Ignore scalability for speed | Creates problems at scale |
| Over-optimize premature code | Reduces maintainability |
| Skip testing in optimization | Introduces bugs |
| Document after optimization | Documentation becomes outdated |
