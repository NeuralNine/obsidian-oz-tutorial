---
title: "Quamina and Claude, Case 1"
url: "https://www.tbray.org/ongoing/When/202x/2026/02/06/Q-Plus-C-Ch1"
hn_id: 47020879
hn_url: "https://news.ycombinator.com/item?id=47020879"
date: 2026-02-18
tags: [ai, claude, llm, code-optimization, go-programming]
source: hackernews
---

# Summary

Tim Bray, with 47 years of coding experience, shares a case study of Claude being applied to his open-source Go library Quamina (a high-performance pattern matching library based on finite automata). A collaborator named Rob Sayre began sending Claude-generated PRs that roughly doubled Quamina's performance on several benchmarks.

The initial PRs focused on standard Go optimization techniques: pre-allocating slice capacities and reusing slices across operations to minimize memory allocation. But Claude also identified two non-trivial improvements: precomputing NFA epsilon closures when building the automaton rather than during matching, and replacing map-based memoization with integer generation counters.

Rob's workflow involved telling Claude to profile memory and CPU benchmarks, then selecting from Claude's good and bad suggestions. When Tim left code review comments, Rob would tell Claude to address them, often getting "one-shot" fixes. The PRs were well-commented with decent code and maintained test coverage.

Bray explicitly avoids drawing conclusions, positioning this as pure anecdata amid the polarized debate about GenAI in software development. He promises to share additional case studies before offering any final assessment.

## Key Takeaways

- Claude-generated PRs doubled Quamina's performance on multiple benchmarks
- AI identified both standard optimizations and non-trivial algorithmic improvements
- Workflow involved profiling, AI suggestions, human selection and refinement
- PRs maintained test coverage and code quality standards
- Author intentionally avoids advocacy, positioning as objective case study
