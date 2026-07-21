# MayStreet (maystreet)

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
