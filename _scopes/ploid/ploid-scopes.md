---
api_specs:
- filename: ploid-account-api-openapi.yml
  format: yaml
  label: Ploid Account API
  slug: ploid-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-account-api-openapi.yml
- filename: ploid-discovery-api-openapi.yml
  format: yaml
  label: Ploid Discovery API
  slug: ploid-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-discovery-api-openapi.yml
- filename: ploid-enrichment-api-openapi.yml
  format: yaml
  label: Ploid Enrichment API
  slug: ploid-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-enrichment-api-openapi.yml
- filename: ploid-harness-api-openapi.yml
  format: yaml
  label: Ploid Harness API
  slug: ploid-harness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-harness-api-openapi.yml
- filename: ploid-monitors-api-openapi.yml
  format: yaml
  label: Ploid Monitors API
  slug: ploid-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-monitors-api-openapi.yml
- filename: ploid-people-api-openapi.yml
  format: yaml
  label: Ploid People API
  slug: ploid-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-people-api-openapi.yml
- filename: ploid-search-api-openapi.yml
  format: yaml
  label: Ploid Search API
  slug: ploid-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-search-api-openapi.yml
- filename: ploid-social-api-openapi.yml
  format: yaml
  label: Ploid Social API
  slug: ploid-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-social-api-openapi.yml
- filename: ploid-linked-in-api-openapi.yml
  format: yaml
  label: Ploid Linked In API
  slug: ploid-linked-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-linked-in-api-openapi.yml
authorization_urls: []
description: ''
docs: https://ploid.com/documentation/getting-started/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Ploid Scopes
name_suffix: OAuth Scopes
note: The OpenAPI document declares bearer and x-api-key schemes with no oauth2 scheme, so scopes are documented rather than derived. API keys are permissioned with these scopes; the hosted MCP server is an OAuth 2.1 protected resource whose metadata lists agent:chat, people:enrich, people:search and account:read. An endpoint called without its required permission returns 403 insufficient_scope. auth.ploid.com is a separate OpenID Connect issuer for workspace login (scopes openid, profile, email, offline_access) and is not the API authorization server.
overview: 'Ploid publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ploid API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ploid
provider_slug: ploid
schemes: []
scope_count: 6
scope_names:
- agent:chat
- people:search
- people:enrich
- linkedin:read
- account:read
- account:write
scopes:
- description: Use the harness context and chat completions
  flows: []
  scope: agent:chat
- description: Search the public people index; also required for the People Sets preview
  flows: []
  scope: people:search
- description: Enrich supported profile and contact fields (POST /v1/person, POST /v1/enrich, POST /v1/socials require people:enrich)
  flows: []
  scope: people:enrich
- description: Read the documented public LinkedIn operations
  flows: []
  scope: linkedin:read
- description: Read usage and credits or revoke the caller key
  flows: []
  scope: account:read
- description: Granted to CLI-created keys by default (docs list it among the CLI's default permissions); no operation-level documentation.
  flows: []
  scope: account:write
slug: ploid-scopes
source_filename: ploid-scopes.yml
source_heading: OAuth Scopes
source_url: https://ploid.com/documentation/getting-started/authentication
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: https://ploid.com/documentation/getting-started/authentication\ndocs: https://ploid.com/documentation/getting-started/authentication\nsources:\n  - https://ploid.com/documentation/getting-started/authentication\n  - https://ploid.com/.well-known/oauth-protected-resource\n  - https://api.ploid.com/.well-known/oauth-authorization-server\n  - https://auth.ploid.com/.well-known/openid-configuration\n  - https://ploid.com/documentation/mcp\nnote: >-\n  The OpenAPI document declares bearer and x-api-key schemes with no oauth2 scheme, so scopes are\n  documented rather than derived. API keys are permissioned with these scopes; the hosted MCP server is\n  an OAuth 2.1 protected resource whose metadata lists agent:chat, people:enrich, people:search and\n  account:read. An endpoint called without its required permission returns 403 insufficient_scope.\n  auth.ploid.com is a separate OpenID Connect issuer for workspace login (scopes openid,\
  \ profile, email,\n  offline_access) and is not the API authorization server.\nscopes:\n  - scope: agent:chat\n    description: Use the harness context and chat completions\n    operations: [getHarnessContext, createHarnessChatCompletion]\n    mcp_granted: true\n  - scope: people:search\n    description: Search the public people index; also required for the People Sets preview\n    operations: [syncPeopleSearch, resolvePerson]\n    mcp_granted: true\n  - scope: people:enrich\n    description: Enrich supported profile and contact fields (POST /v1/person, POST /v1/enrich, POST /v1/socials require people:enrich)\n    operations: [getPerson, getPersonRun, cancelPersonRun, enrichPerson, enrichSocialProfile]\n    mcp_granted: true\n  - scope: linkedin:read\n    description: Read the documented public LinkedIn operations\n    operations: [getLinkedInProfile, searchLinkedInPeople, listLinkedInPosts, listLinkedInProfileComments, getLinkedInCompany, listLinkedInCompanyPosts]\n    mcp_granted: false\n\
  \  - scope: account:read\n    description: Read usage and credits or revoke the caller key\n    operations: [getCredits, getAccountUsage, revokeCurrentApiKey]\n    mcp_granted: true\n  - scope: account:write\n    description: Granted to CLI-created keys by default (docs list it among the CLI's default permissions); no operation-level documentation.\n    mcp_granted: false\noauth_metadata:\n  protected_resource: https://api.ploid.com/mcp\n  authorization_servers: [https://api.ploid.com]\n  scopes_supported: [agent:chat, people:enrich, people:search, account:read]\n  bearer_methods_supported: [header]\n  resource_documentation: https://ploid.com/documentation/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/scopes/ploid-scopes.yml
summary_line: 6 scopes
tags:
- Company
- People Data
- People Search
- Contact Enrichment
- Sales Intelligence
- Recruiting
- LinkedIn
- MCP
- Agents
- Data Enrichment
token_bound: false
token_urls: []
---
