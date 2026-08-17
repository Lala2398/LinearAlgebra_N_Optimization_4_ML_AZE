# Persistent Compounding Wiki

**Summary**: The foundational concept of building an evolving, interlinked knowledge base that accumulates structured knowledge over time rather than relying on ephemeral RAG retrieval.

**Sources**: `raw/index.md`

**Last updated**: 2026-08-16

---

## Persistent Wiki vs. Traditional RAG

Most modern AI document workflows rely on standard Retrieval-Augmented Generation (RAG), where raw chunks are retrieved dynamically when a prompt is issued (source: index.md). While functional, standard RAG suffers from fundamental limitations:
- **No Accumulation**: The model rediscovers context from scratch on every question (source: index.md).
- **Shallow Synthesis Across Many Documents**: Complex queries spanning multiple sources require fragile real-time aggregation rather than built-up synthesis (source: index.md).
- **Ephemerality**: Valuable comparisons, answers, and connections disappear into chat logs after the session ends (source: index.md).

In contrast, a **persistent compounding wiki** compiles information into structured Markdown files that sit between the user and raw data (source: index.md). 

## How Knowledge Compounds

1. **Incremental Updates**: As new sources are ingested, existing entity and concept pages are modified to reflect new facts, refine summaries, or highlight contradictions (source: index.md).
2. **Associative Trails & Cross-References**: Wiki-links (`[[page-name]]`) establish persistent links between related entities and ideas (source: index.md).
3. **Query Feedback Loop**: High-value answers, comparative tables, and newly discovered connections generated during Q&A are filed back into the wiki as permanent pages (source: index.md).

## Example Use Cases

The persistent compounding wiki approach applies across diverse domains (source: index.md):
- **Deep Research**: Formulating and evolving a thesis across hundreds of papers over months (source: index.md).
- **Personal Knowledge Management**: Tracking health, psychology, journal entries, and personal development over time (source: index.md).
- **Book Companions & Fan Wikis**: Building comprehensive wikis for dense texts (similar to Tolkien Gateway) with characters, themes, and plot threads (source: index.md).
- **Team Knowledge Bases**: Organizing Slack threads, customer transcripts, and project specifications without manual documentation fatigue (source: index.md).

## Related pages

- [[llm-wiki-concept]]
- [[three-layer-architecture]]
- [[wiki-operations]]
- [[human-llm-division-of-labor]]
