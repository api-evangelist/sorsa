# Sorsa (sorsa)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Sorsa Labs operates a real-time X (Twitter) data API providing developers access to tweets, profiles, search, mentions, lists, communities, engagement verification, and Sorsa Score crypto-influence analytics through 40 REST endpoints. It markets itself as an affordable alternative to the official X API and was formerly known as Tweetscout.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Twitter
- X
- Social Media
- Data Extraction
- Real-Time

## Timestamps

- **Created:** 2026-05-16
- **Modified:** 2026-05-19

## APIs

### Sorsa API v3

The Sorsa API v3 is a RESTful API exposing 40 endpoints for real-time X (Twitter) data: user profiles and About metadata, followers and following lists, tweet data (single and batch), articles, user timelines, comments, quotes, retweets, search of tweets and users, mentions, Twitter Spaces (Places), lists, communities, engagement and membership verification, Sorsa Score crypto-influence analytics, follower category breakdowns, and technical utilities (username/user-id conversion, profile-link parsing, API-key usage). Authentication uses a simple `ApiKey` header.

- **Human URL:** [https://docs.sorsa.io/](https://docs.sorsa.io/)
- **Base URL:** `https://api.sorsa.io/v3`

#### Tags

- Twitter
- X
- Social Media
- Real-Time
- Data Extraction
- Crypto

#### Properties

- [Documentation](https://docs.sorsa.io/)
- [API Reference](https://docs.sorsa.io/api-reference-guide)
- [Getting Started](https://docs.sorsa.io/quickstart)
- [Quickstart](https://docs.sorsa.io/quickstart)
- [Authentication](https://docs.sorsa.io/authentication)
- [Rate Limits](https://docs.sorsa.io/rate-limits)
- [Pricing](https://docs.sorsa.io/pricing)
- [Errors](https://docs.sorsa.io/error-codes)
- [Versioning](https://docs.sorsa.io/base-url-and-versioning)
- [Changelog](https://docs.sorsa.io/Migration-Guide)
- [A P Is J S O N](https://api.sorsa.io/apis.json)
- [OpenAPI](openapi/sorsa-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sorsa.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sorsa.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Swagger J S O N](https://api.sorsa.io/v3/swagger.json)
- [JSON Schema](json-schema/sorsa-user-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sorsa-follower-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sorsa-tweet-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sorsa-tweet-entity-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sorsa-top-follower-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sorsa-place-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sorsa-trend-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sorsa-community-user-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/sorsa-user-structure.json)
- [JSON Structure](json-structure/sorsa-follower-structure.json)
- [JSON Structure](json-structure/sorsa-tweet-structure.json)
- [JSON Structure](json-structure/sorsa-tweet-entity-structure.json)
- [JSON Structure](json-structure/sorsa-top-follower-structure.json)
- [JSON Structure](json-structure/sorsa-place-structure.json)
- [JSON Structure](json-structure/sorsa-trend-structure.json)
- [JSON Structure](json-structure/sorsa-community-user-structure.json)
- [JSON-LD](json-ld/sorsa-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/sorsa-security-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Example](examples/sorsa-info-example.json)
- [Example](examples/sorsa-tweet-info-example.json)
- [Example](examples/sorsa-tweet-info-bulk-example.json)
- [Example](examples/sorsa-search-tweets-example.json)
- [Example](examples/sorsa-mentions-example.json)
- [Example](examples/sorsa-followers-example.json)
- [Example](examples/sorsa-follows-example.json)
- [Example](examples/sorsa-score-example.json)
- [Example](examples/sorsa-check-follow-example.json)
- [Example](examples/sorsa-key-usage-info-example.json)
- [Example](examples/sorsa-user-example.json)
- [Example](examples/sorsa-follower-example.json)
- [Example](examples/sorsa-tweet-example.json)
- [Example](examples/sorsa-tweet-entity-example.json)
- [Example](examples/sorsa-top-follower-example.json)
- [Example](examples/sorsa-place-example.json)
- [Example](examples/sorsa-trend-example.json)
- [Example](examples/sorsa-community-user-example.json)

## Common Properties

- [Website](https://sorsa.io/)
- [Developer Portal](https://docs.sorsa.io/)
- [Documentation](https://docs.sorsa.io/)
- [A P Is J S O N](https://api.sorsa.io/apis.json)
- [Sign Up](https://app.sorsa.io/)
- [Login](https://app.sorsa.io/)
- [Console](https://app.sorsa.io/)
- [Pricing](https://docs.sorsa.io/pricing)
- [Plans](plans/sorsa-plans-pricing.yml)
- [Rate Limits](rate-limits/sorsa-rate-limits.yml)
- [Fin Ops](finops/sorsa-finops.yml)
- [Spectral Rules](rules/sorsa-rules.yml)
- [Vocabulary](vocabulary/sorsa-vocabulary.yml)
- [Status Page](https://uptime.sorsa.io/status/v3)
- [Support](https://docs.sorsa.io/support)
- [Contact](mailto:contacts@sorsa.io)
- [Discord](https://discord.com/invite/uwAefKCj7X)
- [Twitter](https://x.com/SorsaApp)
- [Glossary](https://docs.sorsa.io/use-cases-overview)
- [Best Practices](https://docs.sorsa.io/optimizing-api-usage)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)
- [L L Ms Txt](https://api.sorsa.io/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
**URL:** https://apievangelist.com/
