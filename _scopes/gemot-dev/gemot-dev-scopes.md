---
api_specs:
- filename: gemot-dev-a2a-api-openapi.yml
  format: yaml
  label: Gemot A2a API
  slug: gemot-dev-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-a2a-api-openapi.yml
- filename: gemot-dev-balance-api-openapi.yml
  format: yaml
  label: Gemot Balance API
  slug: gemot-dev-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-balance-api-openapi.yml
- filename: gemot-dev-checkout-api-openapi.yml
  format: yaml
  label: Gemot Checkout API
  slug: gemot-dev-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-checkout-api-openapi.yml
- filename: gemot-dev-events-api-openapi.yml
  format: yaml
  label: Gemot Events API
  slug: gemot-dev-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-events-api-openapi.yml
- filename: gemot-dev-export-api-openapi.yml
  format: yaml
  label: Gemot Export API
  slug: gemot-dev-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-export-api-openapi.yml
- filename: gemot-dev-health-api-openapi.yml
  format: yaml
  label: Gemot Health API
  slug: gemot-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-health-api-openapi.yml
- filename: gemot-dev-join-api-openapi.yml
  format: yaml
  label: Gemot Join API
  slug: gemot-dev-join-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-join-api-openapi.yml
- filename: gemot-dev-oauth-api-openapi.yml
  format: yaml
  label: Gemot OAuth API
  slug: gemot-dev-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-oauth-api-openapi.yml
- filename: gemot-dev-try-api-openapi.yml
  format: yaml
  label: Gemot Try API
  slug: gemot-dev-try-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-try-api-openapi.yml
- filename: gemot-dev-well-known-api-openapi.yml
  format: yaml
  label: Gemot .well Known API
  slug: gemot-dev-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-well-known-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Gemot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Gemot publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gemot API on a user''s behalf.


  Tokens are issued from https://gemot.dev/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gemot
provider_slug: gemot-dev
schemes:
- description: 'Client-credentials facade over the same API key: the key IS the client_secret. See /.well-known/oauth-authorization-server.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://gemot.dev/oauth/token
  name: oauth2ClientCredentials
  source: openapi/gemot-dev-openapi.json
scope_count: 1
scope_names:
- deliberate
scopes:
- description: Full access to all seven grouped tools, scoped to the underlying API key's own permissions and credit balance.
  flows:
  - clientCredentials
  scope: deliberate
slug: gemot-dev-scopes
source_filename: gemot-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/gemot-dev-openapi.json\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/gemot-dev-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://gemot.dev/oauth/token\n  description: 'Client-credentials facade over the same API key: the key IS the client_secret.\n    See /.well-known/oauth-authorization-server.'\nscopes:\n- scope: deliberate\n  description: Full access to all seven grouped tools, scoped to the underlying API key's own\n    permissions and credit balance.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/gemot-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/gemot-dev/scopes/gemot-dev-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Governance
- Decentralization
- Autonomous Organizations
- Coordination
- Open Protocol
token_bound: false
token_urls:
- https://gemot.dev/oauth/token
---
