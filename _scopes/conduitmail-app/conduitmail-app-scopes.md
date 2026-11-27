---
authorization_urls: []
description: ''
docs: https://conduitmail.app/agents
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Conduit Mail Scopes
name_suffix: OAuth Scopes
note: Scope list from scopes_supported in https://connect.conduitmail.app/.well-known/oauth-authorization-server (HTTP 200); descriptions from the "What an agent can do" section of /agents. A grant covers every mailbox the user has linked to Conduit.
overview: 'Conduit Mail publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Conduit Mail API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Conduit Mail
provider_slug: conduitmail-app
schemes: []
scope_count: 4
scope_names:
- email:read
- email:write
- rules:manage
- notes:manage
scopes:
- description: Search, open messages (and whole threads on Gmail), read attachments up to 5 MB, and list folders and accounts. Full message bodies arrive marked as untrusted content.
  flows: []
  scope: email:read
- description: Mark read/unread, star, archive and move mail to Trash (up to 50 messages a call) or mark a whole folder read; labels on Gmail; drafts, reply and send (direct sending is off until enabled in Settings); block senders (off by default).
  flows: []
  scope: email:write
- description: Create, pause and delete automation rules. A rule an agent writes can't trash, archive or call a webhook.
  flows: []
  scope: rules:manage
- description: Create and edit notes.
  flows: []
  scope: notes:manage
slug: conduitmail-app-scopes
source_filename: conduitmail-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://conduitmail.app/agents\ndocs: https://conduitmail.app/agents\nname: Conduit Mail OAuth scopes\nnote: Scope list from scopes_supported in https://connect.conduitmail.app/.well-known/oauth-authorization-server (HTTP 200); descriptions from the \"What an agent can do\" section of /agents. A grant covers every mailbox the user has linked to Conduit.\nscopes:\n- name: email:read\n  description: Search, open messages (and whole threads on Gmail), read attachments up to 5 MB, and list folders and accounts. Full message bodies arrive marked as untrusted content.\n- name: email:write\n  description: Mark read/unread, star, archive and move mail to Trash (up to 50 messages a call) or mark a whole folder read; labels on Gmail; drafts, reply and send (direct sending is off until enabled in Settings); block senders (off by default).\n- name: rules:manage\n  description: Create, pause and delete automation rules. A rule an agent\
  \ writes can't trash, archive or call a webhook.\n- name: notes:manage\n  description: Create and edit notes.\nwithheld:\n- Delete received mail forever, move it into folders of its choosing, delete labels, turn on its own sending, or see mailbox passwords.\n"
source_yaml_url: https://artifacts.apis.io/conduitmail-app/scopes/conduitmail-app-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Email
- Email Client
- Artificial Intelligence
- MCP
- AI Agents
- Productivity
- Automation
token_bound: false
token_urls: []
---
