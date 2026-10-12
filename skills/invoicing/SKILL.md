---
name: invoicing
description: Use when the user asks about Sqyre invoices, balances, overdue bills, or sending an invoice. Creating an invoice does not send it.
---

# Sqyre invoices

Use Sqyre MCP tools only. Never invent invoice numbers or amounts.

Find the invoice with `list_invoices`, `search_invoices`, `get_overdue_invoices`, or `get_unpaid_invoices`. Read it with `get_invoice`, `get_invoice_summary`, `get_invoice_balance`, and `get_invoice_payments`.

`create_invoice` saves a draft. `send_invoice` is separate. Do not send unless the user asked to send that invoice.

`mark_invoice_void` and `hard_delete_invoice` need an explicit yes that names the invoice. Re-read `get_invoice_balance` after a payment, void, or send, and report that balance.
