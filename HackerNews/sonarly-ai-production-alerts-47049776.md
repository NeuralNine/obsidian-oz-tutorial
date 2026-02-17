---
title: "Sonarly (YC W26) – AI agent to triage and fix your production alerts"
url: "https://sonarly.com/"
hn_id: 47049776
hn_url: "https://news.ycombinator.com/item?id=47049776"
date: 2026-02-17
tags: [ai, devops, monitoring, startup, yc, machine-learning, agents]
source: hackernews
---

# Summary

Sonarly, a Y Combinator W26 company, has launched an AI-powered solution for triaging and fixing production alerts. The tool connects to existing observability platforms like Sentry, Datadog, and Slack feedback channels to automatically group duplicates, analyze root causes, and suggest fixes—dramatically reducing Mean Time To Repair (MTTR).

The founders built Sonarly after experiencing alert fatigue firsthand while running a B2C edtech app with thousands of users. With up to 50 Sentry alerts per day and only two people on the team, they struggled to filter noise from actual problems. Their solution reduced one customer's alerts from 180/day to 50/day through intelligent grouping, then down to just 5 priority issues by analyzing severity and impact.

The architecture works in three steps: deduplicating before triggering a coding agent, gathering root cause analysis for each alert, and re-grouping by RCA. For multi-repo and multi-service architectures, they built an internal map that dynamically tracks links between services, logs, and metrics—enabling Claude Code to understand issues faster.

A key insight from the founders: while Claude Code excels at writing code, handling runtime issues requires deep runtime context, immediate reactivity, and intelligent triage that can't simply pipe every alert into an agent.

## Key Takeaways

- Connects to Sentry, Datadog, and Slack to consolidate production alerts
- Uses AI to deduplicate, analyze root causes, and suggest fixes
- Reduced one customer's daily alerts from 180 to 5 priority issues
- Built internal service mapping for complex multi-repo architectures
- YC W26 company with self-serve product and large free tier
