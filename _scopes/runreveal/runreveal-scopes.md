---
authorization_urls:
- https://www-api.runreveal.com/oauth/authorize
description: ''
docs: https://docs.runreveal.com/ai-chat/model-context-protocol
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Runreveal Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RunReveal publishes 37 OAuth 2.0 scopes via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the RunReveal API on a user''s behalf.


  Tokens are issued from https://www-api.runreveal.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RunReveal
provider_slug: runreveal
schemes:
- flows:
  - authorizationUrl: https://www-api.runreveal.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    tokenUrl: https://www-api.runreveal.com/oauth/token
  - flow: refreshToken
    tokenUrl: https://www-api.runreveal.com/oauth/token
  issuer: https://www-api.runreveal.com
  name: OAuth2
  registration_endpoint: https://www-api.runreveal.com/oauth/client
  source: https://api.runreveal.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - client_secret_post
  - none
scope_count: 37
scope_names:
- workspaces#read
- workspaces#edit
- sources#read
- sources#edit
- destinations#read
- destinations#edit
- queries#read
- queries#edit
- filters#read
- filters#edit
- enrichments#read
- enrichments#edit
- investigations#read
- investigations#edit
- investigations#delete
- notifications#read
- notifications#edit
- notifications#send
- dashboard_layouts#read
- dashboard_layouts#edit
- custom_views#read
- custom_views#edit
- custom_roles#read
- custom_roles#edit
- agents#read
- agents#edit
- agent_skills#read
- agent_skills#edit
- agent_skills#load
- chat#read
- chat#edit
- topics#read
- topics#edit
- params#read
- params#edit
- tokens#create
- sessions#manage
scopes:
- description: Read workspace settings and membership
  flows: []
  scope: workspaces#read
- description: Modify workspace settings and membership
  flows: []
  scope: workspaces#edit
- description: Read log sources and their configuration
  flows: []
  scope: sources#read
- description: Create and modify log sources
  flows: []
  scope: sources#edit
- description: Read log destinations
  flows: []
  scope: destinations#read
- description: Create and modify log destinations
  flows: []
  scope: destinations#edit
- description: Read saved queries
  flows: []
  scope: queries#read
- description: Create and modify saved queries
  flows: []
  scope: queries#edit
- description: Read pipeline filters
  flows: []
  scope: filters#read
- description: Create and modify pipeline filters
  flows: []
  scope: filters#edit
- description: Read log enrichments
  flows: []
  scope: enrichments#read
- description: Create and modify log enrichments
  flows: []
  scope: enrichments#edit
- description: Read investigations
  flows: []
  scope: investigations#read
- description: Create and modify investigations
  flows: []
  scope: investigations#edit
- description: Delete investigations
  flows: []
  scope: investigations#delete
- description: Read notification configuration
  flows: []
  scope: notifications#read
- description: Create and modify notification configuration
  flows: []
  scope: notifications#edit
- description: Send notifications
  flows: []
  scope: notifications#send
- description: Read dashboard layouts
  flows: []
  scope: dashboard_layouts#read
- description: Create and modify dashboard layouts
  flows: []
  scope: dashboard_layouts#edit
- description: Read custom log views
  flows: []
  scope: custom_views#read
- description: Create and modify custom log views
  flows: []
  scope: custom_views#edit
- description: Read custom RBAC roles
  flows: []
  scope: custom_roles#read
- description: Create and modify custom RBAC roles
  flows: []
  scope: custom_roles#edit
- description: Read AI agents
  flows: []
  scope: agents#read
- description: Create and modify AI agents
  flows: []
  scope: agents#edit
- description: Read agent skills
  flows: []
  scope: agent_skills#read
- description: Create and modify agent skills
  flows: []
  scope: agent_skills#edit
- description: Load and execute agent skills
  flows: []
  scope: agent_skills#load
- description: Read AI chat sessions
  flows: []
  scope: chat#read
- description: Create and modify AI chat sessions
  flows: []
  scope: chat#edit
- description: Read topics
  flows: []
  scope: topics#read
- description: Create and modify topics
  flows: []
  scope: topics#edit
- description: Read parameters
  flows: []
  scope: params#read
- description: Create and modify parameters
  flows: []
  scope: params#edit
- description: Create API tokens
  flows: []
  scope: tokens#create
- description: Manage authentication sessions
  flows: []
  scope: sessions#manage
slug: runreveal-scopes
source_filename: runreveal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.runreveal.com/.well-known/oauth-authorization-server\ndocs: https://docs.runreveal.com/ai-chat/model-context-protocol\nnotes: >-\n  Scopes captured verbatim from RunReveal's RFC 8414 OAuth Authorization Server\n  metadata (scopes_supported). Format is resource#action. OAuth is used for the\n  hosted remote MCP server and for third-party API access; the CLI also supports\n  API-token auth. No published human-readable scope reference page was found, so\n  descriptions below are derived from the resource#action naming.\nschemes:\n- name: OAuth2\n  source: https://api.runreveal.com/.well-known/oauth-authorization-server\n  issuer: https://www-api.runreveal.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www-api.runreveal.com/oauth/authorize\n    tokenUrl: https://www-api.runreveal.com/oauth/token\n    pkce: [S256, plain]\n  - flow: refreshToken\n    tokenUrl: https://www-api.runreveal.com/oauth/token\n\
  \  registration_endpoint: https://www-api.runreveal.com/oauth/client\n  token_endpoint_auth_methods: [client_secret_post, none]\nscopes:\n- {scope: 'workspaces#read',        description: Read workspace settings and membership}\n- {scope: 'workspaces#edit',        description: Modify workspace settings and membership}\n- {scope: 'sources#read',           description: Read log sources and their configuration}\n- {scope: 'sources#edit',           description: Create and modify log sources}\n- {scope: 'destinations#read',      description: Read log destinations}\n- {scope: 'destinations#edit',      description: Create and modify log destinations}\n- {scope: 'queries#read',           description: Read saved queries}\n- {scope: 'queries#edit',           description: Create and modify saved queries}\n- {scope: 'filters#read',           description: Read pipeline filters}\n- {scope: 'filters#edit',           description: Create and modify pipeline filters}\n- {scope: 'enrichments#read',      \
  \ description: Read log enrichments}\n- {scope: 'enrichments#edit',       description: Create and modify log enrichments}\n- {scope: 'investigations#read',    description: Read investigations}\n- {scope: 'investigations#edit',    description: Create and modify investigations}\n- {scope: 'investigations#delete',  description: Delete investigations}\n- {scope: 'notifications#read',     description: Read notification configuration}\n- {scope: 'notifications#edit',     description: Create and modify notification configuration}\n- {scope: 'notifications#send',     description: Send notifications}\n- {scope: 'dashboard_layouts#read', description: Read dashboard layouts}\n- {scope: 'dashboard_layouts#edit', description: Create and modify dashboard layouts}\n- {scope: 'custom_views#read',      description: Read custom log views}\n- {scope: 'custom_views#edit',      description: Create and modify custom log views}\n- {scope: 'custom_roles#read',      description: Read custom RBAC roles}\n- {scope:\
  \ 'custom_roles#edit',      description: Create and modify custom RBAC roles}\n- {scope: 'agents#read',            description: Read AI agents}\n- {scope: 'agents#edit',            description: Create and modify AI agents}\n- {scope: 'agent_skills#read',      description: Read agent skills}\n- {scope: 'agent_skills#edit',      description: Create and modify agent skills}\n- {scope: 'agent_skills#load',      description: Load and execute agent skills}\n- {scope: 'chat#read',              description: Read AI chat sessions}\n- {scope: 'chat#edit',              description: Create and modify AI chat sessions}\n- {scope: 'topics#read',            description: Read topics}\n- {scope: 'topics#edit',            description: Create and modify topics}\n- {scope: 'params#read',            description: Read parameters}\n- {scope: 'params#edit',            description: Create and modify parameters}\n- {scope: 'tokens#create',          description: Create API tokens}\n- {scope: 'sessions#manage', \
  \       description: Manage authentication sessions}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runreveal/refs/heads/main/scopes/runreveal-scopes.yml
summary_line: 37 scopes · authorizationCode/refreshToken
tags:
- Company
- Security
- SIEM
- Security Log Management
- Detection Engineering
- Threat Detection
- Incident Response
- Observability
- SQL
- MCP
- AI
token_urls:
- https://www-api.runreveal.com/oauth/token
---
