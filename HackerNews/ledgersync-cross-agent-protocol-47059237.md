---
title: "LedgerSync – A cross-agent shared-memory protocol for AI coding"
url: "https://github.com/Metacog-AI/ledgersync"
hn_id: 47059237
hn_url: "https://news.ycombinator.com/item?id=47059237"
date: 2026-02-18
tags: [ai, llm, developer-tools, multi-agent, ai-coding]
source: hackernews
---

# Summary

LedgerSync is a file-based protocol designed to solve context loss when switching between AI coding agents like Claude, Cursor, and Copilot. When hitting rate limits or switching tools, developers often lose all context and must re-explain their project. LedgerSync creates a shared memory layer that all agents can read.

The system has two components: a ledger.jsonl file where agents log every decision with reasoning, and "grounding docs" that define the product's philosophy, design principles, and user research. Agents read these before writing code, ensuring decisions align with product vision rather than generic best practices.

Each ledger entry captures what happened, why (with considerations and uncertainties), and how it aligns with grounding documents. This creates rich reasoning traces—for example noting "PKCE chosen over implicit—security-first principle" with references to the philosophy document.

The tool integrates with Claude Code (CLAUDE.md), Cursor (.cursorrules), GitHub Copilot, and Codex via agent-specific instruction files. The philosophy emphasizes file-first operation (no servers), append-only logging, and human authority over AI suggestions.

## Key Takeaways

- Solves context loss when switching between AI coding agents
- File-based protocol with no servers or accounts required
- Grounding docs encode product philosophy for consistent agent decisions
- Captures reasoning traces with confidence levels and alignment notes
- Integrates with Claude Code, Cursor, Copilot, and Codex
