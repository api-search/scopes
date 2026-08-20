---
authorization_urls:
- https://mcp.reevo.ai/authorize
description: ''
docs: https://help.reevo.ai/AI-and-productivity/Reevo-MCP
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Reevo Scopes
name_suffix: OAuth Scopes
note: These are the OAuth 2.0 scopes Reevo's MCP server requests at authorization, transcribed from Reevo's published MCP documentation. `derive-oauth-scopes.py` was run first and produced nothing because the repo holds no OpenAPI. The MCP authorization-server metadata document at https://mcp.reevo.ai/.well-known/oauth-authorization-server does NOT publish a scopes_supported array, so this list cannot be confirmed mechanically without an authorization round-trip against an enabled workspace. Scope naming is verb:object. The public REST API at api.reevo.ai does not use OAuth — it uses per-key read/write permissions recorded in authentication/reevo-authentication.yml.
overview: 'Reevo publishes 22 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Reevo API on a user''s behalf.


  Tokens are issued from https://mcp.reevo.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Reevo
provider_slug: reevo
schemes:
- applies_to: https://mcp.reevo.ai/mcp
  flows:
  - authorizationUrl: https://mcp.reevo.ai/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://mcp.reevo.ai/token
  name: ReevoMCPOAuth
  scopes_supported_published: false
  source: https://mcp.reevo.ai/.well-known/oauth-authorization-server
scope_count: 22
scope_names:
- read:account
- create:account
- update:account
- read:contact
- create:contact
- update:contact
- read:opportunity
- create:opportunity
- update:opportunity
- read:pipeline
- read:meeting
- read:task
- create:task
- update:task
- read:note
- create:note
- read:custom_object
- create:custom_object
- update:custom_object
- read:sequence
- update:sequence
- read:email_account
scopes:
- description: Read accounts.
  flows:
  - authorizationCode
  scope: read:account
- description: Create accounts.
  flows:
  - authorizationCode
  scope: create:account
- description: Update existing accounts.
  flows:
  - authorizationCode
  scope: update:account
- description: Read contacts.
  flows:
  - authorizationCode
  scope: read:contact
- description: Create contacts.
  flows:
  - authorizationCode
  scope: create:contact
- description: Update existing contacts.
  flows:
  - authorizationCode
  scope: update:contact
- description: Read opportunities.
  flows:
  - authorizationCode
  scope: read:opportunity
- description: Create opportunities.
  flows:
  - authorizationCode
  scope: create:opportunity
- description: Update opportunities, including moving them between pipeline stages.
  flows:
  - authorizationCode
  scope: update:opportunity
- description: Read the opportunity pipelines and their stages configured in the workspace.
  flows:
  - authorizationCode
  scope: read:pipeline
- description: Read meetings, including recording and transcript status.
  flows:
  - authorizationCode
  scope: read:meeting
- description: Read tasks.
  flows:
  - authorizationCode
  scope: read:task
- description: Create tasks.
  flows:
  - authorizationCode
  scope: create:task
- description: Update task status, owner, due date or description.
  flows:
  - authorizationCode
  scope: update:task
- description: Read notes.
  flows:
  - authorizationCode
  scope: read:note
- description: Log a note on an account, contact or opportunity.
  flows:
  - authorizationCode
  scope: create:note
- description: Read records in custom objects.
  flows:
  - authorizationCode
  scope: read:custom_object
- description: Create records in custom objects.
  flows:
  - authorizationCode
  scope: create:custom_object
- description: Update records in custom objects.
  flows:
  - authorizationCode
  scope: update:custom_object
- description: Read sequences and their performance metrics.
  flows:
  - authorizationCode
  scope: read:sequence
- description: Enroll and unenroll contacts in sequences. Enrolling sends real outreach email.
  flows:
  - authorizationCode
  scope: update:sequence
- description: List the email accounts the connected user can send from, with status and quota.
  flows:
  - authorizationCode
  scope: read:email_account
slug: reevo-scopes
source_filename: reevo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.reevo.ai/AI-and-productivity/Reevo-MCP\ndocs: https://help.reevo.ai/AI-and-productivity/Reevo-MCP\nnote: 'These are the OAuth 2.0 scopes Reevo''s MCP server requests at authorization,\n  transcribed from Reevo''s published MCP documentation. `derive-oauth-scopes.py` was\n  run first and produced nothing because the repo holds no OpenAPI. The MCP authorization-server\n  metadata document at https://mcp.reevo.ai/.well-known/oauth-authorization-server\n  does NOT publish a scopes_supported array, so this list cannot be confirmed mechanically\n  without an authorization round-trip against an enabled workspace. Scope naming is\n  verb:object. The public REST API at api.reevo.ai does not use OAuth — it uses per-key\n  read/write permissions recorded in authentication/reevo-authentication.yml.'\nschemes:\n- name: ReevoMCPOAuth\n  source: https://mcp.reevo.ai/.well-known/oauth-authorization-server\n  applies_to: https://mcp.reevo.ai/mcp\n\
  \  scopes_supported_published: false\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.reevo.ai/authorize\n    tokenUrl: https://mcp.reevo.ai/token\n    pkce: S256\nscope_count: 22\nscopes:\n- scope: read:account\n  description: Read accounts.\n  object: account\n  action: read\n  flows:\n  - authorizationCode\n- scope: create:account\n  description: Create accounts.\n  object: account\n  action: create\n  flows:\n  - authorizationCode\n- scope: update:account\n  description: Update existing accounts.\n  object: account\n  action: update\n  flows:\n  - authorizationCode\n- scope: read:contact\n  description: Read contacts.\n  object: contact\n  action: read\n  flows:\n  - authorizationCode\n- scope: create:contact\n  description: Create contacts.\n  object: contact\n  action: create\n  flows:\n  - authorizationCode\n- scope: update:contact\n  description: Update existing contacts.\n  object: contact\n  action: update\n  flows:\n  - authorizationCode\n- scope: read:opportunity\n\
  \  description: Read opportunities.\n  object: opportunity\n  action: read\n  flows:\n  - authorizationCode\n- scope: create:opportunity\n  description: Create opportunities.\n  object: opportunity\n  action: create\n  flows:\n  - authorizationCode\n- scope: update:opportunity\n  description: Update opportunities, including moving them between pipeline stages.\n  object: opportunity\n  action: update\n  flows:\n  - authorizationCode\n- scope: read:pipeline\n  description: Read the opportunity pipelines and their stages configured in the workspace.\n  object: pipeline\n  action: read\n  flows:\n  - authorizationCode\n- scope: read:meeting\n  description: Read meetings, including recording and transcript status.\n  object: meeting\n  action: read\n  flows:\n  - authorizationCode\n- scope: read:task\n  description: Read tasks.\n  object: task\n  action: read\n  flows:\n  - authorizationCode\n- scope: create:task\n  description: Create tasks.\n  object: task\n  action: create\n  flows:\n \
  \ - authorizationCode\n- scope: update:task\n  description: Update task status, owner, due date or description.\n  object: task\n  action: update\n  flows:\n  - authorizationCode\n- scope: read:note\n  description: Read notes.\n  object: note\n  action: read\n  flows:\n  - authorizationCode\n- scope: create:note\n  description: Log a note on an account, contact or opportunity.\n  object: note\n  action: create\n  flows:\n  - authorizationCode\n- scope: read:custom_object\n  description: Read records in custom objects.\n  object: custom_object\n  action: read\n  flows:\n  - authorizationCode\n- scope: create:custom_object\n  description: Create records in custom objects.\n  object: custom_object\n  action: create\n  flows:\n  - authorizationCode\n- scope: update:custom_object\n  description: Update records in custom objects.\n  object: custom_object\n  action: update\n  flows:\n  - authorizationCode\n- scope: read:sequence\n  description: Read sequences and their performance metrics.\n\
  \  object: sequence\n  action: read\n  flows:\n  - authorizationCode\n- scope: update:sequence\n  description: Enroll and unenroll contacts in sequences. Enrolling sends real outreach\n    email.\n  object: sequence\n  action: update\n  flows:\n  - authorizationCode\n- scope: read:email_account\n  description: List the email accounts the connected user can send from, with status\n    and quota.\n  object: email_account\n  action: read\n  flows:\n  - authorizationCode\nunscoped_tools:\n- tool: whoami\n  note: Documented as requiring no scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reevo/refs/heads/main/scopes/reevo-scopes.yml
summary_line: 22 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Sales
- CRM
- Revenue Operations
- Sales Automation
- Lead Generation
- Agents
- MCP
- Sales Engagement
token_urls:
- https://mcp.reevo.ai/token
---
