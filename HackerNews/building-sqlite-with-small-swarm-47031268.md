---
title: "Building SQLite with a small swarm"
url: "https://kiankyars.github.io/machine_learning/2026/02/12/sqlite.html"
hn_id: 47031268
hn_url: "https://news.ycombinator.com/item?id=47031268"
date: 2026-02-16
tags: [ai, machine-learning, llm, coding-agents, programming]
source: hackernews
---

# Summary
This article explores an experiment in using parallel AI coding agents to build a SQLite implementation from scratch. The author employed multiple AI models (Claude, Codex, and Gemini) working simultaneously in a swarm-like configuration to generate code.

The project produced approximately 18,650 lines of Rust code and 199 lines of shell scripts across 154 commits in just two days (February 10-12, 2026). The harness includes specialized prompts for agent bootstrapping, task execution, and code coalescing.

The workflow involves launching multiple agents that work on different parts of the codebase, with a coalescing step to merge their contributions. The author shares resource usage data, noting that Gemini operates on a 24-hour basis, Codex used 100% of a Pro Plan's weekly allocation, and Claude used about 70% of Pro weekly usage.

The experiment demonstrates both the potential and limitations of parallel AI coding approaches, with the author providing detailed replication instructions and analysis of the methodology.

## Key Takeaways
- Parallel AI coding agents can produce substantial codebases quickly when properly coordinated
- Different AI models (Claude, Codex, Gemini) can be combined in swarm workflows
- Resource management is crucial - various models have different usage patterns and limits
- A harness/orchestration layer is necessary to coordinate multiple agents and merge their outputs
- The approach shows promise but has limitations that need further exploration
