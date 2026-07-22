---
api_specs:
- filename: nomos-openapi-original.json
  format: json
  label: Nomos API
  slug: nomos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.nomos.energy/api-references/authentication#scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Nomos Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares http Bearer (JWT) + Basic security schemes, but the bearer token is minted through an OAuth 2.0 flow (RFC 6749). Scopes are documented on the authentication page, not in the spec's securitySchemes, so this artifact is searched from the docs.
overview: 'Nomos publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nomos API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nomos
provider_slug: nomos
schemes:
- authorization_endpoint: https://api.nomos.energy/oauth/authorize
  grant_types:
  - client_credentials
  - authorization_code
  - refresh_token
  metadata: https://api.nomos.energy/.well-known/oauth-authorization-server
  name: OAuth2
  token_endpoint: https://api.nomos.energy/oauth/token
  token_endpoint_auth: client_secret_basic
  token_ttl_seconds: 3600
  type: oauth2
scope_count: 2
scope_names:
- read:*
- write:*
scopes:
- description: All GET requests across the API (the entire read surface).
  flows: []
  scope: read:*
- description: All non-GET requests (POST, PATCH, PUT, DELETE). A key without write:* is rejected with 403 FORBIDDEN on any mutating request.
  flows: []
  scope: write:*
slug: nomos-scopes
source_filename: nomos-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nomos-openapi-original.json\ndocs: https://docs.nomos.energy/api-references/authentication#scopes\nnote: >-\n  The OpenAPI declares http Bearer (JWT) + Basic security schemes, but the\n  bearer token is minted through an OAuth 2.0 flow (RFC 6749). Scopes are\n  documented on the authentication page, not in the spec's securitySchemes,\n  so this artifact is searched from the docs.\nschemes:\n- name: OAuth2\n  type: oauth2\n  authorization_endpoint: https://api.nomos.energy/oauth/authorize\n  token_endpoint: https://api.nomos.energy/oauth/token\n  metadata: https://api.nomos.energy/.well-known/oauth-authorization-server\n  grant_types:\n  - client_credentials      # server-to-server against your own org data (most integrations)\n  - authorization_code      # acting on behalf of an end customer (PKCE, S256/plain)\n  - refresh_token\n  token_endpoint_auth: client_secret_basic\n  token_ttl_seconds: 3600\nscopes:\n- scope:\
  \ 'read:*'\n  description: All GET requests across the API (the entire read surface).\n  applies_to: [GET]\n- scope: 'write:*'\n  description: >-\n    All non-GET requests (POST, PATCH, PUT, DELETE). A key without write:* is\n    rejected with 403 FORBIDDEN on any mutating request.\n  applies_to: [POST, PATCH, PUT, DELETE]\nnotes: >-\n  Scopes are fixed when a key is created and cannot be narrowed per request;\n  rotate to a new key to change scope. The wildcard scopes are supersets:\n  resource-named scopes (read:invoice, write:subscription) may be introduced\n  later. Default full-access key carries \"read:* write:*\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/scopes/nomos-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Energy
- Electricity
- Utilities
- Embedded Finance
- Dynamic Pricing
- Billing
- Metering
- Smart Meter
- Germany
- OAuth
- Webhooks
token_urls: []
---
