# Zen Goggles

Curated [Brave Search Goggles](https://search.brave.com/goggles) for an indie-web-first search experience.

Powered by [Brave Search](https://brave.com/search/) and its open [Goggles](https://search.brave.com/goggles) re-ranking system — one of the few search engines that gives users real control over their results.

## Philosophy

The modern web is dominated by SEO farms, walled gardens, and corporate mega-sites that outrank original, independent content. These goggles fight back by:

- **Downranking** corporate noise, content farms, paywalled sites, and ad-heavy aggregators
- **Boosting** independent blogs, personal sites, small communities, open access research, and non-profit knowledge sources
- **Curating** subject-specific allowlists of the best free-to-read sources in each field

## Goggles

| Goggle | Type | Description |
|--------|------|-------------|
| `zen_default` | Re-rank | Indie-web base layer. Applied to all general searches. Downranks corporate/SEO, boosts indie voices. |
| `academic` | Allowlist | Open access research only — preprints, OA journals, government, universities. No paywalled publishers. |
| `code` | Allowlist | Developer resources — docs, repos, Q&A, indie dev blogs. Primary sources over corporate marketing. |

## Usage

These goggles work with the [Brave Search API](https://brave.com/search/api/) via the `goggles_id` parameter:

```
GET https://api.search.brave.com/res/v1/web/search
  ?q=your+query
  &goggles_id=https://raw.githubusercontent.com/wakingbuddhas/zen-goggles/main/zen_default.goggle
```

Or use them with [Zen Notes](https://github.com/wakingbuddhas/zen-notes) where they're applied automatically.

## Contributing

PRs welcome — especially for new subject goggles and domain additions to existing ones. See the [Brave Goggles documentation](https://search.brave.com/goggles) for syntax reference.

## Acknowledgments

Built on [Brave Search](https://brave.com/search/) and the [Goggles](https://search.brave.com/goggles) open re-ranking system. Brave is building one of the few truly independent search indexes, and Goggles give users the power to shape their own search experience. We're grateful for both.
