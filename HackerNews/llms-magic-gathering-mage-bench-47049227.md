---
title: "I taught LLMs to play Magic: The Gathering against each other"
url: "https://mage-bench.com/"
hn_id: 47049227
hn_url: "https://news.ycombinator.com/item?id=47049227"
date: 2026-02-17
tags: [ai, llm, games, benchmark, machine-learning, research]
source: hackernews
---

# Summary

A developer has created Mage-Bench, a platform for teaching and benchmarking LLMs playing Magic: The Gathering against each other. The system uses MCP (Model Context Protocol) tools connected to the open-source XMage codebase to enable AI models to play the complex card game.

Magic: The Gathering presents an interesting challenge for AI due to its combinatorial complexity, need for strategic planning, and requirement to understand nuanced card interactions. Unlike simpler games, MTG involves hidden information, resource management, and emergent interactions between thousands of unique cards.

The project is still in active development—the creator notes it's "still pretty buggy" with significant room for improvement through tooling enhancements. Ratings for expensive frontier models are currently artificially low because development has focused on cheaper models while bugs are being worked out.

The platform allows different LLM models to compete against each other, providing an interesting benchmark for evaluating AI capabilities in complex strategic reasoning. The use of the XMage open-source codebase enables full rules enforcement and game state management.

## Key Takeaways

- Mage-Bench enables LLMs to play Magic: The Gathering via MCP tools
- Built on open-source XMage codebase for rules enforcement
- Provides benchmark for strategic reasoning in complex games
- Currently in active development with focus on tooling improvements
- Frontier model ratings are low due to limited testing during bug fixes
