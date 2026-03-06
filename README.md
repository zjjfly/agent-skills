# Agent Skills

A personal collection of custom skills for [Claude Code](https://claude.ai/code).

> [中文 README](README.zh.md)

## Installation

```bash
npx skills add zjjfly/agent-skills
```

## Skills

### draft-merger

Merges multiple drafts of the same document into one polished final version.

**Triggers on:** "merge these drafts", "combine these versions", "I have multiple drafts", "把这几份稿子合并", "合并稿子", or whenever multiple files are clearly different versions of the same content.

**Process:**
1. Reads and assesses all provided drafts, summarizing the strengths of each
2. Selects the strongest draft as the base (or uses your specified base)
3. Enriches the base with valuable content from other drafts — unique examples, stronger evidence, missing context
4. Polishes the merged result for coherence, consistency, and flow
5. Outputs the final merged document along with a **Merge Notes** section explaining key decisions

**Best for:** Documents, articles, reports, proposals — any text-based writing. Not intended for code or data file merging.
