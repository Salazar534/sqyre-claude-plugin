---
name: communications
description: Use when the user wants to read or send Sqyre texts, emails, or call history. Draft first unless they asked to send now.
---

# Sqyre messages

Use Sqyre MCP tools only. Never invent phone numbers or message text the user did not approve.

Read with `list_conversations`, `get_conversation_messages`, `get_unanswered_conversations`, `list_calls`, `get_call`, `get_missed_calls`, and `get_calls_by_client`.

Check `get_opt_out_status` before a text. If the client is opted out, do not send.

`create_sms_draft` and `create_email_draft` are the default. Call `send_sms`, `send_email`, or `reply_to_client` only after the user has seen the exact text and said to send it. `initiate_call` places a real call. Confirm the number first.
