# Agentic Context Engineering for Reliable LLM Tool-Calling

**Georgia Tech · CS 7643 Conversational AI · Spring 2026**

Authors: Agam Saraf, collaborators

---

## Overview

This project introduces a **3-stage Dynamic Context Engineering (DCE)** framework that significantly improves the reliability of Large Language Model tool-calling.

### Key Results

| Method | Tool-Selection Accuracy | Improvement |
|--------|------------------------|-------------|
| Static RAG (baseline) | ~72% | — |
| **DCE Framework (ours)** | **~82%** | **+10%** |

Benchmarked against DeepSeek-V3.1 on the [Berkeley Function-Calling Leaderboard (BFCL)](https://gorilla.cs.berkeley.edu/leaderboard.html).

---

## Architecture: 3-Stage Pipeline
*See `Final_Report.pdf` and `ACE_Poster.pdf` for complete details.*

1. **Context Retrieval** — Key-value vector DB indexes available API specs
2. **Agentic Reasoning** — LLM agent reasons over retrieved tool candidates
3. **Reflector-Curator Feedback Loop** — Self-correcting mechanism where failed tool calls trigger context refinement

## Author
**Agam Saraf** — Georgia Institute of Technology
