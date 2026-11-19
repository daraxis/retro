# Public Daily Reflection Dataset (`data/`)

This directory archives the real, publicly shared daily reflection entries that power the live demo at [https://retro.darialan.com/demo](https://retro.darialan.com/demo).

- **Author & Initiator**: Daria
- **Upstream Public Profile**: [https://note.mowen.cn/user/-HvTNe8K6obWxOULo0Gtg](https://note.mowen.cn/user/-HvTNe8K6obWxOULo0Gtg)
- **Current Snapshot**: **91** daily entries (`2026-01-02` ~ `2026-11-14`)

## Files

- `retros.jsonl`: One JSON object per line, sorted ascending by `date`.
- `daily/YYYY-MM-DD.json`: Per-day formatted JSON files for direct browsing on GitHub.

## Schema

```json
{
  "date": "2026-01-02",
  "did": "- Action bullets for the day...",
  "thinking": "### Heading\n\nReflections and insights...",
  "sourceUrls": ["https://note.mowen.cn/detail/..."]
}
```

| Field | Type | Description |
| --- | --- | --- |
| `date` | `string` (`YYYY-MM-DD`) | Business date key (Asia/Shanghai). |
| `did` | `string` | Objective actions or milestones completed that day (may be empty if only thinking was logged). |
| `thinking` | `string` | Independent reflections, insights, bad/emotion/plan sections formatted in Markdown. |
| `sourceUrls` | `string[]` | Links back to the original public notes on Mowen. |

## Usage Note

All entries in this directory were originally written and published openly by the author. You are welcome to explore them for personal inspiration, Chinese RAG / Agent retrieval benchmarks, or reflection workflow research with attribution to the source profile.
