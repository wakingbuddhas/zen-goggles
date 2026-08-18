# zen-goggles

A re-ranking filter for the [Brave Search API](https://search.brave.com/goggles).

`zen_default.goggle` is purely subtractive — it downranks noise and boosts nothing. Everything not listed keeps its natural ranking and rises as the listed sites fall.

| Weight | Downranked |
|---|---|
| 5 | Social walled gardens, SEO/content farms, affiliate review sites |
| 4 | Aggregators over originals, paywalled news, e-commerce, review/travel/job aggregators |
| 3 | Substack, YouTube, G2, Capterra |
| 2 | Large-vendor documentation |

## Use

```
&goggles_id=https://raw.githubusercontent.com/wakingbuddhas/zen-goggles/main/zen_default.goggle
```
