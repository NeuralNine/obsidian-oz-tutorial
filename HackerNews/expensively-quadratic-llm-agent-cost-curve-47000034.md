---
title: "Expensively Quadratic: The LLM Agent Cost Curve"
url: "https://blog.exe.dev/expensively-quadratic"
hn_id: 47000034
hn_url: "https://news.ycombinator.com/item?id=47000034"
date: 2026-02-16
tags: [ai, llm, agents, cost-optimization, inference]
source: hackernews
---

# Summary

This technical article from exe.dev explores the often-overlooked quadratic cost growth in LLM agent conversations. The authors demonstrate that as coding agent conversations progress, cache reads increasingly dominate costs—reaching 87% of total costs by conversation end in their example, and hitting 50% of costs at just 27,500 tokens.

The mechanics work like this: LLM providers charge differently for input tokens, cache writes, cache reads, and output tokens. Each subsequent call reads the entire conversation history from cache, creating a triangular accumulation pattern that grows quadratically with conversation length and number of LLM calls.

Through analysis of 250 real conversations from their platform, the authors visualize how cumulative costs evolve. The cost isn't purely tokens-squared—it's tokens multiplied by number of calls, and different conversations have wildly different call patterns based on how much code is written, how many tool calls are made, and whether cache expires.

The article proposes several strategies for managing these costs: "dead reckoning" (fewer LLM calls with less feedback), avoiding splitting large tool outputs into multiple calls, using subagents for iteration outside the main context, and simply starting new conversations more often—which may feel wasteful but is often cheaper than continuing.

## Key Takeaways
- Cache reads can dominate LLM agent costs (87% by end of long conversations)
- Cost growth is quadratic: tokens × number of calls, not just tokens squared
- At ~20,000 tokens, cache reads typically start dominating costs
- Starting fresh conversations is often cheaper than continuing long ones
- Subagents and LLM-assisted tools can offload iteration from the main context
