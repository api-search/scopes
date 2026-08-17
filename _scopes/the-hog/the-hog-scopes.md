---
api_specs:
- filename: the-hog-company-search-api-openapi.yml
  format: yaml
  label: The Hog Company Search API
  slug: the-hog-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-company-search-api-openapi.yml
- filename: the-hog-deep-research-api-openapi.yml
  format: yaml
  label: The Hog Deep Research API
  slug: the-hog-deep-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-deep-research-api-openapi.yml
- filename: the-hog-enrichments-api-openapi.yml
  format: yaml
  label: The Hog Enrichments API
  slug: the-hog-enrichments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-enrichments-api-openapi.yml
- filename: the-hog-monitors-api-openapi.yml
  format: yaml
  label: The Hog Monitors API
  slug: the-hog-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-monitors-api-openapi.yml
- filename: the-hog-operations-api-openapi.yml
  format: yaml
  label: The Hog Operations API
  slug: the-hog-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-operations-api-openapi.yml
- filename: the-hog-people-search-api-openapi.yml
  format: yaml
  label: The Hog People Search API
  slug: the-hog-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-people-search-api-openapi.yml
- filename: the-hog-scrapers-api-openapi.yml
  format: yaml
  label: The Hog Scrapers API
  slug: the-hog-scrapers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-scrapers-api-openapi.yml
- filename: the-hog-search-api-openapi.yml
  format: yaml
  label: The Hog Search API
  slug: the-hog-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-search-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.thehog.ai/guides/use-mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: The Hog Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'The Hog uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: The Hog
provider_slug: the-hog
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: the-hog-scopes
source_filename: the-hog-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.thehog.ai/.well-known/oauth-authorization-server\nchecked: '2026-08-14'\nhttp_status: 200\ndocs: https://docs.thehog.ai/guides/use-mcp\n\nscope_count: 7\nscope_model: oauth2-authorization-code-pkce\napplies_to: hosted MCP server (https://mcp.thehog.ai/mcp)\n\nimportant: >-\n  These are NOT REST API authorization scopes. The Hog's REST API at\n  https://developer.thehog.ai is authorized with a static dual API-key header pair\n  (X-Access-Key / X-Secret-Key) and declares NO oauth2 securityScheme in its\n  OpenAPI -- there is no scope model on the REST surface at all, so an agent cannot\n  request least-privilege access to the API itself. The scopes below govern only the\n  OAuth handshake that fronts the hosted MCP server, and they are Clerk identity\n  scopes (the authorization server is a Clerk tenant at clerk.thehog.ai, whose own\n  service_documentation points at clerk.com/docs/oauth/scoped-access). None of them\n\
  \  narrows what a connected agent may DO with The Hog data once the token is issued.\n\nauthorization_server:\n  issuer: https://clerk.thehog.ai\n  authorization_endpoint: https://clerk.thehog.ai/oauth/authorize\n  token_endpoint: https://clerk.thehog.ai/oauth/token\n  revocation_endpoint: https://clerk.thehog.ai/oauth/token/revoke\n  registration_endpoint: https://clerk.thehog.ai/oauth/register\n  registration_note: >-\n    RFC 7591 dynamic client registration is open, which is what lets an MCP client\n    connect without a pre-provisioned client_id.\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, none]\n  id_token_signing_alg_values_supported: [RS256]\n  jwks_uri: https://clerk.thehog.ai/.well-known/jwks.json\n  claims_supported: [sub, iss, aud, exp, iat, email, name, org_id]\n\nprotected_resource:\n  resource:\
  \ https://mcp.thehog.ai/\n  authorization_servers: [https://clerk.thehog.ai]\n  authorization_data_types_supported: [oauth_scope]\n  authorization_data_locations_supported: [header, body]\n  source: https://mcp.thehog.ai/.well-known/oauth-protected-resource\n\nscopes:\n  - name: openid\n    kind: identity\n    description: OpenID Connect base scope; requests an ID token for the signed-in user.\n  - name: profile\n    kind: identity\n    description: Basic profile claims for the signed-in user (name).\n  - name: email\n    kind: identity\n    description: The signed-in user's email address claim.\n  - name: public_metadata\n    kind: identity\n    description: Clerk public user metadata attached to the account.\n  - name: private_metadata\n    kind: identity\n    description: Clerk private user metadata attached to the account.\n  - name: offline_access\n    kind: session\n    description: >-\n      Issues a refresh token so the MCP client can keep the connection alive without\n      re-prompting\
  \ the user.\n  - name: user:org:read\n    kind: organization\n    description: >-\n      Read the organizations the user belongs to. This is the scope that lets the MCP\n      connect flow present the organization picker -- The Hog bills and rate-limits\n      per organization-and-user, so the selected org determines which balance the\n      agent's calls are charged against.\n\ngaps:\n  - >-\n    No resource scopes. Nothing in scopes_supported distinguishes read from write,\n    search from enrichment, or monitors from scrapers. An agent granted MCP access\n    holds the full published tool surface for the selected organization.\n  - >-\n    No scope model on the REST API. The OpenAPI declares only apiKey schemes, so REST\n    consumers get all-or-nothing credentials with no per-capability narrowing.\n  - >-\n    Spend, not scope, is the control. The published cost boundary is the customer-set\n    spend cap on the pricing page, not an authorization boundary.\n\nrefs:\n  authentication:\
  \ authentication/the-hog-authentication.yml\n  well_known: well-known/the-hog-well-known.yml\n  mcp: mcp/the-hog-mcp.yml\n  plans: plans/the-hog-plans-pricing.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/scopes/the-hog-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- GTM Intelligence
- Sales Intelligence
- Data Enrichment
- Web Scraping
- People Data
- Company Data
- Deep Research
- Social Monitoring
- MCP
- AI Agents
- Y Combinator
token_urls: []
---
