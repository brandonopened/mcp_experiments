# mcp_experiments

A collection of small demo applications that consume data from MCP (Model Context Protocol) servers.

> **Demo notice.** These are demonstrations, not production tools. Data is sourced via [olyport.com](https://olyport.com/), which surfaces public datasets (BLS LAUS, O*NET, etc.) through MCP servers. Treat all outputs as directional.

## Demos

### `lane-county-employment/`
Single-page dashboard for Lane County, Oregon employment trends. Charts BLS county/state unemployment rate, employment, and labor force from Jan 2020 through Dec 2025, plus an O*NET-driven occupation watchlist (Bright Outlook vs. pressured roles).

Open `lane-county-employment/index.html` in a browser. No build step.

**Data sources**
- BLS LAUS series for Lane County (FIPS 41039) and Oregon — fetched via MCP at build time and embedded in the page.
- O*NET-SOC occupation profiles (description, skills, knowledge areas) and Bright Outlook flag — fetched via MCP.
- Numeric career-outlook and wage endpoints returned errors at fetch time and are intentionally omitted rather than fabricated.

## License

MIT
