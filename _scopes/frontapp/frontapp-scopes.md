---
authorization_urls:
- https://app.frontapp.com/oauth/authorize
description: ''
docs: https://dev.frontapp.com/docs/oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Frontapp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FrontApp publishes 57 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the FrontApp API on a user''s behalf.


  Tokens are issued from https://app.frontapp.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FrontApp
provider_slug: frontapp
schemes:
- flows:
  - authorizationUrl: https://app.frontapp.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.frontapp.com/oauth/token
  name: oauth2
scope_count: 57
scope_names:
- accounts:read
- accounts:write
- accounts:delete
- analytics:read
- attachments:read
- channels:read
- channels:write
- comments:read
- comments:write
- contacts:read
- contacts:write
- contacts:delete
- conversations:read
- conversations:write
- conversations:delete
- custom_fields:read
- drafts:read
- drafts:write
- drafts:delete
- events:*:read
- inboxes:read
- inboxes:write
- knowledge_bases:read
- knowledge_bases:write
- knowledge_bases:delete
- links:read
- links:write
- message_templates:read
- message_templates:write
- message_templates:delete
- messages:read
- messages:write
- messages:send
- rules:read
- shifts:read
- shifts:write
- signatures:read
- signatures:write
- signatures:delete
- statuses:read
- tags:read
- tags:write
- tags:delete
- teammate_groups:read
- teammate_groups:write
- teammate_groups:delete
- teammates:read
- teammates:write
- teams:read
- teams:write
- time_off:read
- time_off:write
- time_off:delete
- views:read
- views:write
- feature:app_trigger
- feature:mcp
scopes:
- description: Read accounts (companies)
  flows: []
  scope: accounts:read
- description: Create and update accounts
  flows: []
  scope: accounts:write
- description: Delete accounts
  flows: []
  scope: accounts:delete
- description: Create and fetch analytics reports and exports
  flows: []
  scope: analytics:read
- description: Download message attachments
  flows: []
  scope: attachments:read
- description: Read channels
  flows: []
  scope: channels:read
- description: Create and update channels
  flows: []
  scope: channels:write
- description: Read internal comments
  flows: []
  scope: comments:read
- description: Create comments and mentions
  flows: []
  scope: comments:write
- description: Read contacts and contact lists
  flows: []
  scope: contacts:read
- description: Create
  flows: []
  scope: contacts:write
- description: Delete contacts
  flows: []
  scope: contacts:delete
- description: List and read conversations and events
  flows: []
  scope: conversations:read
- description: Create and update conversations
  flows: []
  scope: conversations:write
- description: Delete conversations
  flows: []
  scope: conversations:delete
- description: Read custom fields
  flows: []
  scope: custom_fields:read
- description: Read message drafts
  flows: []
  scope: drafts:read
- description: Create and update drafts
  flows: []
  scope: drafts:write
- description: Delete drafts
  flows: []
  scope: drafts:delete
- description: Read events (wildcard event source)
  flows: []
  scope: events:*:read
- description: Read inboxes
  flows: []
  scope: inboxes:read
- description: Create and update inboxes
  flows: []
  scope: inboxes:write
- description: Read knowledge bases
  flows: []
  scope: knowledge_bases:read
- description: Create and update knowledge bases
  flows: []
  scope: knowledge_bases:write
- description: Delete knowledge base content
  flows: []
  scope: knowledge_bases:delete
- description: Read links and linked conversations
  flows: []
  scope: links:read
- description: Create and update links
  flows: []
  scope: links:write
- description: Read message templates
  flows: []
  scope: message_templates:read
- description: Create and update message templates
  flows: []
  scope: message_templates:write
- description: Delete message templates
  flows: []
  scope: message_templates:delete
- description: Read messages
  flows: []
  scope: messages:read
- description: Create and update messages
  flows: []
  scope: messages:write
- description: Send outbound messages
  flows: []
  scope: messages:send
- description: Read rules
  flows: []
  scope: rules:read
- description: Read shifts
  flows: []
  scope: shifts:read
- description: Create and update shifts
  flows: []
  scope: shifts:write
- description: Read signatures
  flows: []
  scope: signatures:read
- description: Create and update signatures
  flows: []
  scope: signatures:write
- description: Delete signatures
  flows: []
  scope: signatures:delete
- description: Read ticket/conversation statuses
  flows: []
  scope: statuses:read
- description: Read tags
  flows: []
  scope: tags:read
- description: Create and update tags
  flows: []
  scope: tags:write
- description: Delete tags
  flows: []
  scope: tags:delete
- description: Read teammate groups
  flows: []
  scope: teammate_groups:read
- description: Create and update teammate groups
  flows: []
  scope: teammate_groups:write
- description: Delete teammate groups
  flows: []
  scope: teammate_groups:delete
- description: Read teammates
  flows: []
  scope: teammates:read
- description: Update teammates
  flows: []
  scope: teammates:write
- description: Read teams
  flows: []
  scope: teams:read
- description: Create and update teams
  flows: []
  scope: teams:write
- description: Read time off
  flows: []
  scope: time_off:read
- description: Create and update time off
  flows: []
  scope: time_off:write
- description: Delete time off
  flows: []
  scope: time_off:delete
- description: Read views
  flows: []
  scope: views:read
- description: Create and update views
  flows: []
  scope: views:write
- description: Feature scope for application triggers
  flows: []
  scope: feature:app_trigger
- description: Feature scope granting access to the Front MCP server
  flows: []
  scope: feature:mcp
slug: frontapp-scopes
source_filename: frontapp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://dev.frontapp.com/reference (per-endpoint \"Required scope\") + https://dev.frontapp.com/docs/oauth\ndocs: https://dev.frontapp.com/docs/oauth\nschemes:\n- name: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.frontapp.com/oauth/authorize\n    tokenUrl: https://app.frontapp.com/oauth/token\nnotes: >-\n  Front uses granular resource:action scopes (read/write/delete). Some resources\n  additionally support a delete scope. `events:*:read` uses a wildcard segment\n  for the event source. `feature:app_trigger` and `feature:mcp` are feature\n  scopes rather than resource scopes. Scopes were harvested from the \"Required\n  scope\" annotations across the 340+ published API reference endpoints.\nscopes:\n- {scope: accounts:read, description: Read accounts (companies)}\n- {scope: accounts:write, description: Create and update accounts}\n- {scope: accounts:delete, description: Delete accounts}\n\
  - {scope: analytics:read, description: Create and fetch analytics reports and exports}\n- {scope: attachments:read, description: Download message attachments}\n- {scope: channels:read, description: Read channels}\n- {scope: channels:write, description: Create and update channels}\n- {scope: comments:read, description: Read internal comments}\n- {scope: comments:write, description: Create comments and mentions}\n- {scope: contacts:read, description: Read contacts and contact lists}\n- {scope: contacts:write, description: Create, update, and merge contacts}\n- {scope: contacts:delete, description: Delete contacts}\n- {scope: conversations:read, description: List and read conversations and events}\n- {scope: conversations:write, description: Create and update conversations}\n- {scope: conversations:delete, description: Delete conversations}\n- {scope: custom_fields:read, description: Read custom fields}\n- {scope: drafts:read, description: Read message drafts}\n- {scope: drafts:write, description:\
  \ Create and update drafts}\n- {scope: drafts:delete, description: Delete drafts}\n- {scope: 'events:*:read', description: Read events (wildcard event source)}\n- {scope: inboxes:read, description: Read inboxes}\n- {scope: inboxes:write, description: Create and update inboxes}\n- {scope: knowledge_bases:read, description: Read knowledge bases, articles, and categories}\n- {scope: knowledge_bases:write, description: Create and update knowledge bases, articles, and categories}\n- {scope: knowledge_bases:delete, description: Delete knowledge base content}\n- {scope: links:read, description: Read links and linked conversations}\n- {scope: links:write, description: Create and update links}\n- {scope: message_templates:read, description: Read message templates}\n- {scope: message_templates:write, description: Create and update message templates}\n- {scope: message_templates:delete, description: Delete message templates}\n- {scope: messages:read, description: Read messages}\n- {scope: messages:write,\
  \ description: Create and update messages}\n- {scope: messages:send, description: Send outbound messages}\n- {scope: rules:read, description: Read rules}\n- {scope: shifts:read, description: Read shifts}\n- {scope: shifts:write, description: Create and update shifts}\n- {scope: signatures:read, description: Read signatures}\n- {scope: signatures:write, description: Create and update signatures}\n- {scope: signatures:delete, description: Delete signatures}\n- {scope: statuses:read, description: Read ticket/conversation statuses}\n- {scope: tags:read, description: Read tags}\n- {scope: tags:write, description: Create and update tags}\n- {scope: tags:delete, description: Delete tags}\n- {scope: teammate_groups:read, description: Read teammate groups}\n- {scope: teammate_groups:write, description: Create and update teammate groups}\n- {scope: teammate_groups:delete, description: Delete teammate groups}\n- {scope: teammates:read, description: Read teammates}\n- {scope: teammates:write, description:\
  \ Update teammates}\n- {scope: teams:read, description: Read teams}\n- {scope: teams:write, description: Create and update teams}\n- {scope: time_off:read, description: Read time off}\n- {scope: time_off:write, description: Create and update time off}\n- {scope: time_off:delete, description: Delete time off}\n- {scope: views:read, description: Read views}\n- {scope: views:write, description: Create and update views}\n- {scope: feature:app_trigger, description: Feature scope for application triggers}\n- {scope: feature:mcp, description: Feature scope granting access to the Front MCP server}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontapp/refs/heads/main/scopes/frontapp-scopes.yml
summary_line: 57 scopes · authorizationCode
tags:
- Company
- Communication
- Customer Service
- Shared Inbox
- Email
- Messaging
- Collaboration
- Help Desk
token_urls:
- https://app.frontapp.com/oauth/token
---
