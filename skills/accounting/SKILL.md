---
name: accounting
description: Use when the user asks about Sqyre books, expenses, bills, accounts receivable, payments, or the accounting overview. Read records before changing them.
---

# Sqyre accounting

Use Sqyre MCP tools only. Never invent client ids, invoice ids, or dollar amounts.

Start with `get_current_user` if the organization is unclear, then `get_accounting_overview`.

Read with:

- `list_expenses`
- `list_bills`
- `get_accounts_receivable`
- `get_accounts_receivable_metrics`
- `list_payments`, `get_payment`, `get_invoice_payments`, `get_recent_payments`, `get_failed_payments`

`create_accounting_adjustment` changes the books. Show the amount, the account, and the reason, and wait for a yes before calling it.

Do not call `refund_payment` or `create_payment_charge` unless the user explicitly asked to refund or charge that payment. Re-read the invoice or bill after any write.
