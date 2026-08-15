---
name: together-ai
description: >
  Distributed reasoning platform powered by Together AI's inference optimization 
  and multi-model routing. Routes through 7 specialized sub-skills for model 
  selection, prompt optimization, distributed inference, cost optimization, and 
  performance benchmarking. Optimized for production-scale reasoning at scale.
license: MIT
compatibility: Requires Claude Code and Python 3.11+; Together AI API credentials
metadata:
  author: @edoneoo
  version: "1.0.0"
  model: together-ai-router
user-invokable: true
argument-hint: "[route|optimize|distribute|benchmark|cost-analyze|compare|scale]"
---

# Together AI: Distributed Reasoning at Scale

Full-lifecycle distributed inference platform: intelligent model routing, prompt optimization, 
distributed processing, cost optimization, and performance benchmarking. Leverages Together AI's 
inference optimization for production-scale reasoning.

## Quick Reference

| Command | What it does |
|---------|-------------|
| `/together route <task>` | Intelligent model selection & routing |
| `/together optimize <prompt>` | Prompt optimization for efficiency |
| `/together distribute <batch>` | Distributed batch processing |
| `/together benchmark <task>` | Performance & cost benchmarking |
| `/together cost-analyze <workload>` | Cost optimization analysis |
| `/together compare <models>` | Multi-model performance comparison |
| `/together scale <workload>` | Scale processing capacity |

## Core Architecture

**7 Sub-Skills:**
- `together-route` - Intelligent model routing
- `together-optimize` - Prompt & token optimization
- `together-distribute` - Distributed inference
- `together-benchmark` - Performance benchmarking
- `together-cost` - Cost analysis & optimization
- `together-compare` - Model comparison
- `together-scale` - Scaling & load management

**5 Specialized Agents:**
- `together-router` - Model selection specialist
- `together-optimizer` - Prompt optimization expert
- `together-distributor` - Distributed systems expert
- `together-analyst` - Cost & performance analyst
- `together-benchmarker` - Benchmarking specialist

## 5-Gate Delivery Contract for Distributed Processing

| Gate | Enforces | Implementation |
|---|---|---|
| 1. Route Validation | Model selection justified | `scripts/together_validate_route.py --gate 1` |
| 2. Optimization Verification | Prompts optimized | `scripts/together_check_optimization.py` |
| 3. Performance Baseline | Performance measured | `scripts/together_benchmark.py` |
| 4. Cost Verification | Cost within budget | `agents/together-analyst.md` |
| 5. Scaling Check | Handles projected load | `scripts/together_validate_scaling.py` |

## Quality Scoring (100 points)

| Category | Points | Focus |
|---|---:|---|
| Route Accuracy | 25 | Correct model selection |
| Cost Efficiency | 25 | Optimized spend & performance |
| Performance | 20 | Speed & throughput metrics |
| Reliability | 20 | Uptime & consistency |
| Scalability | 10 | Handles growth requirements |

## Execution Flow

1. **Analyze** - Assess task requirements
2. **Route** - Spawn `together-router` for model selection
3. **Optimize** - Optimize prompts & tokens
4. **Distribute** - Prepare for distributed processing
5. **Benchmark** - Run performance tests
6. **Review** - Run 5-gate delivery contract
7. **Deliver** - Output with cost & performance metrics

## Model Categories

- **Fast & Cheap**: Optimized for speed (Mistral, Llama 7B)
- **Balanced**: Quality vs. cost trade-off (Llama 13B, Mistral 7B)
- **Premium**: Highest quality (GPT-4, Claude, Llama 70B)
- **Specialized**: Domain-specific models
- **Custom**: Fine-tuned models

## Routing Intelligence

- **Latency-Optimized**: Fastest response times
- **Cost-Optimized**: Lowest spend per token
- **Quality-Optimized**: Best output quality
- **Throughput-Optimized**: Maximum requests/sec
- **Auto**: Intelligent selection based on SLA

## Integration Points

- Model APIs: OpenAI, Anthropic, Mistral, Together
- Monitoring: Datadog, New Relic, CloudWatch
- Cost tracking: AWS Cost Explorer, Azure Cost Management
- Performance: Prometheus, Grafana dashboards
- Infrastructure: Kubernetes, Docker, Terraform

## Anti-Patterns (Never Do These)

| Anti-Pattern | Why |
|-------------|-----|
| Use one model for all tasks | Wastes money on premium models for simple tasks |
| Ignore cost tracking | Budget overruns without visibility |
| Skip performance benchmarking | Unknown system behavior at scale |
| Over-optimize for single dimension | Ignores trade-offs (speed vs. quality) |
| Fail to monitor routing decisions | Can't identify suboptimal patterns |
