---
api_specs:
- filename: statable-stats-api-openapi.yml
  format: yaml
  label: Statable Stats API
  slug: statable-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statable-stats-api/refs/heads/main/openapi/statable-stats-api-openapi.yml
authorization_urls: []
description: ''
docs: https://statable.com/docs/integrations/mcp/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Statable Stats Api Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Statable Stats API publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Statable Stats API API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Statable Stats API
provider_slug: statable-stats-api
schemes: []
scope_count: 2
scope_names:
- read
- sites:write
scopes:
- description: Read analytics — visitors, pageviews, sources, goals, funnels, live visitors. Always granted.
  flows:
  - authorizationCode
  scope: read
- description: Create and configure sites, goals, funnels, tracking settings and filters. Granted on the OAuth consent screen.
  flows:
  - authorizationCode
  scope: sites:write
slug: statable-stats-api-scopes
source_filename: statable-stats-api-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: https://statable.com/.well-known/oauth-authorization-server\ndocs: https://statable.com/docs/integrations/mcp/\n# The REST API authenticates with an stbl_ bearer key whose PERMISSIONS (Read analytics,\n# Manage sites, Manage API keys) are fixed at creation. The OAuth 2.1 surface that fronts the\n# MCP server uses SCOPES, advertised in RFC 8414 metadata. Both are recorded here.\noauth:\n  authorization_server: https://statable.com\n  issuer: https://statable.com\n  authorization_endpoint: https://statable.com/api/oauth/authorize\n  token_endpoint: https://statable.com/api/oauth/token\n  registration_endpoint: https://statable.com/api/oauth/register   # RFC 7591 Dynamic Client Registration\n  revocation_endpoint: https://statable.com/api/oauth/revoke\n  grant_types: [authorization_code, refresh_token]\n  code_challenge_methods: [S256]                                    # PKCE required\n  token_endpoint_auth_methods: [none]  \
  \                             # public clients\nscopes:\n  - scope: read\n    description: Read analytics — visitors, pageviews, sources, goals, funnels, live visitors. Always granted.\n    flows: [authorizationCode]\n  - scope: sites:write\n    description: Create and configure sites, goals, funnels, tracking settings and filters. Granted on the OAuth consent screen.\n    flows: [authorizationCode]\nkey_permissions:\n  # stbl_ API-key permissions (fixed at key creation; not OAuth scopes)\n  - name: Read analytics\n    always_on: true\n  - name: Manage sites\n    description: create/update sites, goals, funnels, tracking settings; can delete site data and make analytics public\n  - name: Manage API keys\n    description: create, rotate and revoke other keys\nnotes:\n  - \"billing:write is referenced in docs as a scope that CANNOT be obtained via the HTTP bootstrap (400 invalid_scope); it is not advertised in the MCP OAuth scopes_supported.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statable-stats-api/refs/heads/main/scopes/statable-stats-api-scopes.yml
summary_line: 2 scopes
tags:
- Analytics
- Web Analytics
- Cookieless
- Privacy
- GDPR
- OpenAPI
- MCP
- llms-txt
- EU-hosted
token_urls: []
---
