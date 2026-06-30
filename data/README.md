# Net Value History

`nav-history.jsonl` is one JSON object per line.

Example:

```json
{"date":"2026-06-30","portfolio_id":"default","portfolio_name":"默认组合","unit_nav":1.0000,"total_assets":1000000}
```

The scheduled collector is:

```bash
./scripts/collect-nav-from-mcp.sh
```

It is intended to run at 15:00 on trading days and append one JSONL record after calling the portfolio-management MCP through the PM Agent.
