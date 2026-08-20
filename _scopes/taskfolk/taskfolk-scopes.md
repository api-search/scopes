---
api_specs:
- filename: taskfolk-product-api-openapi.yml
  format: yaml
  label: Taskfolk API
  slug: taskfolk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskfolk/refs/heads/main/openapi/taskfolk-product-api-openapi.yml
- filename: taskfolk-agent-commerce-openapi.yml
  format: yaml
  label: Taskfolk Agent Commerce API
  slug: taskfolk-agent-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskfolk/refs/heads/main/openapi/taskfolk-agent-commerce-openapi.yml
authorization_urls:
- https://taskfolk.ai/api/oauth/authorize
description: ''
docs: https://taskfolk.ai/auth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Taskfolk Scopes
name_suffix: OAuth Scopes
note: 'The published OpenAPI declares ONLY a bearerAuth http scheme, so derive-oauth-scopes.py found zero oauth2 flows in the spec. The OAuth surface is real but lives entirely in the RFC 8414 / RFC 9728 discovery documents and auth.md, not in the contract. All 47 scopes below are read verbatim from those two documents, which agree exactly. Recording the gap: a securitySchemes.oauth2 block in the OpenAPI would put these scopes in the contract where a generated client can see them.'
overview: 'Taskfolk publishes 47 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Taskfolk API on a user''s behalf.


  Tokens are issued from https://taskfolk.ai/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Taskfolk
provider_slug: taskfolk
schemes:
- dynamic_client_registration: RFC 7591, unauthenticated by design, rate limited per IP and per workspace
  flows:
  - authorizationUrl: https://taskfolk.ai/api/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    pkce_required: true
    refreshUrl: https://taskfolk.ai/api/oauth/token
    tokenUrl: https://taskfolk.ai/api/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://taskfolk.ai
  name: oauth2
  registration_endpoint: https://taskfolk.ai/api/oauth/register
  revocation_endpoint: https://taskfolk.ai/api/oauth/revoke
  source: https://taskfolk.ai/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  - client_secret_post
scope_count: 47
scope_names:
- read
- write
- admin
- workspaces:read
- workspaces:write
- projects:read
- projects:write
- projects:admin
- issues:read
- issues:write
- comments:read
- comments:write
- attachments:read
- attachments:write
- labels:read
- labels:write
- custom_fields:read
- custom_fields:write
- saved_views:read
- saved_views:write
- docs:read
- docs:write
- members:read
- members:write
- notifications:read
- notifications:write
- search:read
- chat:read
- chat:write
- forms:read
- forms:write
- automations:read
- automations:write
- portfolios:read
- portfolios:write
- goals:read
- goals:write
- agents:read
- agents:write
- workflows:read
- workflows:write
- api_keys:read
- api_keys:write
- webhooks:read
- webhooks:write
- oauth_apps:read
- oauth_apps:write
scopes:
- description: Read workspaces, projects, issues, comments, members (coarse-grained).
  flows:
  - authorizationCode
  scope: read
- description: Create and update resources (coarse-grained).
  flows:
  - authorizationCode
  scope: write
- description: Workspace management, billing, settings, and agent commerce (credit purchase).
  flows:
  - authorizationCode
  scope: admin
- description: Read access to workspaces.
  flows:
  - authorizationCode
  scope: workspaces:read
- description: Create and update workspaces.
  flows:
  - authorizationCode
  scope: workspaces:write
- description: Read access to projects.
  flows:
  - authorizationCode
  scope: projects:read
- description: Create and update projects.
  flows:
  - authorizationCode
  scope: projects:write
- description: Administer projects.
  flows:
  - authorizationCode
  scope: projects:admin
- description: Read access to issues.
  flows:
  - authorizationCode
  scope: issues:read
- description: Create and update issues.
  flows:
  - authorizationCode
  scope: issues:write
- description: Read access to comments.
  flows:
  - authorizationCode
  scope: comments:read
- description: Create and update comments.
  flows:
  - authorizationCode
  scope: comments:write
- description: Read access to attachments.
  flows:
  - authorizationCode
  scope: attachments:read
- description: Create and update attachments.
  flows:
  - authorizationCode
  scope: attachments:write
- description: Read access to labels.
  flows:
  - authorizationCode
  scope: labels:read
- description: Create and update labels.
  flows:
  - authorizationCode
  scope: labels:write
- description: Read access to custom fields.
  flows:
  - authorizationCode
  scope: custom_fields:read
- description: Create and update custom fields.
  flows:
  - authorizationCode
  scope: custom_fields:write
- description: Read access to saved views.
  flows:
  - authorizationCode
  scope: saved_views:read
- description: Create and update saved views.
  flows:
  - authorizationCode
  scope: saved_views:write
- description: Read access to docs.
  flows:
  - authorizationCode
  scope: docs:read
- description: Create and update docs.
  flows:
  - authorizationCode
  scope: docs:write
- description: Read access to members.
  flows:
  - authorizationCode
  scope: members:read
- description: Create and update members.
  flows:
  - authorizationCode
  scope: members:write
- description: Read access to notifications.
  flows:
  - authorizationCode
  scope: notifications:read
- description: Create and update notifications.
  flows:
  - authorizationCode
  scope: notifications:write
- description: Read access to search.
  flows:
  - authorizationCode
  scope: search:read
- description: Read access to chat.
  flows:
  - authorizationCode
  scope: chat:read
- description: Create and update chat.
  flows:
  - authorizationCode
  scope: chat:write
- description: Read access to forms.
  flows:
  - authorizationCode
  scope: forms:read
- description: Create and update forms.
  flows:
  - authorizationCode
  scope: forms:write
- description: Read access to automations.
  flows:
  - authorizationCode
  scope: automations:read
- description: Create and update automations.
  flows:
  - authorizationCode
  scope: automations:write
- description: Read access to portfolios.
  flows:
  - authorizationCode
  scope: portfolios:read
- description: Create and update portfolios.
  flows:
  - authorizationCode
  scope: portfolios:write
- description: Read access to goals.
  flows:
  - authorizationCode
  scope: goals:read
- description: Create and update goals.
  flows:
  - authorizationCode
  scope: goals:write
- description: Read access to agents.
  flows:
  - authorizationCode
  scope: agents:read
- description: Create and update agents.
  flows:
  - authorizationCode
  scope: agents:write
- description: Read access to workflows.
  flows:
  - authorizationCode
  scope: workflows:read
- description: Create and update workflows.
  flows:
  - authorizationCode
  scope: workflows:write
- description: Read access to api keys.
  flows:
  - authorizationCode
  scope: api_keys:read
- description: Create and update api keys.
  flows:
  - authorizationCode
  scope: api_keys:write
- description: Read access to webhooks.
  flows:
  - authorizationCode
  scope: webhooks:read
- description: Create and update webhooks.
  flows:
  - authorizationCode
  scope: webhooks:write
- description: Read access to oauth apps.
  flows:
  - authorizationCode
  scope: oauth_apps:read
- description: Create and update oauth apps.
  flows:
  - authorizationCode
  scope: oauth_apps:write
slug: taskfolk-scopes
source_filename: taskfolk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-20'\nmethod: searched\nsource: https://taskfolk.ai/.well-known/oauth-authorization-server (RFC 8414, HTTP 200) and https://taskfolk.ai/.well-known/oauth-protected-resource\n  (RFC 9728, HTTP 200)\ndocs: https://taskfolk.ai/auth.md\nnote: 'The published OpenAPI declares ONLY a bearerAuth http scheme, so derive-oauth-scopes.py found zero\n  oauth2 flows in the spec. The OAuth surface is real but lives entirely in the RFC 8414 / RFC 9728 discovery\n  documents and auth.md, not in the contract. All 47 scopes below are read verbatim from those two documents,\n  which agree exactly. Recording the gap: a securitySchemes.oauth2 block in the OpenAPI would put these\n  scopes in the contract where a generated client can see them.'\nschemes:\n- name: oauth2\n  source: https://taskfolk.ai/.well-known/oauth-authorization-server\n  issuer: https://taskfolk.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://taskfolk.ai/api/oauth/authorize\n    tokenUrl:\
  \ https://taskfolk.ai/api/oauth/token\n    refreshUrl: https://taskfolk.ai/api/oauth/token\n    pkce_required: true\n    code_challenge_methods:\n    - S256\n  revocation_endpoint: https://taskfolk.ai/api/oauth/revoke\n  registration_endpoint: https://taskfolk.ai/api/oauth/register\n  dynamic_client_registration: RFC 7591, unauthenticated by design, rate limited per IP and per workspace\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  grant_types:\n  - authorization_code\n  - refresh_token\nprotected_resources:\n- https://taskfolk.ai/api/mcp/v1\nscope_count: 47\nscope_model: Three coarse scopes (read / write / admin) plus 44 fine-grained resource:action scopes across\n  22 resource families. A key is bound to exactly one workspace and carries a set of scopes; MCP tools/list\n  is filtered by them, so a read-only key literally cannot see a write tool. Tokens inherit the creator\n  role ceiling.\nscopes:\n- scope: read\n  description: Read workspaces, projects, issues,\
  \ comments, members (coarse-grained).\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: write\n  description: Create and update resources (coarse-grained).\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: admin\n  description: Workspace management, billing, settings, and agent commerce (credit purchase).\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: workspaces:read\n  description: Read access to workspaces.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: workspaces:write\n\
  \  description: Create and update workspaces.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: projects:read\n  description: Read access to projects.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: projects:write\n  description: Create and update projects.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: projects:admin\n  description: Administer projects.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: issues:read\n  description: Read access to issues.\n  flows:\n \
  \ - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: issues:write\n  description: Create and update issues.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: comments:read\n  description: Read access to comments.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: comments:write\n  description: Create and update comments.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: attachments:read\n  description: Read access to attachments.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n\
  \  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: attachments:write\n  description: Create and update attachments.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: labels:read\n  description: Read access to labels.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: labels:write\n  description: Create and update labels.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: custom_fields:read\n  description: Read access to custom fields.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n\
  - scope: custom_fields:write\n  description: Create and update custom fields.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: saved_views:read\n  description: Read access to saved views.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: saved_views:write\n  description: Create and update saved views.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: docs:read\n  description: Read access to docs.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: docs:write\n  description:\
  \ Create and update docs.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: members:read\n  description: Read access to members.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: members:write\n  description: Create and update members.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: notifications:read\n  description: Read access to notifications.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: notifications:write\n  description: Create and update notifications.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: search:read\n  description: Read access to search.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: chat:read\n  description: Read access to chat.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: chat:write\n  description: Create and update chat.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: forms:read\n  description: Read access to forms.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n\
  \  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: forms:write\n  description: Create and update forms.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: automations:read\n  description: Read access to automations.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: automations:write\n  description: Create and update automations.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: portfolios:read\n  description: Read access to portfolios.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n\
  - scope: portfolios:write\n  description: Create and update portfolios.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: goals:read\n  description: Read access to goals.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: goals:write\n  description: Create and update goals.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: agents:read\n  description: Read access to agents.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: agents:write\n  description: Create and update agents.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: workflows:read\n  description: Read access to workflows.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: workflows:write\n  description: Create and update workflows.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: api_keys:read\n  description: Read access to api keys.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: api_keys:write\n  description: Create and update api keys.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: webhooks:read\n  description: Read access to webhooks.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: webhooks:write\n  description: Create and update webhooks.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: oauth_apps:read\n  description: Read access to oauth apps.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n  - https://taskfolk.ai/.well-known/oauth-protected-resource\n- scope: oauth_apps:write\n  description: Create and update oauth apps.\n  flows:\n  - authorizationCode\n  sources:\n  - https://taskfolk.ai/.well-known/oauth-authorization-server\n\
  \  - https://taskfolk.ai/.well-known/oauth-protected-resource\nagent_auth:\n  skill: https://taskfolk.ai/auth.md\n  identity_types_supported:\n  - anonymous\n  credential_types_supported:\n  - oauth2_authorization_code\n  - access_token\n  note: Non-standard agent_auth block in the AS metadata. It lets an ANONYMOUS agent register an OAuth\n    client with no pre-existing account or API key, then obtain user-delegated tokens through a claim\n    ceremony the human approves. This is the mechanism that makes the OAuth surface reachable by an agent\n    that has never met the user.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskfolk/refs/heads/main/scopes/taskfolk-scopes.yml
summary_line: 47 scopes · authorizationCode
tags:
- Project Management
- Issue Tracking
- Task Management
- Productivity
- Collaboration
- MCP
- AI Agents
- agent-native
- Agentic Commerce
- A2A
- REST API
- OpenAPI
- Webhook
- Authentication
- Agile
- Sprints
- OKR
- Developer Tools
token_urls:
- https://taskfolk.ai/api/oauth/token
---
