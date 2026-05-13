# Super-paper skill

A Claude Code skill for deep reading academic papers from Zotero — producing Obsidian-compatible structured Markdown summaries (8 sections) and JSON Canvas visual logic flow boards.

Building a complete Obsidian + Zotero + Claude Code research workflow.

> [中文文档](README.zh.md)

## Features

Four-step workflow:

1. **Locate** — Search papers in Zotero by keyword, collection, or recently added
2. **Extract** — Fetch metadata, full text, and annotations with support for multiple PDF extractors
3. **Summarize** — Generate an 8-section structured Markdown summary (overview → background → method → experiments → conclusion → references)
4. **Visualize** — Auto-generate `.canvas` files for logic flow diagrams viewable in Obsidian Canvas

## Dependencies

Install the following skills before using Super-paper:

| Skill | Purpose |
|-------|---------|
| [zotero-cli-cc](https://github.com/AlaskGulf/zotero-cli-cc) | Zotero search & PDF extraction |
| [obsidian-markdown](https://github.com/AlaskGulf/obsidian-markdown) | Obsidian-compatible Markdown output |
| [obsidian-bases](https://github.com/AlaskGulf/obsidian-bases) | Dataview-compatible data tables |
| [json-canvas](https://github.com/AlaskGulf/json-canvas) | Obsidian Canvas generation |

## Installation

### Option 1: Clone to user skills directory

```bash
git clone https://github.com/AlaskGulf/super-paper.git ~/.claude/skills/Super-paper
```

### Option 2: Via Marketplace (once registered)

```bash
claude skills install super-paper
```

## Usage

Express your intent to read a paper in a Claude Code conversation:

```
Read and summarize the "Semantic Communication" paper from my Zotero library
```

Or invoke explicitly:

```
/super-paper analyze the most recently added paper
```

## Output

- `<paper-title>.md` — 8-section structured summary
- `<paper-slug>_logic.canvas` — Paper logic flow canvas
- `<paper-slug>_arch.canvas` (on demand) — Technical architecture canvas

## License

MIT
