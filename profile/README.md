# DataCore Vietnam

Open infrastructure for Vietnamese financial data.

DataCore builds the data layer Vietnamese capital markets have been missing: clean catalogs, alternative data, MCP-native AI access, and the SDKs to make it all usable from any language and any agent.

This GitHub organisation hosts our open-source ecosystem. Everything here is MIT-licensed unless noted otherwise.

## Repositories

### SDKs and tooling

| Repo | Language | What it does |
|---|---|---|
| [datacore-python](https://github.com/DataCore-VietNam/datacore-python) | Python | Official Python SDK. Pandas-first. Async support. Local parquet cache. |
| [datacore-r](https://github.com/DataCore-VietNam/datacore-r) | R | Official R client. Tibble-native. httr2-based. |
| [datacore-js](https://github.com/DataCore-VietNam/datacore-js) | TypeScript | Official JS / TS SDK. ESM. Works in Node, Deno, Bun, and browsers. |
| [datacore-cli](https://github.com/DataCore-VietNam/datacore-cli) | Python | Terminal interface - search, sample, download, configure. |
| [datacore-cookbook](https://github.com/DataCore-VietNam/datacore-cookbook) | Jupyter | End-to-end notebooks: VN30 screeners, factor investing, alt-data. |

### Quant infrastructure

| Repo | What it does |
|---|---|
| [vn-market-calendar](https://github.com/DataCore-VietNam/vn-market-calendar) | HOSE / HNX / UPCOM trading calendar - holidays 2018-2027, sessions, tick sizes. |
| [vn-corporate-actions](https://github.com/DataCore-VietNam/vn-corporate-actions) | Splits, dividends, bonuses, rights - clean backward-adjusted price series. |
| [vn-financial-terms](https://github.com/DataCore-VietNam/vn-financial-terms) | Bilingual VN-EN glossary - 340+ accounting, tax, banking, and markets terms. |

### Catalog and specifications

| Repo | What it does |
|---|---|
| [datacore-catalog-spec](https://github.com/DataCore-VietNam/datacore-catalog-spec) | Open specification for describing Vietnamese datasets in YAML. |

### Curated lists

| Repo | What it does |
|---|---|
| [awesome-vietnam-finance-data](https://github.com/DataCore-VietNam/awesome-vietnam-finance-data) | Data sources, libraries, and tools for Vietnamese financial markets. |

## Quick start

```bash
pip install datacore
export DATACORE_API_KEY=dc_...
```

```python
from datacore import Client

dc = Client()
vn30 = dc.dataset("equity.vn30.daily").to_pandas(start="2024-01-01")
```

Get a free API key at [datacore.vn](https://datacore.vn).

## Contributing

PRs welcome across all repos. Each repo has its own CONTRIBUTING.md. All contributions are licensed under each repo's license (MIT unless stated).

## Contact

Website: [datacore.vn](https://datacore.vn)

LinkedIn: [DataCore VietNam](https://linkedin.com/company/datacore-vietnam)

Issues: open one in the relevant repo

Email: contact@datacore.vn

Built in Vietnam.
