# Sorsa

Real-time X (Twitter) data API providing developers access to tweets, profiles, search, mentions, lists, communities, engagement verification, and Sorsa Score crypto-influence analytics across **40 REST endpoints**. Marketed as an affordable alternative to the official X API. Formerly Tweetscout.

- **Provider:** Sorsa Labs
- **Website:** https://sorsa.io/
- **Documentation:** https://docs.sorsa.io/
- **APIs.json:** https://api.sorsa.io/apis.json
- **Status Page:** https://uptime.sorsa.io/status/v3
- **Discord:** https://discord.com/invite/uwAefKCj7X
- **Contact:** contacts@sorsa.io
- **api-search issue:** [#21](https://github.com/api-search/network/issues/21)

## APIs

### Sorsa API v3

- **Base URL:** `https://api.sorsa.io/v3`
- **Authentication:** `ApiKey` HTTP header
- **Format:** JSON, REST
- **Pagination:** cursor (`next_cursor`)
- **OpenAPI:** [`openapi/sorsa-openapi.yml`](openapi/sorsa-openapi.yml)
- **Swagger source:** https://api.sorsa.io/v3/swagger.json
- **API reference:** https://docs.sorsa.io/api-reference-guide
- **Quickstart:** https://docs.sorsa.io/quickstart
- **Error codes:** https://docs.sorsa.io/error-codes
- **Versioning:** https://docs.sorsa.io/base-url-and-versioning

## Tags

`Twitter` · `X` · `Social Media` · `Data Extraction` · `Real-Time` · `Crypto`

## Pricing

| Plan | Monthly Requests | Price | Effective Per-Request | Rate Limit |
|---|---|---|---|---|
| Starter | 10,000 | $49 | $0.0049 | 20 req/s |
| Pro | 100,000 | $199 | $0.00199 | 20 req/s |
| Enterprise | 500,000 | $899 | $0.0018 | 20 req/s |
| Custom | negotiated | contact | negotiated | >=20 req/s |

Source: https://docs.sorsa.io/pricing · Sales: sales@sorsa.io

## Rate Limits

- **20 requests per second, per API key**, applied universally across every endpoint.
- Breach returns **HTTP 429**. No `Retry-After` or `x-ratelimit-*` headers are emitted.
- Recommended client mitigation: fixed 50 ms delay between requests, or reactive retry on 429.
- Live quota state is available via `GET /key-usage-info` (returns total, remaining, and expiry).

Source: https://docs.sorsa.io/rate-limits

## Endpoints (40)

| Tag | Method | Path | Summary |
|---|---|---|---|
| Users Data | GET | /info | User Profile |
| Users Data | GET | /info-batch | User Profile (Batch) |
| Users Data | GET | /about | Account About Info |
| Users Data | GET | /followers | Followers |
| Users Data | GET | /follows | Following |
| Users Data | GET | /verified-followers | Verified Followers |
| Tweets | POST | /tweet-info | Tweet Data |
| Tweets | POST | /tweet-info-bulk | Tweet Data (Batch) |
| Tweets | POST | /article | Article Data |
| Tweets | POST | /user-tweets | User Tweets |
| Tweets | POST | /comments | Tweet Comments |
| Tweets | POST | /quotes | Quote Tweets |
| Tweets | POST | /retweeters | Retweeters List |
| Tweets | GET | /trends | Trends List |
| Search | POST | /search-tweets | Search Tweets |
| Search | POST | /search-users | Search Users |
| Search | POST | /mentions | Search Mentions |
| Search | GET | /place | Place Information |
| Lists | GET | /list-tweets | List Tweets |
| Lists | GET | /list-members | List Members |
| Lists | GET | /list-followers | List Followers |
| Community | POST | /community-tweets | Community Tweets |
| Community | POST | /community-members | Community Members |
| Community | POST | /community-search-tweets | Search Community Tweets |
| Verification | POST | /check-follow | Check Follow |
| Verification | GET | /check-comment | Check Comment |
| Verification | POST | /check-retweet | Check Retweet |
| Verification | POST | /check-quoted | Check Quote or Retweet |
| Verification | POST | /check-community-member | Check Community Membership |
| Sorsa Info (Crypto) | GET | /score | Sorsa Score |
| Sorsa Info (Crypto) | GET | /score-changes | Sorsa Score Changes |
| Sorsa Info (Crypto) | GET | /followers-stats | Follower Category Stats |
| Sorsa Info (Crypto) | GET | /top-followers | Top 20 Followers by Score |
| Sorsa Info (Crypto) | GET | /top-following | Top 20 Following by Score |
| Sorsa Info (Crypto) | GET | /new-followers-7d | New Followers (7 Days) |
| Sorsa Info (Crypto) | GET | /new-following-7d | New Following (7 Days) |
| Technical | GET | /username-to-id/{user_handle} | Convert Username to User ID |
| Technical | GET | /id-to-username/{user_id} | Convert User ID to Username |
| Technical | GET | /link-to-id | Convert Profile Link to User ID |
| Technical | GET | /key-usage-info | API Key Usage |

## Generated Artifacts

| Type | Path | Notes |
|---|---|---|
| OpenAPI | [`openapi/sorsa-openapi.yml`](openapi/sorsa-openapi.yml) | OpenAPI 3.0.3, 40 paths, 52 schemas |
| JSON Schema | [`json-schema/`](json-schema/) | 8 entity schemas (user, follower, tweet, place, trend, etc.) |
| JSON Structure | [`json-structure/`](json-structure/) | 8 structure docs |
| JSON-LD | [`json-ld/sorsa-context.jsonld`](json-ld/sorsa-context.jsonld) · [`json-ld/sorsa-security-context.jsonld`](json-ld/sorsa-security-context.jsonld) | schema.org-aligned |
| Examples | [`examples/`](examples/) | 18 request/response and entity examples |
| Spectral Rules | [`rules/sorsa-rules.yml`](rules/sorsa-rules.yml) | API design conventions |
| Naftiko Capabilities | [`capabilities/`](capabilities/) | Shared + 3 workflows |
| Vocabulary | [`vocabulary/sorsa-vocabulary.yml`](vocabulary/sorsa-vocabulary.yml) | Operational dimensions |
| Plans / Pricing | [`plans/sorsa-plans-pricing.yml`](plans/sorsa-plans-pricing.yml) | API Commons Plans 0.1 |
| Rate Limits | [`rate-limits/sorsa-rate-limits.yml`](rate-limits/sorsa-rate-limits.yml) | API Commons Rate Limits 0.1 |
| FinOps | [`finops/sorsa-finops.yml`](finops/sorsa-finops.yml) | FOCUS-aligned (`reconciled: false`) |

## Use Cases

- **Crypto Twitter Intelligence** — track CT influencers, projects, and VC activity in real time.
- **Marketing Campaign Verification** — validate follows, retweets, quotes, comments, and Community membership for airdrops or contests.
- **Audience Geography Analysis** — combine `/about` and `/followers-stats` for audience composition mapping.
- **Competitor Analysis** — compare Sorsa Score, follower growth, and top-follower overlap between accounts.
- **Mention Monitoring** — engagement-filtered, date-bounded alerting on @-mentions.
- **Target Audience Discovery** — surface high-score followers and followings for outreach.
- **Migration from Official X API** — read-only drop-in at a fraction of the cost.

## Profiling Status

- **x-type:** `company`
- **Last profiled:** 2026-05-16
- **Pipeline:** Full company pipeline (steps 2-3 N/A — no public Sorsa GitHub org with code)
- **FinOps reconciled:** false (gated; requires customer portal access for full FOCUS export)
