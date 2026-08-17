# Knowledge Base Tooling

**Summary**: Tooling, plugins, and environment integrations that enhance the LLM Wiki pattern, including Obsidian, search utilities, and presentation renderers.

**Sources**: `raw/index.md`

**Last updated**: 2026-08-16

---

## Editor and Environment: Obsidian

The LLM Wiki pattern works naturally with local-first Markdown editors like [Obsidian](https://obsidian.md) acting as the frontend IDE while the LLM acts as the programmer (source: index.md).

Key Obsidian capabilities and workflows:
- **Graph View**: Visualizes the topology of the wiki, revealing clusters, hub pages, and orphan nodes (source: index.md).
- **Obsidian Web Clipper**: Browser extension that converts web articles into clean Markdown directly for the `raw/` folder (source: index.md).
- **Local Attachment Downloading**: Setting attachment folders (e.g. `raw/assets/`) and binding a hotkey to download all embedded images locally preserves assets so links never rot and allow visual LLM inspection (source: index.md).
- **Dataview Plugin**: Enables dynamic SQL-like queries over Markdown frontmatter (tags, dates, categories) (source: index.md).
- **Marp Plugin**: Generates presentation slide decks directly from wiki markdown pages (source: index.md).

---

## Navigation & Search Infrastructure

As a wiki grows from dozens to hundreds or thousands of pages, navigational layers scale as follows (source: index.md):

1. **Table of Contents (`index.md`)**: A structured markdown catalog organized by category, sufficient for small to medium wikis (~100 sources) (source: index.md).
2. **Local Hybrid Search (`qmd`)**: A fast local search engine combining BM25 and vector search with on-device LLM re-ranking, accessible via CLI or MCP server (source: index.md).
3. **Version Control**: Tracking the entire wiki in a Git repository provides full version history, branching, and automated backup for free (source: index.md).

---

## Related pages

- [[llm-wiki-concept]]
- [[three-layer-architecture]]
- [[wiki-operations]]
