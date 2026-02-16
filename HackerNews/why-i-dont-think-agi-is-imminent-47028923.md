---
title: "Why I don't think AGI is imminent"
url: "https://dlants.me/agi-not-imminent.html"
hn_id: 47028923
hn_url: "https://news.ycombinator.com/item?id=47028923"
date: 2026-02-16
tags: [ai, agi, deep-learning, cognitive-science, llm]
source: hackernews
---

# Summary

This thoughtful critique challenges claims from OpenAI and Anthropic CEOs that human-level AI is imminent. The author, who holds an MS in Machine Learning, argues that transformer-based LLMs face fundamental architectural limitations when it comes to replicating human cognition.

The core argument centers on "cognitive primitives"—hardwired capabilities like number sense, object permanence, causality, and spatial navigation that evolved in vertebrate brains over hundreds of millions of years. Language evolved atop these primitives and takes them for granted. Consider "Mary held a ball"—humans instantly understand Mary is animate, the ball is inanimate, gravity exists, the ball can't pass through her palm, etc. None of this is in the text.

LLMs are trying to reverse-engineer these primitives from language alone, which is extremely difficult. This explains observed failures: transformers can't reliably do multi-digit arithmetic (no number sense), can't infer "B is A" from "A is B" (no compositional symbolic machinery). Video training helps somewhat but doesn't solve the problem—predicting that a marble reappears from under a cup isn't the same as truly representing object permanence.

The author examines recent work like DeepMind's SIMA 2 and Dreamer 4, finding that embodied training doesn't transfer to language reasoning—the capabilities exist in separate parameter regions. The fundamental gap: organisms don't merely observe reality to predict what happens next; they perceive in order to act. This tight perception-action coupling may be essential for developing robust cognitive primitives.

## Key Takeaways
- Human cognition relies on evolutionary "cognitive primitives" hardwired over millions of years
- Language assumes shared cognitive foundations that LLMs must reverse-engineer from text alone
- LLM failures (arithmetic, logical reversal) map to missing cognitive primitives
- Video/embodied training hasn't shown transfer to improved language reasoning
- Perception-action coupling may be essential—AI lacks rich multisensory embodied experience
