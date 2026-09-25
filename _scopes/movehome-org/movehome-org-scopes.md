---
api_specs:
- filename: movehome-org-raia-portal-feed-openapi.yaml
  format: yaml
  label: RAIA Portal Feed API (MoveHome.org implementation)
  slug: raia-portal-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/movehome-org/refs/heads/main/openapi/movehome-org-raia-portal-feed-openapi.yaml
authorization_urls: []
description: ''
docs: https://github.com/MoveHome/MoveHome.Org/blob/main/docs/raia-portal-feed-api.md#2-getting-credentials
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Movehome Org Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Move Home Organisation CIC publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Move Home Organisation CIC API on a user''s behalf.


  Tokens are issued from https://movehome.org/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Move Home Organisation CIC
provider_slug: movehome-org
schemes:
- client_authentication: HTTP Basic or form client_id / client_secret
  description: 'Server-to-server OAuth2 client credentials flow. The token endpoint is

    published by the implementer; credentials are issued out-of-band

    during onboarding. Tokens are short-lived Bearer JWTs.'
  flows:
  - flow: clientCredentials
    note: The standard's OpenAPI carries an implementer placeholder; MoveHome's docs and the live 401 (WWW-Authenticate Bearer realm="raia-portal-feed") fix the real issuer. Bound in overlays/movehome-org-raia-portal-feed-overlay.yaml.
    tokenUrl: https://movehome.org/oauth/token
    tokenUrl_in_spec: https://feed.example.com/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/movehome-org-raia-portal-feed-openapi.yaml
  token: HS256 JWT, 1-hour TTL, jti audit-logged
scope_count: 3
scope_names:
- feed.read
- feed.write
- products.write
scopes:
- description: Read listings, branches, performance and enquiries.
  flows:
  - clientCredentials
  scope: feed.read
- description: Upsert and remove listings.
  flows:
  - clientCredentials
  scope: feed.write
- description: Request portal product activations.
  flows:
  - clientCredentials
  scope: products.write
slug: movehome-org-scopes
source_filename: movehome-org-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/movehome-org-raia-portal-feed-openapi.yaml\ndocs: https://github.com/MoveHome/MoveHome.Org/blob/main/docs/raia-portal-feed-api.md#2-getting-credentials\ntoken_url: https://movehome.org/oauth/token\nsummary: >-\n  Three OAuth 2.0 scopes, all on the RAIA Portal Feed API's client-credentials flow, declared in the\n  OpenAPI's OAuth2ClientCredentials scheme and documented identically in MoveHome's integrator guide. A\n  credential is bound to one agent and an ALLOWED set of scopes at issuance; a token request's scope is\n  intersected with that set, and omitting scope grants every allowed scope. The agent surfaces (A2A, both\n  MCP servers) and the registry API have no scopes because they have no authentication.\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/movehome-org-raia-portal-feed-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://movehome.org/oauth/token\n    tokenUrl_in_spec:\
  \ https://feed.example.com/oauth/token\n    note: The standard's OpenAPI carries an implementer placeholder; MoveHome's docs and the live 401 (WWW-Authenticate Bearer realm=\"raia-portal-feed\") fix the real issuer. Bound in overlays/movehome-org-raia-portal-feed-overlay.yaml.\n  token: HS256 JWT, 1-hour TTL, jti audit-logged\n  client_authentication: HTTP Basic or form client_id / client_secret\n  description: |-\n    Server-to-server OAuth2 client credentials flow. The token endpoint is\n    published by the implementer; credentials are issued out-of-band\n    during onboarding. Tokens are short-lived Bearer JWTs.\nscopes:\n- scope: feed.read\n  description: Read listings, branches, performance and enquiries.\n  grants: [getListing, listBranchListings, getBranchPerformance, listBranchEnquiries, listPremiumListingActivations, getPremiumListingActivation, listFeaturedPropertyActivations, getFeaturedPropertyActivation]\n  flows: [clientCredentials]\n  sources: [openapi/movehome-org-raia-portal-feed-openapi.yaml,\
  \ docs §2]\n- scope: feed.write\n  description: Upsert and remove listings.\n  grants: [upsertListing, deleteListing]\n  flows: [clientCredentials]\n  sources: [openapi/movehome-org-raia-portal-feed-openapi.yaml, docs §2]\n- scope: products.write\n  description: Request portal product activations.\n  grants: [requestPremiumListingActivation, requestFeaturedPropertyActivation]\n  flows: [clientCredentials]\n  sources: [openapi/movehome-org-raia-portal-feed-openapi.yaml, docs §2]\nunscoped:\n- {operation: getHealth, note: 'security: [] in the spec; live 200 without a token'}\n- {surface: 'A2A https://movehome.org/api/a2a', note: no authentication or scopes}\n- {surface: 'MCP https://movehome.org/mcp and /api/registry/mcp', note: no authentication or scopes}\n- {surface: 'Registry REST https://movehome.org/api/registry/v1', note: no authentication or scopes}\nscope_count: 3\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/movehome-org/refs/heads/main/scopes/movehome-org-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Real Estate
- Property
- Lettings
- Property Sales
- Agents
- A2A
- MCP
- Agent-Native
- Agent Registry
- Non-Profit
- Open Source
- RAIA Protocol
- United Kingdom
token_urls:
- https://movehome.org/oauth/token
---
