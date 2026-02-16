---
title: "Apple open-sources FoundationDB"
url: "https://www.foundationdb.org/blog/foundationdb-is-open-source/"
hn_id: "16877395"
hn_url: "https://news.ycombinator.com/item?id=16877395"
date: 2026-02-16
topic: "open source"
tags: [research, open-source, apple, database, foundationdb, distributed-systems]
source: hackernews
points: 2136
---

# Summary

In April 2018, Apple made a surprise announcement by open-sourcing FoundationDB, a distributed database they had acquired in 2015. This was notable because Apple is traditionally one of the most secretive tech companies, rarely contributing to open source outside of required projects like WebKit and Darwin.

FoundationDB is a multi-model database with a unique architecture that provides ACID transactions across a distributed cluster. It's designed to be a "database of databases" - a lower-level transactional key-value store upon which other database models (document, graph, relational) can be built. The database had been taken offline after Apple's acquisition, leading many to assume it would remain internal.

The open-sourcing of FoundationDB was received enthusiastically by the database community. The technology is known for its rigorous approach to correctness, including simulation testing that can exercise years of runtime in minutes. Apple uses FoundationDB internally for iCloud and other services, demonstrating its production-readiness at massive scale.

The decision gave developers access to enterprise-grade distributed database technology that had previously been proprietary. It also signaled a subtle shift in Apple's approach to open source, though the company remains far less open than competitors like Google, Microsoft, or Meta.

## Key Points
- Apple open-sourced FoundationDB in April 2018
- FoundationDB provides ACID transactions in a distributed database
- Had been taken offline after Apple's 2015 acquisition
- Used internally by Apple for iCloud and other services
- Notable for rigorous simulation testing methodology

## Relevance to open source
Apple's decision to open-source FoundationDB was surprising given the company's secretive culture. It provided the community with production-proven distributed database technology and demonstrated that even Apple sees value in open-source contributions. The project continues to be actively developed and used in production by multiple organizations.
