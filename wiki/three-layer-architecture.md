# Three-Layer Architecture

**Summary**: The structural model of the LLM Wiki pattern consisting of raw sources, the persistent wiki markdown files, and the governing schema.

**Sources**: `raw/index.md`

**Last updated**: 2026-08-16

---

## The Three Layers

The LLM Wiki architecture separates concerns into three distinct layers (source: index.md):

```
┌──────────────────────────────────────────────────────────┐
│                   1. Raw Sources (raw/)                   │
│   Immutable ground truth (PDFs, notes, articles, clips)  │
└────────────────────────────┬─────────────────────────────┘
                             │
                             ▼
┌──────────────────────────────────────────────────────────┐
│                    2. The Wiki (wiki/)                   │
│    Compiled Markdown layer (concepts, entities, links)   │
│              Maintained entirely by the LLM              │
└────────────────────────────┬─────────────────────────────┘
                             │
                             ▼
┌──────────────────────────────────────────────────────────┐
│                   3. The Schema (CLAUDE.md)              │
│       Rules, conventions, and operational workflows      │
└──────────────────────────────────────────────────────────┘
```

### 1. Raw Sources (`raw/`)
- **Role**: Immutable ground truth (source: index.md).
- **Contents**: Unmodified primary sources including articles, research papers, data files, book chapters, and web clippings (source: index.md).
- **Permissions**: The LLM reads from raw sources but never modifies or deletes them (source: index.md).

### 2. The Wiki (`wiki/`)
- **Role**: The persistent synthesis layer (source: index.md).
- **Contents**: Markdown files including source summaries, concept pages, entity profiles, comparison tables, and indexes (source: index.md).
- **Permissions**: The LLM owns this layer completely—creating, updating, linking, and reorganizing files (source: index.md).

### 3. The Schema (`CLAUDE.md` / `AGENTS.md`)
- **Role**: The governance configuration for the LLM agent (source: index.md).
- **Contents**: Conventions for file naming, page formatting, citation standards, folder structure, and operational workflows (source: index.md).
- **Evolution**: Co-evolved by the human and the LLM over time as domain requirements evolve (source: index.md).

## Related pages

- [[llm-wiki-concept]]
- [[persistent-compounding-wiki]]
- [[wiki-operations]]
- [[knowledge-base-tooling]]
