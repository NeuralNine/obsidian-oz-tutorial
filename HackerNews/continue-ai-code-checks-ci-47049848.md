---
title: "Continue – Source-controlled AI checks, enforceable in CI"
url: "https://docs.continue.dev"
hn_id: 47049848
hn_url: "https://news.ycombinator.com/item?id=47049848"
date: 2026-02-17
tags: [ai, developer-tools, code-review, ci-cd, machine-learning]
source: hackernews
---

# Summary

Continue has launched a new product that runs AI-powered code checks on every pull request. The team developed this solution after experiencing PR review fatigue as they scaled their use of AI coding agents. Each check is defined as a source-controlled markdown file in `.continue/checks/` that appears as a GitHub status check.

What makes this approach unique is that checks run as full agents—not just reading the diff, but able to read/write files, run bash commands, and use a browser. When an issue is found, the check fails with a one-click option to accept a diff fix. If nothing is wrong, it passes silently.

The team shared an example check for "Metrics Integrity" that watches for changes that could unintentionally distort analytics metrics—a particularly insidious type of bug that corrupts dashboards without triggering errors or test failures. This check caught a PR that would have silently deflated session counts.

To get started, users can prompt their AI coding agent (like Claude Code) to explore their codebase and write appropriate checks. The agent will analyze past review comments, identify patterns, and create checks in the `.continue/checks/` directory.

## Key Takeaways

- AI checks run as full agents with file access, bash commands, and browser capabilities
- Checks are stored as markdown files under version control
- One-click fix acceptance when issues are found
- Particularly useful for catching subtle bugs that don't trigger test failures
- Can be set up by prompting an AI coding agent to analyze codebase patterns
