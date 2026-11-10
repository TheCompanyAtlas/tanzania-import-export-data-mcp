# Tanzania Import Export Data MCP

**Tanzania Customs Data: Importers, Suppliers & HS Codes.** Tanzania import export data for your AI assistant. Search Tanzania customs shipment records, find importers and foreign suppliers, and break down trade by HS code, partner country and counterparty company, through the Model Context Protocol.

An AI-native alternative to Tanzania trade data from Panjiva, ImportGenius, Volza, Seair, TradeInt and ExportGenius: ask in plain language instead of exporting spreadsheets.

The MCP connection is provided by [The Company Atlas](https://thecompanyatlas.com). This repository does not run a separate server.

## Connect

```
https://thecompanyatlas.com/mcp/trade/tanzania
```

Add this URL as a custom MCP connector in Claude, ChatGPT, Cursor, or any MCP-compatible client. Sign in with Google when prompted.

- Transport: Streamable HTTP
- Auth: Google OAuth (sign in once, stays authorized)
- Free accounts get 50 credits per calendar month
- Defaults to Tanzania: the server tells your AI to filter on `TZ` unless you ask about another country

## Tanzania data coverage

- **Years:** 2024–2026
- **Records:** Import declarations: Tanzanian importer, foreign supplier, origin country, HS code, goods description, value, quantity, port and date.
- **Country code:** `TZ` (use `buyerCountry: "TZ"` for imports into Tanzania)
- **Common products:** refined fuel (HS 2710), wheat (HS 1001), coated steel (HS 7210), cars (HS 8703)

> Declared values are mostly in USD, some in EUR or TZS; check the currency field before totalling.

## Notable traders in the data

Companies that appear most often in recent Tanzania records (by number of declaration lines, not value):

**Importers**

- Said Salim Bakhresa & Company
- GBP Tanzania
- Puma Energy Tanzania
- Lodhia Industries
- ALAF Limited
- Geita Gold Mining

## Example prompts

- *"Who are the top importers of wheat (HS 1001) into Tanzania?"*
- *"What does Said Salim Bakhresa & Company import, and from which countries?"*
- *"List Tanzanian importers of refined fuel (HS 2710) in 2025"*
- *"Which suppliers ship mining equipment to Geita Gold Mining?"*
- *"Show recent import shipments for Lodhia Industries"*

## Tools

### Trade search

| Tool | Description |
|---|---|
| `Trade_search_trades` | Paginated customs shipment search: filter by HS code, buyer, seller, country, port, value and date range |
| `Trade_company_trade_volume_by_year` | Rank importers or exporters by declared value and line counts per year, with HS code and country filters |

### Trade analytics

| Tool | Description |
|---|---|
| `Trade_hs_code_breakdown` | For one company, import and export value by HS chapter, heading or subheading |
| `Trade_year_country_breakdown` | For one company, trade value by year and counterparty country |
| `Trade_partner_breakdown` | For one company, trade value by year and matched counterparty company |

### Company registry

| Tool | Description |
|---|---|
| `Company_search` | Search the global company registry by name or id, with optional country filter |
| `Company_get_by_id` | Full company profile by id |

## Keywords

Tanzania import data, Tanzania export data, Tanzania customs data, Tanzania shipment data, importers in Tanzania, Tanzania buyers and suppliers, HS code search, Tanzania customs data, TRA import data, importers in Tanzania, Dar es Salaam port shipments
