---
title: "WebMCP Proposal"
url: "https://webmachinelearning.github.io/webmcp/"
hn_id: 47037501
hn_url: "https://news.ycombinator.com/item?id=47037501"
date: 2026-02-17
tags: [ai, agents, web-dev, browser, mcp, javascript, api]
source: hackernews
---

# Summary

The WebMCP API is a proposed JavaScript interface that enables web applications to expose functionality as "tools" that AI agents can invoke. This specification from the Web Machine Learning Working Group defines how web developers can register JavaScript functions with natural language descriptions and structured schemas for AI agent consumption.

The API provides methods like `navigator.mcp.register()` to register tools with the browser, clearing any pre-existing tools before adding new ones. Individual tools can be added via `navigator.mcp.registerTool()` or removed with `navigator.mcp.unregisterTool()`. Each tool has a unique identifier used by AI agents to invoke it, along with natural language descriptions that help agents understand the tool's functionality.

This proposal represents a standardization effort for the Model Context Protocol (MCP) in browser environments, potentially enabling a more seamless integration between web applications and AI agents. It allows web developers to make their applications AI-agent-friendly without requiring backend changes.

## Key Takeaways

- WebMCP enables web apps to expose JavaScript functions as tools for AI agents
- Tools include natural language descriptions and structured schemas for agent understanding
- Part of standardization effort by the Web Machine Learning Working Group
- Provides methods to register, unregister, and manage tool sets in the browser
- Could enable tighter integration between browser-based apps and AI assistants
- Allows frontend-only AI tool integration without backend modifications
