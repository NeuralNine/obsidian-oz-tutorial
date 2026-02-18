---
title: "Advice, not control: the role of Remote Assistance in Waymo's operations"
url: "https://waymo.com/blog/?modal=short-advice-not-control-the-role-of-remote-assistance"
hn_id: 47055786
hn_url: "https://news.ycombinator.com/item?id=47055786"
date: 2026-02-18
tags: [ai, autonomous-vehicles, waymo, self-driving, robotics]
source: hackernews
---

# Summary

Waymo has published details about how their Remote Assistance system works, emphasizing a key distinction: remote operators provide "advice, not control" to their autonomous vehicles. This approach differs significantly from teleoperation systems where humans directly drive vehicles remotely.

In Waymo's system, when an autonomous vehicle encounters an unusual situation it cannot confidently handle, it can request assistance from a remote operator. The operator reviews the situation and provides guidance—such as suggesting the vehicle proceed, wait, or take an alternative route—but never takes direct control of steering, acceleration, or braking. The vehicle's onboard AI always remains in control of actual driving functions.

This design philosophy has important implications for safety and scalability. By keeping humans in an advisory role rather than a control role, Waymo avoids the latency and reliability issues that would come with remote driving. The vehicle can always respond instantly to its immediate environment, while leveraging human judgment for higher-level decision-making when needed.

The approach also reflects Waymo's confidence in their autonomous system's core driving capabilities while acknowledging that novel situations may benefit from human input. Remote operators are trained to provide contextual guidance rather than moment-to-moment driving instructions.

## Key Takeaways
- Waymo's Remote Assistance provides advice, never direct vehicle control
- Onboard AI always controls steering, acceleration, and braking
- This avoids latency issues associated with teleoperation
- Human operators help with unusual situations requiring contextual judgment
- Design reflects balance of AI capability and human oversight
