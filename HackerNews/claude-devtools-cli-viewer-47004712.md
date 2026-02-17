---
title: "Show HN: Claude DevTools - Un-dumb Claude Code's CLI Output"
url: "https://github.com/matt1398/claude-devtools"
hn_id: 47004712
hn_url: "https://news.ycombinator.com/item?id=47004712"
date: 2026-02-14
tags: [ai, llm, claude, developer-tools, cli]
source: hackernews
---

# Summary

Claude DevTools is a local Electron application designed to address visibility issues with Anthropic's Claude Code CLI. Recent updates to the Claude Code CLI have replaced critical output with abbreviated summaries like "Read 3 files" or "Edited 2 files," making it difficult to understand what actually happened during execution.

The tool works by tailing session logs in `~/.claude/` to reconstruct execution traces in real-time, providing a middle ground between minimal output and the verbose JSON dump from `--verbose` mode. It runs entirely locally and requires no API keys.

Key features include inline red/green diffs displayed the moment files are edited, context forensics that breaks down token usage by file vs tool output vs thinking, and agent tree visualizations that help understand sub-agent execution paths which are typically interleaved and confusing in the standard CLI output.

## Key Takeaways

- Solves the visibility gap in Claude Code CLI without requiring wrapper tools
- Provides real-time diff visualization for file edits instead of just checkmarks
- Token usage breakdown helps understand why context windows fill up
- Visualizes sub-agent execution paths for complex agent operations
- 100% local processing with no external API dependencies
