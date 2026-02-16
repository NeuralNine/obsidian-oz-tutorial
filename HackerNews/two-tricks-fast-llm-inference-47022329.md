---
title: "Two different tricks for fast LLM inference"
url: "https://www.seangoedecke.com/fast-llm-inference/"
hn_id: 47022329
hn_url: "https://news.ycombinator.com/item?id=47022329"
date: 2026-02-16
tags: [ai, llm, inference, openai, anthropic, performance]
source: hackernews
---

# Summary

This technical analysis compares how Anthropic and OpenAI achieve their recently announced "fast mode" inference, revealing fundamentally different approaches. Anthropic offers up to 2.5x faster tokens per second (~170 vs 65) while serving their actual Opus 4.6 model. OpenAI offers 15x faster inference (1000+ tokens/second) but uses a new, less capable model called GPT-5.3-Codex-Spark.

Anthropic's approach likely uses low-batch-size inference. The key insight is that GPU memory bandwidth is the main bottleneck—copying data onto GPUs is slow even though GPUs themselves are fast. Batching multiple users increases throughput but adds latency. Anthropic's "fast mode" essentially guarantees your bus leaves immediately, costing 6x more because you're paying for empty seats.

OpenAI's approach uses Cerebras partnership with their giant wafer-scale chips (70 square inches vs ~1 square inch for H100). These chips have 44GB of internal SRAM—enough to fit a smaller model entirely in fast memory, eliminating the slow weight-streaming bottleneck. The catch: 44GB only fits ~40B parameters at int8, forcing OpenAI to use a distilled "Spark" model that shows "small model smell" in tool call handling.

The author argues fast-but-less-capable inference is a bad tradeoff: agent usefulness is dominated by mistake rate, not raw speed. Most user time is spent handling mistakes, so 6x speed at 20% more errors is a poor bargain. However, these fast models may find use as lower-level primitives within larger AI systems.

## Key Takeaways
- Anthropic's fast mode: same model, lower batch size, 6x cost for 2.5x speed
- OpenAI's fast mode: distilled smaller model on Cerebras chips, 15x speed
- Memory bandwidth, not compute, is the main inference bottleneck
- Cerebras chips have 44GB SRAM—enough for ~40B param models only
- Fast-but-less-capable may be worse tradeoff than slower-but-smarter for agents
