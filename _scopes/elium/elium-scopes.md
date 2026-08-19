---
authorization_urls:
- https://{platform}.elium.com/oauth/authorize
description: ''
docs: https://learn.elium.com/en/api/getting_started/authentication
flows:
- authorizationCode
- password
kind: oauth-scopes
layout: scope
method: searched
name: Elium Scopes
name_suffix: OAuth Scopes
note: 'Derived nothing from OpenAPI - Elium publishes none. Read from the provider''s authentication guide and quick-start, both of which name exactly one scope. There is no scopes/permissions reference page beyond this, and no per-resource or read/write split: apiv1 is the whole API surface.'
overview: 'Elium publishes 1 OAuth 2.0 scope via the authorizationCode and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Elium API on a user''s behalf.


  Tokens are issued from https://{platform}.elium.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Elium
provider_slug: elium
schemes:
- flows:
  - authorizationUrl: https://{platform}.elium.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{platform}.elium.com/oauth/token
  - flow: password
    tokenUrl: https://{platform}.elium.com/oauth/token
  name: OAuth2
  source: https://learn.elium.com/en/api/getting_started/authentication
scope_count: 1
scope_names:
- apiv1
scopes:
- description: The single scope covering the entire Elium API. Granted on behalf of one Elium user; the effective permissions are that user's own content permissions, not the scope's.
  flows:
  - authorizationCode
  - password
  scope: apiv1
slug: elium-scopes
source_filename: elium-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: https://learn.elium.com/en/api/getting_started/authentication\ndocs: https://learn.elium.com/en/api/getting_started/authentication\nnote: >-\n  Derived nothing from OpenAPI - Elium publishes none. Read from the provider's authentication guide and\n  quick-start, both of which name exactly one scope. There is no scopes/permissions reference page beyond\n  this, and no per-resource or read/write split: apiv1 is the whole API surface.\nschemes:\n- name: OAuth2\n  source: https://learn.elium.com/en/api/getting_started/authentication\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{platform}.elium.com/oauth/authorize\n    tokenUrl: https://{platform}.elium.com/oauth/token\n  - flow: password\n    tokenUrl: https://{platform}.elium.com/oauth/token\nscope_count: 1\nscopes:\n- scope: apiv1\n  description: >-\n    The single scope covering the entire Elium API. Granted on behalf of one Elium user; the effective\n\
  \    permissions are that user's own content permissions, not the scope's.\n  flows: [authorizationCode, password]\n  sources: [https://learn.elium.com/en/api/getting_started/authentication]\ngaps:\n- One coarse scope for 17 queries, 206 mutations and 18 subscriptions - an agent cannot be granted\n  read-only API access at the OAuth layer. Read-only agent access is instead offered as a separate\n  product surface (the MCP server, whose three published tools are all read-only).\n- No incremental or step-up authorization, and no scope documentation page distinct from the auth guide.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elium/refs/heads/main/scopes/elium-scopes.yml
summary_line: 1 scope · authorizationCode/password
tags:
- Company
- SaaS
- Knowledge Management
- Knowledge Base
- Enterprise Search
- AI Search
- GraphQL
- MCP
- Collaboration
- Documentation
- RAG
- Europe
token_urls:
- https://{platform}.elium.com/oauth/token
---
