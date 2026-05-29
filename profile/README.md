# DataCore Vietnam

**Open infrastructure for Vietnamese financial data.**

DataCore builds the data layer Vietnamese capital markets have been missing — clean catalogs, alternative data, MCP-native AI access, and the SDKs to make it all usable from any language and any agent.

This GitHub organisation hosts our open-source ecosystem. Everything here is MIT-licensed unless noted otherwise.

---

## 📦 Repositories

### Flagship — SDKs & tooling

| Repo | Language | What it does |
|------|----------|--------------|
| [**datacore-python**](https://github.com/DataCore-VietNam/datacore-python) | Python | Official Python SDK. Pandas-first. Async support. Local parquet cache. MCP helpers. |
| [**datacore-r**](https://github.com/DataCore-VietNam/datacore-r) | R | Official R client. Tibble-native. `httr2`-based. Built for Tidy Finance VN. |
| [**datacore-js**](https://github.com/DataCore-VietNam/datacore-js) | TypeScript | Official JS / TS SDK. ESM. Works in Node, Deno, Bun, browsers, Edge. |
| [**datacore-cli**](https://github.com/DataCore-VietNam/datacore-cli) | Python | Terminal interface — search, sample, download, MCP config. |
| [**datacore-mcp-server**](https://github.com/DataCore-VietNam/datacore-mcp-server) | Python | MCP server — expose DataCore to Claude, Cursor, and any MCP-compatible agent. |
| [**datacore-cookbook**](https://github.com/DataCore-VietNam/datacore-cookbook) | Jupyter | End-to-end notebooks: VN30 screeners, factor investing, alt-data, agents. |

### Quant infrastructure

| Repo | What it does |
|------|--------------|
| [**vn-market-calendar**](https://github.com/DataCore-VietNam/vn-market-calendar) | HOSE / HNX / UPCOM trading calendar — holidays 2018-2027, sessions, tick sizes. |
| [**vn-corporate-actions**](https://github.com/DataCore-VietNam/vn-corporate-actions) | Splits, dividends, bonuses, rights — clean backward-adjusted price series. |
| [**vn-finance-ner**](https://github.com/DataCore-VietNam/vn-finance-ner) | Vietnamese financial NER — tickers, companies, money, percent, dates. |
| [**vn-financial-terms**](https://github.com/DataCore-VietNam/vn-financial-terms) | Bilingual VN-EN glossary — 340+ accounting, tax, banking, markets terms. |
| [**datacore-bloomberg-bridge**](https://github.com/DataCore-VietNam/datacore-bloomberg-bridge) | Bloomberg / Refinitiv / ISIN ↔ DataCore identifier mapping (220+ tickers). |

### Catalog & specifications

| Repo | What it does |
|------|--------------|
| [**datacore-catalog-spec**](https://github.com/DataCore-VietNam/datacore-catalog-spec) | Open spec for describing Vietnamese datasets in YAML — JSON-Schema validated. |

### Benchmarks & education

| Repo | What it does |
|------|--------------|
| [**vn-finance-llm-eval**](https://github.com/DataCore-VietNam/vn-finance-llm-eval) | Benchmark suite — 200+ tasks across 6 categories evaluating LLMs on Vietnamese financial reasoning. |
| [**learn-vn-quant**](https://github.com/DataCore-VietNam/learn-vn-quant) | Bilingual open course: quantitative finance with Vietnamese market data. |

### Curated lists

| Repo | What it does |
|------|--------------|
| [**awesome-vietnam-finance-data**](https://github.com/DataCore-VietNam/awesome-vietnam-finance-data) | Data sources, libraries, tools for Vietnamese financial markets. |
| [**awesome-mcp-finance**](https://github.com/DataCore-VietNam/awesome-mcp-finance) | MCP servers for finance, investing, and economic data. |

---

## 🚀 Quick start

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

---

## 🤖 Using DataCore from an AI agent

Drop this into your Claude Desktop config:

```python
from datacore import write_claude_desktop_config
write_claude_desktop_config(api_key="dc_...")
```

Or use [datacore-mcp-server](https://github.com/DataCore-VietNam/datacore-mcp-server) directly with any MCP-compatible agent — Claude, Cursor, VS Code Copilot, custom agents.

---

## 🤝 Contributing

PRs welcome across all repos. We're especially looking for:

- Bug reports and reproductions
- New dataset definitions in [datacore-catalog-spec](https://github.com/DataCore-VietNam/datacore-catalog-spec)
- New tasks in [vn-finance-llm-eval](https://github.com/DataCore-VietNam/vn-finance-llm-eval)
- Translations and new lessons in [learn-vn-quant](https://github.com/DataCore-VietNam/learn-vn-quant)
- Entries in our [Awesome lists](https://github.com/DataCore-VietNam/awesome-vietnam-finance-data)

Each repo has its own `CONTRIBUTING.md`. All contributions are licensed under each repo's license (MIT unless stated).

Org-wide community files:
- [Contributing guide](../CONTRIBUTING.md)
- [Code of conduct](../CODE_OF_CONDUCT.md)
- [Security policy](../SECURITY.md)
- [Support](../SUPPORT.md)

---

## 📫 Connect

- Website: [datacore.vn](https://datacore.vn)
- LinkedIn: [DataCore VietNam](https://vn.linkedin.com/company/datacore-vietnam)
- Issues: open one in the relevant repo
- Email: [contact@datacore.vn](mailto:contact@datacore.vn)

Built in Vietnam 🇻🇳
