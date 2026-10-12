---
name: business-analysis
description: Use when the user wants Sqyre revenue, conversion, schedule utilization, or a comparison between two date ranges.
---

# Sqyre business numbers

Use Sqyre MCP tools only. Never estimate a total when a tool can return it.

Start with `get_business_summary` or `get_dashboard_summary`. Then use the narrower tool:

- `get_revenue_metrics`
- `get_quote_conversion_rate`
- `get_accounts_receivable_metrics`
- `get_schedule_utilization`
- `get_dashboard_metrics`
- `compare_date_ranges`
- `get_recent_activity`

Say which dates the tool used. If the user names a different range, call the tool again instead of scaling the previous number.
