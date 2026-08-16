# Wiki Operations

**Summary**: The core lifecycle operations executed on an LLM Wiki: Ingest, Query, and Lint.

**Sources**: `raw/index.md`

**Last updated**: 2026-08-16

---

## The Three Core Operations

Operating an LLM Wiki centers around three complementary workflows: **Ingest**, **Query**, and **Lint** (source: index.md).

```
 ┌─────────────┐       ┌─────────────┐       ┌─────────────┐
 │   INGEST    │       │    QUERY    │       │    LINT     │
 │ Add sources │  ──►  │ Explore &   │  ──►  │ Audit &     │
 │  & update   │       │  file back  │       │ health-check│
 └─────────────┘       └─────────────┘       └─────────────┘
```

---

## 1. Ingest Workflow

Triggered when a new source document is deposited into the `raw/` directory (source: index.md).

1. **Read**: The LLM reads the complete raw source document (source: index.md).
2. **Discuss**: The LLM surfaces key takeaways and discusses points of emphasis with the human before writing (source: index.md).
3. **Summarize**: Create a dedicated source summary page in the wiki (source: index.md).
4. **Update Entities & Concepts**: Create or update relevant concept pages across the wiki, adding new details or noting conflicting perspectives (source: index.md). A single source frequently touches 10–15 pages (source: index.md).
5. **Cross-Reference**: Insert internal `[[wiki-links]]` across related pages (source: index.md).
6. **Update Index**: Add new pages and brief descriptions to `wiki/index.md` (source: index.md).
7. **Log**: Record an entry in `wiki/log.md` with timestamp and modifications (source: index.md).

---

## 2. Query Workflow

Triggered when the user asks a question against the accumulated knowledge base (source: index.md).

1. **Locate**: The LLM checks `wiki/index.md` first to identify candidate pages rather than scanning all files (source: index.md).
2. **Synthesize**: The LLM reads the identified pages and synthesizes a cited response (source: index.md).
3. **Compound**: If the answer produces novel insights, structured comparisons, or valuable frameworks, the output is filed back into the wiki as a new Markdown page (source: index.md).

---

## 3. Lint Workflow

Periodic health checks to ensure structure, coherence, and accuracy across the wiki (source: index.md).

- **Contradiction Detection**: Flags conflicting claims across different sources and pages (source: index.md).
- **Orphan Page Identification**: Detects pages with zero inbound links (source: index.md).
- **Missing Concepts**: Identifies important terms mentioned in text that lack dedicated concept pages (source: index.md).
- **Superseded Claims**: Flags outdated assertions that newer sources have revised (source: index.md).
- **Research Gaps**: Suggests new questions to explore and external sources to fetch (source: index.md).

---

## Related pages

- [[llm-wiki-concept]]
- [[persistent-compounding-wiki]]
- [[three-layer-architecture]]
- [[human-llm-division-of-labor]]
