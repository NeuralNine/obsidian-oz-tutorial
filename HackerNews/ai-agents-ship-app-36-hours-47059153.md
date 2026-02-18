---
title: "AI agents designed and shipped this app end-to-end in 36 hours for $270"
url: "https://www.ninjaflix.ai/"
hn_id: 47059153
hn_url: "https://news.ycombinator.com/item?id=47059153"
date: 2026-02-18
tags: [ai, multi-agent, automation, video-generation, llm]
source: hackernews
---

# Summary

NinjaTech AI demonstrated a team of 4 AI agents that designed and deployed a complete web application in 36 hours with approximately $270 in compute costs. The app, NinjaFlix, turns trending news into AI-generated short videos using Sora 2 Pro and Veo 3.1.

The agents autonomously chose the tech stack, designed UX, built frontend and backend, created the content pipeline, and deployed to production with minimal human intervention. Three additional agents now run the platform 24/7, researching news, debating story selection, and generating videos continuously.

Each video includes the agents' debate transcript showing genuine disagreement—Scout (researcher) pushes for data-driven stories, Pixel (designer) argues for visual potential, and Bolt (developer) challenges technical feasibility. The best videos come from rounds where agents actually fought about the topic rather than quick consensus.

Known limitations: groupthink produces boring output, video quality is inconsistent (struggles with hands, text, spatial relationships), news selection has recency/virality bias, and agents occasionally hallucinate context. The stack uses Anthropic Opus 3.5 for reasoning, Tavily for research, and agents coordinate via Slack.

## Key Takeaways

- 4 AI agents autonomously built and deployed a complete web app in 36 hours
- Total compute cost approximately $270 with minimal human intervention
- Agent disagreement produces better output than quick consensus
- 3 agents now operate the platform 24/7 generating video content
- Limitations include groupthink, inconsistent video quality, and news selection bias
