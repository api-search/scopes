---
api_specs:
- filename: cloro-dev-async-api-openapi.yml
  format: yaml
  label: cloro Async API
  slug: cloro-dev-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-async-api-openapi.yml
- filename: cloro-dev-countries-api-openapi.yml
  format: yaml
  label: cloro Countries API
  slug: cloro-dev-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-countries-api-openapi.yml
- filename: cloro-dev-credits-api-openapi.yml
  format: yaml
  label: cloro Credits API
  slug: cloro-dev-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-credits-api-openapi.yml
- filename: cloro-dev-monitor-api-openapi.yml
  format: yaml
  label: cloro Monitor API
  slug: cloro-dev-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-monitor-api-openapi.yml
- filename: cloro-dev-states-api-openapi.yml
  format: yaml
  label: cloro States API
  slug: cloro-dev-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-states-api-openapi.yml
authorization_urls: []
description: ''
docs: https://cloro.dev/docs/integrations/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cloro Dev Scopes
name_suffix: OAuth Scopes
note: Scope descriptions are derived from the Clerk authorization-server metadata (claims_supported) and the provider's MCP page; cloro publishes no separate scopes reference. Tokens are verified by the MCP server against the issuer's JWKS; the API key path (Authorization Bearer or key-in-URL) needs no scopes.
overview: 'cloro publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the cloro API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: cloro
provider_slug: cloro-dev
schemes: []
scope_count: 3
scope_names:
- profile
- email
- user:org:read
scopes:
- description: OpenID Connect profile claims (name, given_name, family_name, picture, preferred_username) for the signed-in cloro user. Listed in scopes_supported of the protected-resource document.
  flows: []
  scope: profile
- description: The signed-in user's email and email_verified claims. Listed in scopes_supported of the protected-resource document.
  flows: []
  scope: email
- description: Read the user's organization membership (org_id claim) so the MCP server can bill tool calls to the organization selected at sign-in ("select the organization whose credits pay for the calls"). Listed in scopes_supported of both the protected-resource and the authorization-server documents.
  flows: []
  scope: user:org:read
slug: cloro-dev-scopes
source_filename: cloro-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: https://mcp.cloro.dev/.well-known/oauth-protected-resource (HTTP 200, 2026-10-07); https://clerk.cloro.dev/.well-known/oauth-authorization-server (HTTP 200, 2026-10-07); https://cloro.dev/docs/integrations/mcp\ndocs: https://cloro.dev/docs/integrations/mcp\napplies_to: cloro MCP server (https://mcp.cloro.dev/mcp) only. The REST API at api.cloro.dev uses a bearer API key with no OAuth and no per-key scopes (\"per-key scopes are not available, so a client cannot request a narrower permission\" - openapi/cloro-dev-openapi.yml bearerAuth description).\nresource: https://mcp.cloro.dev/mcp\nauthorization_servers:\n- https://clerk.cloro.dev\nauthorization_server_metadata:\n  issuer: https://clerk.cloro.dev\n  authorization_endpoint: https://clerk.cloro.dev/oauth/authorize\n  token_endpoint: https://clerk.cloro.dev/oauth/token\n  revocation_endpoint: https://clerk.cloro.dev/oauth/token/revoke\n  device_authorization_endpoint: https://clerk.cloro.dev/oauth/device_authorization\n\
  \  jwks_uri: https://clerk.cloro.dev/.well-known/jwks.json\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:device_code']\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, none, client_secret_post]\n  client_id_metadata_document_supported: true\nscopes:\n- name: profile\n  description: OpenID Connect profile claims (name, given_name, family_name, picture, preferred_username) for the signed-in cloro user. Listed in scopes_supported of the protected-resource document.\n- name: email\n  description: The signed-in user's email and email_verified claims. Listed in scopes_supported of the protected-resource document.\n- name: user:org:read\n  description: Read the user's organization membership (org_id claim) so the MCP server can bill tool calls to the organization selected at sign-in (\"select the organization whose credits pay for the calls\"). Listed in scopes_supported of both the protected-resource\
  \ and the authorization-server documents.\nauthorization_server_only_scopes:\n- openid\n- public_metadata\n- private_metadata\n- offline_access\nnote: Scope descriptions are derived from the Clerk authorization-server metadata (claims_supported) and the provider's MCP page; cloro publishes no separate scopes reference. Tokens are verified by the MCP server against the issuer's JWKS; the API key path (Authorization Bearer or key-in-URL) needs no scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/scopes/cloro-dev-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Search
- AI
- Web Scraping
- SERP
- Generative Engine Optimization
- SEO
- Brand Monitoring
- Market Research
- Data Extraction
- MCP
token_bound: false
token_urls: []
---
