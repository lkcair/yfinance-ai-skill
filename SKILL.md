name: Financial Data Pull
description: >
  Quickly access reliable financial data and analytics. This skill connects to
  Yahoo Finance (56+ tools) to fetch real-time stock quotes, crypto and forex
  rates, commodity prices, company financials, earnings and analyst data, ETF and
  fund holdings, SEC filings, and breaking market news. Designed for fast
  lookups or deeper analysis, it integrates smoothly into your workflow.

metadata:
  openclaw:
    requires:
      bins:
        - python3

auto_route:
  # Stocks & Quotes
  - triggers: ["price", "stock price", "quote", "ticker", "shares of", "how much is", "stock data", "market price", "share price", "for stock"]
    tool: "get_stock_price"
  - triggers: ["compare stocks", "stock comparison", "vs", "versus", "side by side"]
    tool: "compare_stocks"
  - triggers: ["fast info", "quick info", "key metrics", "stock metrics"]
    tool: "get_fast_info"

  # Crypto
  - triggers: ["crypto price", "crypto", "cryptocurrency", "bitcoin", "btc", "ethereum", "eth", "dogecoin", "solana", "tether", "usdt"]
    tool: "get_crypto_price"

  # Forex
  - triggers: ["forex", "exchange rate", "currency", "fx rate", "convert currency", "currency pair"]
    tool: "get_forex_rate"

  # Commodities
  - triggers: ["commodity price", "commodity", "gold price", "oil price", "crude", "silver", "copper"]
    tool: "get_commodity_price"

  # Company Info
  - triggers: ["company info", "company profile", "about company", "tell me about", "what does", "company description"]
    tool: "get_company_info"
  - triggers: ["officers", "executives", "management", "ceo", "cfo", "insider roster", "who runs"]
    tool: "get_company_officers"
  - triggers: ["company overview", "overview", "full overview", "company details"]
    tool: "get_company_overview"
  - triggers: ["major holders", "institutional holders", "who owns", "shareholders", "top shareholders"]
    tool: "get_major_holders"

  # Financials & Fundamentals
  - triggers: ["balance sheet", "assets", "liabilities", "financial health"]
    tool: "get_balance_sheet"
  - triggers: ["cash flow", "free cash flow", "cash flows"]
    tool: "get_cash_flow"
  - triggers: ["income statement", "profit and loss", "p&l", "revenue breakdown", "earnings breakdown"]
    tool: "get_income_statement"
  - triggers: ["financial summary", "financials", "financial overview", "fundamentals"]
    tool: "get_financial_summary"
  - triggers: ["key ratios", "ratios", "p/e", "p/b", "valuation", "yield", "financial ratios"]
    tool: "get_key_ratios"

  # Earnings & Estimates
  - triggers: ["earnings history", "earnings", "quarterly earnings", "annual earnings", "historical earnings"]
    tool: "get_earnings_history"
  - triggers: ["earnings calendar", "upcoming earnings", "earnings dates", "when is earnings"]
    tool: "get_earnings_dates"
  - triggers: ["analyst estimates", "estimates", "forecasts", "eps forecast", "growth estimates", "growth projections"]
    tool: "get_analyst_estimates"
  - triggers: ["eps revisions", "earnings revisions", "eps trend", "earnings trend"]
    tool: "get_eps_revisions"

  # Dividends & Corporate Actions
  - triggers: ["dividends", "dividend history", "dividend yield"]
    tool: "get_dividends"
  - triggers: ["capital gains", "capital gains distributions"]
    tool: "get_capital_gains"
  - triggers: ["stock splits", "splits", "split history"]
    tool: "get_stock_splits"
  - triggers: ["corporate actions", "actions", "stock events"]
    tool: "get_corporate_actions"

  # Analysts & News
  - triggers: ["recommendations", "analyst recommendations", "buy sell hold", "analyst rating"]
    tool: "get_analyst_recommendations"
  - triggers: ["upgrades", "downgrades", "rating changes"]
    tool: "get_upgrades_downgrades"
  - triggers: ["news", "stock news", "latest news", "headlines", "financial news"]
    tool: "get_stock_news"
  - triggers: ["analyst price targets", "price targets", "target price"]
    tool: "get_analyst_price_targets"

  # Funds & ETFs
  - triggers: ["fund holdings", "etf holdings", "top holdings", "what is in", "fund composition"]
    tool: "get_fund_holdings"
  - triggers: ["fund overview", "etf overview", "fund info", "etf info", "etf details"]
    tool: "get_fund_overview"
  - triggers: ["fund sector weights", "sector allocation", "fund allocation", "sector breakdown"]
    tool: "get_fund_sector_weights"

  # Historical & Comparison
  - triggers: ["historical data", "history", "historical", "price history", "historical prices", "chart data"]
    tool: "get_historical_data"
  - triggers: ["compare performance", "historical comparison", "performance comparison"]
    tool: "get_historical_comparison"
  - triggers: ["price on date", "price on", "what was the price on", "historical price on"]
    tool: "get_historical_price_on_date"

  # Market Indices & Status
  - triggers: ["market indices", "indices", "s&p 500", "dow jones", "nasdaq", "markets", "index performance"]
    tool: "get_market_indices"
  - triggers: ["market status", "is market open", "market hours", "trading hours"]
    tool: "get_market_status"
  - triggers: ["sector performance", "sector metrics", "sector trends"]
    tool: "get_sector_performance"

  # Other Tools
  - triggers: ["trending tickers", "trending stocks", "popular stocks", "what is trending"]
    tool: "get_trending_tickers"
  - triggers: ["options chain", "options", "calls and puts", "call options", "put options"]
    tool: "get_options_chain"
  - triggers: ["options expirations", "expiry dates", "options dates"]
    tool: "get_options_expirations"
  - triggers: ["sec filings", "filings", "10-k", "10-q", "8-k", "sec documents"]
    tool: "get_sec_filings"
  - triggers: ["peer analysis", "peers", "competitors", "peer comparison"]
    tool: "get_peer_comparison"
  - triggers: ["api status", "api health"]
    tool: "get_api_status"
  - triggers: ["isin lookup", "identifier lookup", "get isin"]
    tool: "get_isin"
  - triggers: ["validate ticker", "is ticker valid", "check ticker"]
    tool: "validate_ticker"
  - triggers: ["search ticker", "find ticker", "ticker lookup", "symbol search"]
    tool: "search_ticker"
  - triggers: ["self test", "run tests", "validate tools"]
    tool: "run_self_test"

