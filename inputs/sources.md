# Sources — AI News Digest

Format: `name | url | type | per_run_cap`

## Feeds

| Name | URL | Type | Cap |
|---|---|---|---|
| Hacker News front page | https://hacker-news.firebaseio.com/v0/topstories.json | json-api | 30 |
| Hacker News AI tag | https://hn.algolia.com/api/v1/search_by_date?tags=story&query=AI | json-api | 30 |
| ArXiv cs.AI new | http://export.arxiv.org/rss/cs.AI | rss | 20 |
| ArXiv cs.CL new | http://export.arxiv.org/rss/cs.CL | rss | 20 |
| TechCrunch AI | https://techcrunch.com/category/artificial-intelligence/feed/ | rss | 20 |
| The Verge AI | https://www.theverge.com/rss/ai-artificial-intelligence/index.xml | rss | 20 |
| Simon Willison weblog | https://simonwillison.net/atom/everything/ | atom | 15 |
| Import AI (Jack Clark) | https://jack-clark.net/feed/ | rss | 10 |

## Exclude

Stories matching these patterns are dropped before clustering:
- Headlines containing: "will AI", "the rise of AI", "what is AI"
- Sponsored / #ad content
- Pure funding announcements under $10M
- Tweets (unless the account is on the allow-list below)

## Allow-list for social

Only include social-media links from these accounts:
- @karpathy, @sama, @miramurati, @sundarpichai
- @AnthropicAI, @OpenAI, @GoogleDeepMind
