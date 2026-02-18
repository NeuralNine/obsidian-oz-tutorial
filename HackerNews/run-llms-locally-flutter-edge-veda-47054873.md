---
title: "Run LLMs locally in Flutter with <200ms latency"
url: "https://github.com/ramanujammv1988/edge-veda"
hn_id: 47054873
hn_url: "https://news.ycombinator.com/item?id=47054873"
date: 2026-02-18
tags: [ai, llm, flutter, mobile, on-device-ai, deep-learning]
source: hackernews
---

# Summary

Edge-Veda is a managed on-device AI runtime designed specifically for Flutter applications, enabling text, vision, speech, and RAG capabilities to run sustainably on mobile devices under real-world constraints. The project addresses critical pain points that cause most on-device AI demos to fail in production: thermal throttling, memory spikes, session instability beyond 60 seconds, and lack of debugging visibility.

The library is substantial at approximately 22,700 lines of code, offering 50 C API functions and 32 Dart SDK files with zero cloud dependencies. This makes it a truly private-by-default solution for developers who want to run AI inference locally without relying on external services.

Edge-Veda's approach focuses on sustainability and stability rather than raw performance benchmarks, acknowledging that real mobile devices have thermal and memory constraints that typical AI demos ignore. The framework provides developers with visibility into runtime behavior, making debugging and optimization possible.

The project represents a significant step toward practical on-device AI for mobile developers, particularly those working in the Flutter ecosystem who need reliable, low-latency inference without the privacy concerns of cloud-based solutions.

## Key Takeaways

- Achieves sub-200ms latency for on-device LLM inference in Flutter
- Addresses real-world production issues: thermal throttling, memory management, session stability
- Zero cloud dependencies - fully private by default
- Comprehensive SDK with 50 C API functions and 32 Dart SDK files
- Supports multiple AI modalities: text, vision, speech, and RAG
