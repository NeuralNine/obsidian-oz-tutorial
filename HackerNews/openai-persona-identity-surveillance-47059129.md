---
title: "OpenAI, the US government, and Persona built an identity surveillance machine"
url: "https://vmfunc.re/blog/persona/"
hn_id: 47059129
hn_url: "https://news.ycombinator.com/item?id=47059129"
date: 2026-02-18
tags: [ai, openai, privacy, surveillance, security-research]
source: hackernews
---

# Summary

Security researchers discovered concerning infrastructure connecting OpenAI, the identity verification company Persona, and US government systems. Through passive reconnaissance using public sources like Shodan and certificate transparency logs, they found dedicated servers with names like "openai-watchlistdb.withpersona.com" that appear to handle identity verification and screening operations.

The investigation uncovered 53 megabytes of unprotected source maps on what appears to be a FedRAMP government endpoint. The exposed codebase allegedly contains functionality for facial recognition watchlist comparisons, Suspicious Activity Reports (SARs) filed with FinCEN, and screening against categories including terrorism and espionage. The researchers found evidence of periodic re-screening of users.

The infrastructure breaks from Persona's normal Cloudflare-protected setup, using dedicated Google Cloud instances in Kansas City. The researchers emphasize that no systems were breached—all findings came from publicly accessible sources including DNS records, HTTP headers, and unauthenticated source maps served by the target servers.

## Key Takeaways

- Dedicated "watchlistdb" infrastructure connects OpenAI verification to government screening systems
- 53MB of unprotected source maps exposed full TypeScript codebase with screening algorithms
- Evidence of facial recognition comparisons against watchlist photos and periodic user re-screening
- Infrastructure bypasses normal Cloudflare protection, running on isolated Google Cloud instances
- Raises significant privacy concerns about AI platform identity verification practices
