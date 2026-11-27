---
authorization_urls: []
description: ''
docs: https://commandmail.app/en/docs/permissions-and-autonomy
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Command Mail Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Command Mail publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Command Mail API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Command Mail
provider_slug: commandmail-app
schemes: []
scope_count: 5
scope_names:
- mail:read
- mail:draft
- mail:send-approved
- mail:send
- mailboxes
scopes:
- description: Read, search and view without marking as read; overview and morning brief; sort within the autonomy level; view activity and undo its own actions; suggest rules; follow up
  flows: []
  scope: mail:read
- description: Save drafts. Never sends or overwrites your edits
  flows: []
  scope: mail:draft
- description: Send the exact version you approved
  flows: []
  scope: mail:send-approved
- description: Send and reply independently from mailboxes on auto, each email with its own sendKey, within the daily limit (50 by default)
  flows: []
  scope: mail:send
- description: Connect addresses, verify domain ownership with a TXT record, import old emails. Sending is set up for each sender address, from Pro
  flows: []
  scope: mailboxes
slug: commandmail-app-scopes
source_filename: commandmail-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commandmail.app/en/docs\ndocs: https://commandmail.app/en/docs/permissions-and-autonomy\nscopes:\n- name: mail:read\n  description: Read, search and view without marking as read; overview and morning brief; sort within the autonomy level; view activity and undo its own actions; suggest rules; follow up\n- name: mail:draft\n  description: Save drafts. Never sends or overwrites your edits\n- name: mail:send-approved\n  description: Send the exact version you approved\n- name: mail:send\n  description: Send and reply independently from mailboxes on auto, each email with its own sendKey, within the daily limit (50 by default)\n- name: mailboxes\n  description: Connect addresses, verify domain ownership with a TXT record, import old emails. Sending is set up for each sender address, from Pro\nnotes:\n- Forwarding, direct Trash and restore calls, direct permanent deletion, emptying Trash or Spam, marking everything read,\
  \ and switching on or shortening automatic removal of Spam and Trash need mail:read and mail:send together.\n- Operator permissions such as admin are not available for customer keys.\n"
source_yaml_url: https://artifacts.apis.io/commandmail-app/scopes/commandmail-app-scopes.yml
summary_line: 5 scopes
tags:
- Company
- Email
- AI Agents
- MCP
- Inbox
- Productivity
- Automation
token_bound: false
token_urls: []
---
