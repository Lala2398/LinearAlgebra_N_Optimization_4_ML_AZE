# LLM Wiki Concept

**Summary**: An architectural pattern for building persistent, compounding personal knowledge bases using LLMs instead of stateless RAG queries.

**Sources**: `raw/index.md`

**Last updated**: 2026-08-16

---

## Overview

The **LLM Wiki** is a pattern designed to overcome the stateless limitations of conventional Retrieval-Augmented Generation (RAG) (source: index.md). Rather than repeatedly searching and synthesizing raw fragments from scratch on every query, an LLM incrementally compiles, cross-references, and maintains a structured Markdown knowledge base (source: index.md).

## Core Principles

- **Accumulation over Rediscovery**: Knowledge is extracted and compiled once, then continuously updated and refined as new sources arrive (source: index.md).
- **Persistent Compounding Artifact**: Every ingested document and answered question adds value to the network of pages, preserving associative trails, comparisons, and resolved contradictions (source: index.md).
- **Clear Division of Labor**: Humans focus on curation, high-level analysis, and critical questions, while the LLM handles maintenance, bookkeeping, cross-linking, and summarization (source: index.md).
- **Inspiration from the Memex**: Rooted in Vannevar Bush's 1945 vision of associative trails between documents, solved practically by having LLMs handle the maintenance burden that previously led to wiki abandonment (source: index.md).

## Related pages

- [[persistent-compounding-wiki]]
- [[three-layer-architecture]]
- [[wiki-operations]]
- [[knowledge-base-tooling]]
- [[human-llm-division-of-labor]]
