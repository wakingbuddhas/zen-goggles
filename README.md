# zen-goggles

Re-ranking filters for the [Brave Search API](https://search.brave.com/goggles).

| File | Effect |
|---|---|
| `zen_default.goggle` | Re-rank. Downranks social media, SEO/content farms, paywalled news, e-commerce, and affiliate review sites. Boosts personal blogs, indie communities, open reference, non-profit journalism, and open access research. |
| `academic.goggle` | Allowlist. Discards everything except open access research — preprints, OA journals, government, universities, libraries. |
| `code.goggle` | Allowlist. Discards everything except developer resources — official docs, repositories, package registries, Q&A, indie dev blogs. |

## Use

```
&goggles_id=https://raw.githubusercontent.com/wakingbuddhas/zen-goggles/main/zen_default.goggle
```
