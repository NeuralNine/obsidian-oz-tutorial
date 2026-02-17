---
title: "Study: Self-generated Agent Skills are useless"
url: "https://arxiv.org/abs/2602.12670"
hn_id: 47040430
hn_url: "https://news.ycombinator.com/item?id=47040430"
date: 2026-02-17
tags: [ai, machine-learning, llm, agents, research, paper]
source: hackernews
---

# Summary

This research paper introduces SkillsBench, a comprehensive benchmark designed to measure the effectiveness of Agent Skills - structured packages of procedural knowledge that augment LLM agents at inference time. The benchmark includes 86 tasks across 11 domains, each paired with curated Skills and deterministic verifiers.

The study tested 7 agent-model configurations over 7,308 trajectories under three conditions: no Skills, curated Skills, and self-generated Skills. Results show that curated Skills improve average pass rates by 16.2 percentage points, though effectiveness varies dramatically by domain - from just +4.5pp for Software Engineering to an impressive +51.9pp for Healthcare.

A critical finding is that self-generated Skills provide no benefit on average. This demonstrates that current models cannot reliably author the procedural knowledge they benefit from consuming - a significant limitation for autonomous agent systems. Interestingly, focused Skills with 2-3 modules outperform comprehensive documentation, and smaller models equipped with good Skills can match the performance of larger models without them.

## Key Takeaways

- Curated Skills improve LLM agent performance by 16.2 percentage points on average
- Self-generated Skills provide zero average benefit - models cannot create the procedural knowledge they consume effectively
- Effectiveness varies widely by domain (Healthcare: +51.9pp vs Software Engineering: +4.5pp)
- 16 of 84 tasks showed negative deltas with Skills - they can sometimes hurt performance
- Focused, modular Skills (2-3 modules) outperform comprehensive documentation
- Smaller models with Skills can match larger models without them
