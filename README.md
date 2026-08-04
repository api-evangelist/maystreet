# MayStreet (maystreet)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

MayStreet is a low-latency market data infrastructure vendor founded in 2012 and acquired by London Stock Exchange Group (LSEG) in May 2022, with maystreet.com now redirecting into LSEG's data feeds pages. The company captures full-depth exchange feeds in raw PCAP form across 300+ venues and sells them through the Bellport feed handler (C++ library, on-premises or managed), a 20+ petabyte Market Data Lake of historical tick data (PCAP/Parquet queried via Athena SQL and the Medusa Python client), the cloud Analytics Workbench (JupyterLab), and the High Performance Query (HPQ) streaming WebSocket API for near-time data. Access is sales-gated and entitlement-managed with no self-serve signup or public developer portal; the public API surface that exists is documented through example "springboard" repositories on the MayStreet GitHub organization rather than a docs site.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/maystreet/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/maystreet/refs/heads/main/apis.yml)

## Tags

- Financial
- Market Data
- Real-Time
- Trading
- Low Latency
- Tick Data
- Order Book
- Equities
- Options
- Feed Handlers
- PCAP

## Timestamps

- **Created:** 2026-07-21
- **Modified:** 2026-07-21

## APIs

### MayStreet High Performance Query (HPQ) API

Low-latency, near-time market data query API delivered as a streaming WebSockets service so clients can process arbitrarily-sized result sets frame-by-frame without pagination. Publicly documented only through the workbench-hpq-springboard example notebooks and hpq.py client on GitHub, which name the UAT endpoint wss://mdx.uat.maystreet.com (the production mdx.maystreet.com host resolves in DNS but is entitlement-gated and not publicly reachable). Access requires a MayStreet/LSEG Analytics Workbench entitlement.

- **Human URL:** [https://github.com/maystreet/workbench-hpq-springboard](https://github.com/maystreet/workbench-hpq-springboard)
- **Base URL:** `wss://mdx.uat.maystreet.com`

#### Tags

- Market Data
- WebSocket
- Streaming
- Tick Data
- Near-Time

#### Properties

- [Documentation](https://github.com/maystreet/workbench-hpq-springboard)

### MayStreet Market Data Lake Query API

Query access to MayStreet's 20+ petabyte Market Data Lake of historical exchange data captured as PCAP and converted to Parquet, exposed as Athena SQL plus a growing set of client functions through the Medusa2 Python client library inside Analytics Workbench. The Medusa client also reaches Refinitiv Tick History and Machine Readable News History stores backed by Google BigQuery. Publicly documented only via springboard example repositories on GitHub; no public REST endpoint or self-serve access is documented.

- **Human URL:** [https://github.com/maystreet/workbench-data-lake-springboard](https://github.com/maystreet/workbench-data-lake-springboard)

#### Tags

- Market Data
- Historical
- Tick Data
- SQL
- Python

#### Properties

- [Documentation](https://github.com/maystreet/workbench-data-lake-springboard)
- [Documentation](https://github.com/maystreet/workbench-medusa-springboard)

## Common Properties

- [Website](https://maystreet.com/)
- [GitHub Organization](https://github.com/maystreet)
- [LinkedIn](https://www.linkedin.com/company/maystreet)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
