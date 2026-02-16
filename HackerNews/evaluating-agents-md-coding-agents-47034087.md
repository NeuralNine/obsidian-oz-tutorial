---
title: "Evaluating AGENTS.md: Are Repository-Level Context Files Helpful for Coding Agents?"
url: "https://arxiv.org/abs/2602.11988"
hn_id: 47034087
hn_url: "https://news.ycombinator.com/item?id=47034087"
date: 2026-02-16
tags: [ai, coding-agents, research, llm, software-engineering, arxiv]
source: hackernews
---

# Summary

This research paper from ETH Zurich investigates whether AGENTS.md context files—repository-level instructions commonly used to guide coding agents—actually help or hinder task completion. Despite being strongly encouraged by agent developers, no rigorous evaluation had previously been conducted.

The researchers evaluated coding agents across two settings: established SWE-bench tasks from popular repositories using LLM-generated context files, and a novel collection of issues from repositories with developer-committed context files. The findings were surprising and counterintuitive.

Across multiple coding agents and LLMs, context files actually tend to **reduce** task success rates compared to providing no repository context. Additionally, they increase inference costs by over 20%. The behavioral analysis revealed that both LLM-generated and human-written context files encourage broader exploration (more testing, more file traversal), and agents do follow the instructions provided.

The core problem: unnecessary requirements in context files make tasks harder. The paper concludes that human-written context files should describe only minimal requirements rather than comprehensive guidelines. This challenges the common practice of creating detailed AGENTS.md files for AI coding assistants.

## Key Takeaways
- AGENTS.md files often reduce coding agent success rates
- Context files increase inference costs by over 20%
- Agents do follow instructions, but unnecessary requirements cause problems
- Both LLM-generated and developer-written files encourage broader (often counterproductive) exploration
- Recommendation: context files should contain only minimal, essential requirements
