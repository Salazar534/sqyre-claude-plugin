---
name: quoting
description: Use when the user wants a Sqyre quote created, priced, sent, or checked. Creating a quote does not send it.
---

# Sqyre quotes

Use Sqyre MCP tools only. Never invent quote ids, line prices, or totals.

Resolve the client with `search_clients` before `create_quote`. Read an existing quote with `list_quotes`, `search_quotes`, `get_quote`, `get_quote_summary`, and `list_quote_line_items`.

`create_quote` saves a draft. `send_quote` is a second, explicit step. Do not send because the user only asked to write the quote.

After line changes, call `recalculate_quote` and then `get_quote` so the total you report is the one Sqyre stored. Use `generate_quote_pdf` only when the user asks for a PDF.

`approve_quote`, `mark_quote_accepted`, and `mark_quote_declined` need a clear yes for that quote. `convert_quote_to_invoice` and `create_invoice_from_quote` create a bill for the customer. Confirm before either one.
