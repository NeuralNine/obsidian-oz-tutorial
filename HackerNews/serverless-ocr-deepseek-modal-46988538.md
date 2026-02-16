---
title: "Rolling your own serverless OCR in 40 lines of code"
url: "https://christopherkrapu.com/blog/2026/ocr-textbooks-modal-deepseek/"
hn_id: 46988538
hn_url: "https://news.ycombinator.com/item?id=46988538"
date: 2026-02-16
tags: [ai, deep-learning, ocr, deepseek, modal, serverless, tutorial]
source: hackernews
---

# Summary

The author needed to make their copy of Gelman's Bayesian Data Analysis textbook searchable for a statistics-focused agent. Rather than using expensive commercial OCR tools with usage limits, they built a serverless solution using DeepSeek's open OCR model and Modal's serverless compute platform.

Modal enables running Python code on cloud infrastructure with GPU access, paying only for seconds used. The approach involves deploying a FastAPI server that accepts images and returns markdown text. DeepSeek's OCR model handles mathematical notation well—crucial for academic textbooks.

The implementation uses batched inference for efficiency, processing multiple pages in single forward passes through the model. Key optimizations include rendering pages at 2x resolution for better accuracy on small text and mathematical subscripts, and using deterministic output (temperature=0.0) for reproducibility.

For BDA's ~600 pages, processing takes about 45 minutes on an A100 and costs around $2. The output is markdown files with page markers, enabling grep searches, pasting sections into Claude for explanation, and building proper search indexes.

The OCR quality on mathematical content is "surprisingly good" with nearly all equations coming through intact. The setup is reusable for any PDF—course notes, papers, or other textbooks.

## Key Takeaways
- DeepSeek released an open OCR model with strong mathematical notation handling
- Modal provides serverless GPU compute with pay-per-second pricing
- Batched inference dramatically improves throughput
- 2x resolution rendering improves accuracy on small text
- Full textbook (~600 pages) can be processed for ~$2
