---
api_specs:
- filename: kannkidas-de-openapi.yml
  format: yaml
  label: Kann KI das? API
  slug: kann-ki-das-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kannkidas-de/refs/heads/main/openapi/kannkidas-de-openapi.yml
authorization_urls: []
description: ''
docs: https://kannkidas.de/auth.md
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Kannkidas De Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kann KI das? Sponsoring Agent publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kann KI das? Sponsoring Agent API on a user''s behalf.


  Tokens are issued from https://kannkidas.de/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kann KI das? Sponsoring Agent
provider_slug: kannkidas-de
schemes:
- flows:
  - default_scope: sponsorship:read
    flow: clientCredentials
    registrationUrl: https://kannkidas.de/api/agent/register
    tokenUrl: https://kannkidas.de/api/oauth/token
    token_endpoint_auth_method: client_secret_basic
  name: oauth2
  source: openapi/kannkidas-de-openapi.yml
scope_count: 2
scope_names:
- sponsorship:read
- sponsorship:write
scopes:
- description: Read own purchase status
  flows:
  - clientCredentials
  scope: sponsorship:read
- description: Create a confirmed checkout
  flows:
  - clientCredentials
  scope: sponsorship:write
slug: kannkidas-de-scopes
source_filename: kannkidas-de-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/kannkidas-de-openapi.yml\ndocs: https://kannkidas.de/auth.md\ndiscovery:\n  authorization_server_metadata: https://kannkidas.de/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://kannkidas.de/.well-known/oauth-protected-resource\n  scopes_supported: [sponsorship:read, sponsorship:write]\n  note: Both served documents list exactly the two scopes the OpenAPI declares; the derived baseline and the docs agree.\nschemes:\n- name: oauth2\n  source: openapi/kannkidas-de-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://kannkidas.de/api/oauth/token\n    registrationUrl: https://kannkidas.de/api/agent/register\n    token_endpoint_auth_method: client_secret_basic\n    default_scope: sponsorship:read\nscopes:\n- scope: sponsorship:read\n  description: Read own purchase status\n  flows:\n  - clientCredentials\n  granted_by_default: true\n  operations: [getSponsorPurchase]\n  docs_note:\
  \ 'auth.md: registration grants only sponsorship:read by default; a token request without a scope parameter also defaults to read-only.'\n  sources:\n  - openapi/kannkidas-de-openapi.yml\n  - https://kannkidas.de/auth.md\n- scope: sponsorship:write\n  description: Create a confirmed checkout\n  flows:\n  - clientCredentials\n  granted_by_default: false\n  operations: [createSponsorPurchase]\n  docs_note: 'auth.md: request scopes [\"sponsorship:read\",\"sponsorship:write\"] explicitly at registration only when the buyer intends to create a checkout; AGENTS.md: use the smallest required scope.'\n  sources:\n  - openapi/kannkidas-de-openapi.yml\n  - https://kannkidas.de/auth.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kannkidas-de/refs/heads/main/scopes/kannkidas-de-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- Sponsoring
- Advertising
- Software Reviews
- Build vs Buy
- Search
- agent-native
- MCP
- A2A
- Authentication
- x402
- Stripe Checkout
- Germany
token_urls:
- https://kannkidas.de/api/oauth/token
---
