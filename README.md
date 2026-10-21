# yfinance-ai skill (`@lkcair/stocks`)

**Thousands of downloads on ClawHub.** The OpenClaw skill for [yfinance-ai](https://github.com/lkcair/yfinance-ai): 68 Yahoo Finance tools for stocks, ETFs, crypto, forex and commodities, from prices and fundamentals to analyst estimates, options, holders and market-wide calendars.

## Install

```bash
openclaw skills install @lkcair/stocks
```

Skill page: [clawhub.ai/lkcair/stocks](https://clawhub.ai/lkcair/stocks). The agent follows [SKILL.md](SKILL.md): a one-time setup in its own virtual environment (hash-pinned `requirements.txt`), then every function runs with one command through `scripts/cli.py`.

## Also available

- **MCP server** (Claude, Cursor, VS Code, any MCP client): `uvx yfinance-ai@latest`, see [yfinance-ai-mcp](https://github.com/lkcair/yfinance-ai-mcp)
- **OpenWebUI tool**, thousands of downloads: see [yfinance-ai](https://github.com/lkcair/yfinance-ai)
- **SEC filings skill**: `openclaw skills install @lkcair/sec`

Powered by [yfinance-ai](https://github.com/lkcair/yfinance-ai). MIT-0. Data from Yahoo Finance, may be delayed; not investment advice.
