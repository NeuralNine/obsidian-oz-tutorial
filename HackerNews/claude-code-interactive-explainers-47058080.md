---
title: "Beautiful interactive explainers generated with Claude Code"
url: "https://paraschopra.github.io/explainers/"
hn_id: 47058080
hn_url: "https://news.ycombinator.com/item?id=47058080"
date: 2026-02-18
tags: [ai, claude, llm, visualization, education]
source: hackernews
---

# Summary

A developer used Claude Code (with Opus 4.6) to generate beautiful interactive explainers on complex topics, largely with single-shot prompting and minimal manual adjustment. The project was inspired by explainers.blog and demonstrates current frontier models' ability to produce detailed, animated educational content.

The site includes interactive explainers on: diffusion models and AI image generation, Fourier transforms and how Shazam works, biological scaling laws, cellular automata and emergent complexity, and how LLMs work internally. Each explainer features detailed animations and interactive elements.

Key learnings from the project: prompting Claude Code to test builds using headless Chromium was essential, there are subtle bugs in generated content (like showing human lifespan as 40 years in one animation), and asking Claude Code to verify its plan via Codex works well.

The creator emphasizes that pages were "mostly one-shot" which is notable given how detailed the pages and animations are. This demonstrates the current capabilities of AI code generation for creating rich interactive web content.

## Key Takeaways

- Frontier AI models can generate detailed interactive educational content in single shots
- Claude Code + Opus 4.6 used to create animated explainers on complex topics
- Testing with headless Chromium helps catch issues during generation
- Some subtle errors still occur, requiring human review
- Demonstrates rapid prototyping potential for educational content
