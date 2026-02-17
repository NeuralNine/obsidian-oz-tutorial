---
title: "The Long Tail of LLM-Assisted Decompilation"
url: "https://blog.chrislewis.au/the-long-tail-of-llm-assisted-decompilation/"
hn_id: 47038270
hn_url: "https://news.ycombinator.com/item?id=47038270"
date: 2026-02-17
tags: [ai, llm, decompilation, reverse-engineering, claude, code-generation]
source: hackernews
---

# Summary

Chris Lewis describes his experience using LLMs to decompile the Nintendo 64 game Snowboard Kids 2, exploring how the workflow evolved as the easy functions were completed and harder challenges emerged. After initial rapid progress using one-shot decompilation (going from 25% to 58% matched code), progress dramatically slowed.

The article describes key workflow improvements that helped push the project to ~75% completion. A significant breakthrough came from using function similarity via text embeddings of assembly instructions. By computing similar matched functions for each unmatched function, Claude could use these as references for how particular assembly blocks map to C code. This approach proved highly effective for identifying patterns the model couldn't recognize on its own.

Despite these improvements, the project eventually stalled. Lewis discusses the fundamental limits of LLM-assisted decompilation: while models can quickly handle straightforward functions and those with similar reference examples, they struggle with truly novel or complex logic. The "long tail" of difficult functions requires increasingly sophisticated techniques and human expertise.

The article provides valuable insights for other decompilation projects and demonstrates both the power and limitations of current LLM capabilities for reverse engineering tasks.

## Key Takeaways
- One-shot LLM decompilation worked well initially (25% → 58% matched)
- Function similarity via embeddings helped push progress to ~75%
- Claude benefits from reference examples of similar decompiled functions
- Progress eventually stalls on the hardest remaining functions
- Demonstrates practical limits of LLM code generation for complex tasks
