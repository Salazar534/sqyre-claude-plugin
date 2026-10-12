---
name: crm
description: Use when the user looks up, creates, or updates a Sqyre client, request, project, or client history. Search before creating a duplicate.
---

# Sqyre clients

Use Sqyre MCP tools only. Never invent ids, phone numbers, or balances.

Find the person first with `search_clients` or `resolve_client_by_phone`. If several people match, ask which one. Use `resolve_entity` when the name could be a client, project, quote, or invoice.

Read with `get_client`, `get_client_summary`, `get_client_projects`, `get_client_quotes`, `get_client_invoices`, `get_client_balance`, `get_client_timeline`, and `list_client_notes`.

Requests: `list_requests`, `search_requests`, `get_request`, `get_new_requests`, `get_stale_requests`. Create with `create_request` only after the client id is confirmed. `convert_request_to_quote` is a separate step from creating the request.

Projects: `list_projects`, `search_projects`, `get_project`, `get_project_summary`, `get_project_visits`. Confirm before `create_project`, `set_project_status`, `archive_client`, `merge_duplicate_clients`, or `hard_delete_client`.

Re-read the record after a write and report what Sqyre returned.
