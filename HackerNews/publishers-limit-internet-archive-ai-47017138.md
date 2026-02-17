---
title: "News publishers limit Internet Archive access due to AI scraping concerns"
url: "https://www.niemanlab.org/2026/01/news-publishers-limit-internet-archive-access-due-to-ai-scraping-concerns/"
hn_id: 47017138
hn_url: "https://news.ycombinator.com/item?id=47017138"
date: 2026-02-17
tags: [ai, web-scraping, journalism, copyright, llm]
source: hackernews
---

# Summary

Major news publishers including The Guardian and The New York Times are limiting the Internet Archive's access to their content due to concerns that AI companies might scrape their articles via the nonprofit's repository of over one trillion webpage snapshots. The Guardian decided to limit access after access logs revealed the Internet Archive was a frequent crawler.

The Guardian has excluded itself from Internet Archive's APIs and filtered out article pages from the Wayback Machine's URLs interface (while homepages and topic pages remain). The head of business affairs expressed concern that AI businesses seeking structured databases of content might use the Archive's API to "suck out the IP."

The New York Times is actively "hard blocking" the Internet Archive's crawlers and has added archive.org_bot to its robots.txt file, stating that "the Wayback Machine provides unfettered access to Times content — including by AI companies — without authorization." The Financial Times blocks any bot trying to scrape paywalled content, including from OpenAI, Anthropic, Perplexity, and the Internet Archive.

Internet Archive founder Brewster Kahle responded that "if publishers limit libraries, like the Internet Archive, then the public will have less access to the historical record." The Archive has implemented rate-limiting and filtering mechanisms but doesn't disallow specific AI crawlers in its robots.txt. Analysis showed the Wayback Machine was ranked 187th most present in Google's C4 training dataset.

## Key Takeaways

- Guardian and NYT limiting Internet Archive access over AI concerns
- Publishers fear Archive's API is backdoor for AI training data scraping
- Internet Archive's repository contains 1+ trillion webpage snapshots
- Reddit also blocked Archive in August 2025 citing AI scraping
- Collateral damage to historical preservation in fight against AI scraping
