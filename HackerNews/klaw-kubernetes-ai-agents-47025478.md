---
title: "Klaw.sh – Kubernetes for AI agents"
url: "https://github.com/klawsh/klaw.sh"
hn_id: 47025478
hn_url: "https://news.ycombinator.com/item?id=47025478"
date: 2026-02-17
tags: [ai, ai-agent, kubernetes, devops, infrastructure]
source: hackernews
---

# Summary

Klaw is an open-source platform for deploying and managing AI agents at scale, positioning itself as "Kubernetes for AI agents." Instead of orchestrating containers, it orchestrates intelligent agents that can code, research, communicate, and automate tasks. The project is written in Go and just released v0.1.0.

The platform supports multiple deployment modes: single-node mode for development (interactive chat or full platform with Slack integration), distributed mode with controller-node architecture for scaling across machines, and container mode using Podman for isolated, secure agent execution.

Key features include support for 300+ LLM models through router services (each::labs, OpenRouter, or direct Anthropic), Kubernetes-style multi-tenancy with namespaces and clusters, built-in tools (bash, file read/write, web fetch/search, agent spawning), a composable skills system, scheduled tasks via cron, and multi-channel deployment (CLI, TUI, Slack, API).

The architecture maps directly to Kubernetes concepts: Agent Definition = Container Image, Agent Instance = Pod, Channel = Service, Namespace = Namespace, klaw CLI = kubectl. This familiar paradigm aims to solve agent orchestration challenges similar to how Kubernetes solved container orchestration.

## Key Takeaways

- Open-source platform for deploying/managing AI agents at scale
- Kubernetes-like paradigm: namespaces, clusters, declarative configs
- Supports 300+ models via routing services (OpenRouter, Anthropic, etc.)
- Single-node, distributed, and containerized deployment modes
- Built-in tools for file ops, web access, sub-agent spawning, scheduling
